# 导入API到已有分组<a name="ZH-CN_TOPIC_0000001081976231"></a>

## 功能介绍<a name="zh-cn_topic_0225569014_section39777523194"></a>

导入swagger格式的文件, 在已有分组中创建或更新API。swagger文件支持json以及yaml格式。

## URI<a name="zh-cn_topic_0225569014_section1199919551442"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1** 

<a name="zh-cn_topic_0225569014_table1030719520475"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row1130715217477"><th class="cellrowborder" valign="top" width="20.57%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225569014_p130795213478"><a name="zh-cn_topic_0225569014_p130795213478"></a><a name="zh-cn_topic_0225569014_p130795213478"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="79.43%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225569014_p13307135204712"><a name="zh-cn_topic_0225569014_p13307135204712"></a><a name="zh-cn_topic_0225569014_p13307135204712"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row15307252144718"><td class="cellrowborder" valign="top" width="20.57%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569014_p1930714525475"><a name="zh-cn_topic_0225569014_p1930714525475"></a><a name="zh-cn_topic_0225569014_p1930714525475"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="79.43%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569014_p19454226101515"><a name="zh-cn_topic_0225569014_p19454226101515"></a><a name="zh-cn_topic_0225569014_p19454226101515"></a>/v1/{project_id}/apigw/instances/{instance_id}/openapi?group_id={0}&amp;mode={1}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225569014_table871144945810"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row14734499589"><th class="cellrowborder" valign="top" width="17.87178717871787%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p1973174918589"><a name="zh-cn_topic_0225569014_p1973174918589"></a><a name="zh-cn_topic_0225569014_p1973174918589"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="14.041404140414041%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p4731749125817"><a name="zh-cn_topic_0225569014_p4731749125817"></a><a name="zh-cn_topic_0225569014_p4731749125817"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.511151115111511%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p1730491589"><a name="zh-cn_topic_0225569014_p1730491589"></a><a name="zh-cn_topic_0225569014_p1730491589"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="56.57565756575658%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p1073649175817"><a name="zh-cn_topic_0225569014_p1073649175817"></a><a name="zh-cn_topic_0225569014_p1073649175817"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row19924920720"><td class="cellrowborder" valign="top" width="17.87178717871787%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p55878963"><a name="zh-cn_topic_0225569014_p55878963"></a><a name="zh-cn_topic_0225569014_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.041404140414041%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p29902160"><a name="zh-cn_topic_0225569014_p29902160"></a><a name="zh-cn_topic_0225569014_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="11.511151115111511%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p6155914"><a name="zh-cn_topic_0225569014_p6155914"></a><a name="zh-cn_topic_0225569014_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57565756575658%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p28867016"><a name="zh-cn_topic_0225569014_p28867016"></a><a name="zh-cn_topic_0225569014_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row111589478711"><td class="cellrowborder" valign="top" width="17.87178717871787%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1780913159538"><a name="zh-cn_topic_0225569014_p1780913159538"></a><a name="zh-cn_topic_0225569014_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.041404140414041%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p9809215115310"><a name="zh-cn_topic_0225569014_p9809215115310"></a><a name="zh-cn_topic_0225569014_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="11.511151115111511%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1280914152538"><a name="zh-cn_topic_0225569014_p1280914152538"></a><a name="zh-cn_topic_0225569014_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57565756575658%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1880914157537"><a name="zh-cn_topic_0225569014_p1880914157537"></a><a name="zh-cn_topic_0225569014_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row15201144012331"><td class="cellrowborder" valign="top" width="17.87178717871787%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p142011240183311"><a name="zh-cn_topic_0225569014_p142011240183311"></a><a name="zh-cn_topic_0225569014_p142011240183311"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.041404140414041%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p112014407332"><a name="zh-cn_topic_0225569014_p112014407332"></a><a name="zh-cn_topic_0225569014_p112014407332"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="11.511151115111511%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p120384023318"><a name="zh-cn_topic_0225569014_p120384023318"></a><a name="zh-cn_topic_0225569014_p120384023318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57565756575658%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p162039406337"><a name="zh-cn_topic_0225569014_p162039406337"></a><a name="zh-cn_topic_0225569014_p162039406337"></a>分组 ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row13868431333"><td class="cellrowborder" valign="top" width="17.87178717871787%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p16386174316334"><a name="zh-cn_topic_0225569014_p16386174316334"></a><a name="zh-cn_topic_0225569014_p16386174316334"></a>mode</p>
</td>
<td class="cellrowborder" valign="top" width="14.041404140414041%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p12386164313315"><a name="zh-cn_topic_0225569014_p12386164313315"></a><a name="zh-cn_topic_0225569014_p12386164313315"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="11.511151115111511%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p03861443143312"><a name="zh-cn_topic_0225569014_p03861443143312"></a><a name="zh-cn_topic_0225569014_p03861443143312"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57565756575658%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p159102715173"><a name="zh-cn_topic_0225569014_p159102715173"></a><a name="zh-cn_topic_0225569014_p159102715173"></a>导入模式，可选merge和override。</p>
<p id="zh-cn_topic_0225569014_p338634311333"><a name="zh-cn_topic_0225569014_p338634311333"></a><a name="zh-cn_topic_0225569014_p338634311333"></a>当API定义冲突时，merge保留原有API，override会覆盖原有API。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row11890741245"><td class="cellrowborder" valign="top" width="17.87178717871787%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p12891154343"><a name="zh-cn_topic_0225569014_p12891154343"></a><a name="zh-cn_topic_0225569014_p12891154343"></a>extend_mode</p>
</td>
<td class="cellrowborder" valign="top" width="14.041404140414041%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p6531195013518"><a name="zh-cn_topic_0225569014_p6531195013518"></a><a name="zh-cn_topic_0225569014_p6531195013518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.511151115111511%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1089114945"><a name="zh-cn_topic_0225569014_p1089114945"></a><a name="zh-cn_topic_0225569014_p1089114945"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57565756575658%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1089213410413"><a name="zh-cn_topic_0225569014_p1089213410413"></a><a name="zh-cn_topic_0225569014_p1089213410413"></a>扩展信息导入模式，可选merge和override。</p>
<p id="zh-cn_topic_0225569014_p10778501566"><a name="zh-cn_topic_0225569014_p10778501566"></a><a name="zh-cn_topic_0225569014_p10778501566"></a>当扩展信息定义冲突时，merge保留原有扩展信息，override会覆盖原有扩展信息。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225569014_section178868115223"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225569014_table9773163143319"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row57739315330"><th class="cellrowborder" valign="top" width="19.801980198019802%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p1777313115338"><a name="zh-cn_topic_0225569014_p1777313115338"></a><a name="zh-cn_topic_0225569014_p1777313115338"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p16773123153311"><a name="zh-cn_topic_0225569014_p16773123153311"></a><a name="zh-cn_topic_0225569014_p16773123153311"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p1077314311338"><a name="zh-cn_topic_0225569014_p1077314311338"></a><a name="zh-cn_topic_0225569014_p1077314311338"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.44554455445545%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p57731931163310"><a name="zh-cn_topic_0225569014_p57731931163310"></a><a name="zh-cn_topic_0225569014_p57731931163310"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row2773153115338"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p207735314331"><a name="zh-cn_topic_0225569014_p207735314331"></a><a name="zh-cn_topic_0225569014_p207735314331"></a>swagger</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p9773153173314"><a name="zh-cn_topic_0225569014_p9773153173314"></a><a name="zh-cn_topic_0225569014_p9773153173314"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p4773123193314"><a name="zh-cn_topic_0225569014_p4773123193314"></a><a name="zh-cn_topic_0225569014_p4773123193314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p67736311339"><a name="zh-cn_topic_0225569014_p67736311339"></a><a name="zh-cn_topic_0225569014_p67736311339"></a>固定值2.0</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row37747316331"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p8774193183317"><a name="zh-cn_topic_0225569014_p8774193183317"></a><a name="zh-cn_topic_0225569014_p8774193183317"></a>info</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1377493113317"><a name="zh-cn_topic_0225569014_p1377493113317"></a><a name="zh-cn_topic_0225569014_p1377493113317"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p6774133117331"><a name="zh-cn_topic_0225569014_p6774133117331"></a><a name="zh-cn_topic_0225569014_p6774133117331"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p147741931103310"><a name="zh-cn_topic_0225569014_p147741931103310"></a><a name="zh-cn_topic_0225569014_p147741931103310"></a>参考<a href="#zh-cn_topic_0225569014_table17777531133316">表4</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row12774431113317"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p277493110331"><a name="zh-cn_topic_0225569014_p277493110331"></a><a name="zh-cn_topic_0225569014_p277493110331"></a>paths</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p177741231183318"><a name="zh-cn_topic_0225569014_p177741231183318"></a><a name="zh-cn_topic_0225569014_p177741231183318"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1977483118331"><a name="zh-cn_topic_0225569014_p1977483118331"></a><a name="zh-cn_topic_0225569014_p1977483118331"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p2774183118334"><a name="zh-cn_topic_0225569014_p2774183118334"></a><a name="zh-cn_topic_0225569014_p2774183118334"></a>参考<a href="#zh-cn_topic_0225569014_table4779143143311">表 paths参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row1775193115334"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p13775103110336"><a name="zh-cn_topic_0225569014_p13775103110336"></a><a name="zh-cn_topic_0225569014_p13775103110336"></a>responses</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p377573120333"><a name="zh-cn_topic_0225569014_p377573120333"></a><a name="zh-cn_topic_0225569014_p377573120333"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p19775153113336"><a name="zh-cn_topic_0225569014_p19775153113336"></a><a name="zh-cn_topic_0225569014_p19775153113336"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p77751231153315"><a name="zh-cn_topic_0225569014_p77751231153315"></a><a name="zh-cn_topic_0225569014_p77751231153315"></a>公用响应定义，可以被引用在{method}的操作中，参考<a href="#zh-cn_topic_0225569014_table1179216319331">表9</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row0775183113319"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p177519318331"><a name="zh-cn_topic_0225569014_p177519318331"></a><a name="zh-cn_topic_0225569014_p177519318331"></a>securityDefinitions</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1377519316332"><a name="zh-cn_topic_0225569014_p1377519316332"></a><a name="zh-cn_topic_0225569014_p1377519316332"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p197751031193315"><a name="zh-cn_topic_0225569014_p197751031193315"></a><a name="zh-cn_topic_0225569014_p197751031193315"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p9775183103319"><a name="zh-cn_topic_0225569014_p9775183103319"></a><a name="zh-cn_topic_0225569014_p9775183103319"></a>定义鉴权方式，参考<a href="#zh-cn_topic_0225569014_table8801831163318">表13</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row15840124816259"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1884194822510"><a name="zh-cn_topic_0225569014_p1884194822510"></a><a name="zh-cn_topic_0225569014_p1884194822510"></a>x-apigateway-access-controls</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p13841148172510"><a name="zh-cn_topic_0225569014_p13841148172510"></a><a name="zh-cn_topic_0225569014_p13841148172510"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1784154813256"><a name="zh-cn_topic_0225569014_p1784154813256"></a><a name="zh-cn_topic_0225569014_p1784154813256"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p384164813253"><a name="zh-cn_topic_0225569014_p384164813253"></a><a name="zh-cn_topic_0225569014_p384164813253"></a>访问控制信息，参考<a href="#zh-cn_topic_0225569014_table2090754816252">表 x-apigateway-access-controls参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row684144814253"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p98411348102518"><a name="zh-cn_topic_0225569014_p98411348102518"></a><a name="zh-cn_topic_0225569014_p98411348102518"></a>x-apigateway-ratelimits</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p13841134852518"><a name="zh-cn_topic_0225569014_p13841134852518"></a><a name="zh-cn_topic_0225569014_p13841134852518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p178411048152517"><a name="zh-cn_topic_0225569014_p178411048152517"></a><a name="zh-cn_topic_0225569014_p178411048152517"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p28411648202513"><a name="zh-cn_topic_0225569014_p28411648202513"></a><a name="zh-cn_topic_0225569014_p28411648202513"></a>流量空时信息，参考<a href="#zh-cn_topic_0225569014_table18913124872513">表 x-apigateway-ratelimits参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 4**  info参数说明

<a name="zh-cn_topic_0225569014_table17777531133316"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row677763153314"><th class="cellrowborder" valign="top" width="19.801980198019802%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p577710314330"><a name="zh-cn_topic_0225569014_p577710314330"></a><a name="zh-cn_topic_0225569014_p577710314330"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p6777531153318"><a name="zh-cn_topic_0225569014_p6777531153318"></a><a name="zh-cn_topic_0225569014_p6777531153318"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p777713120337"><a name="zh-cn_topic_0225569014_p777713120337"></a><a name="zh-cn_topic_0225569014_p777713120337"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.45544554455446%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p3777133113314"><a name="zh-cn_topic_0225569014_p3777133113314"></a><a name="zh-cn_topic_0225569014_p3777133113314"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row1777814313334"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p07787319338"><a name="zh-cn_topic_0225569014_p07787319338"></a><a name="zh-cn_topic_0225569014_p07787319338"></a>title</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p2778193118331"><a name="zh-cn_topic_0225569014_p2778193118331"></a><a name="zh-cn_topic_0225569014_p2778193118331"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p13778183193320"><a name="zh-cn_topic_0225569014_p13778183193320"></a><a name="zh-cn_topic_0225569014_p13778183193320"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p12778123119338"><a name="zh-cn_topic_0225569014_p12778123119338"></a><a name="zh-cn_topic_0225569014_p12778123119338"></a>API分组名称，导入到已有分组时不生效</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row20778153110339"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p177812316339"><a name="zh-cn_topic_0225569014_p177812316339"></a><a name="zh-cn_topic_0225569014_p177812316339"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1177813318338"><a name="zh-cn_topic_0225569014_p1177813318338"></a><a name="zh-cn_topic_0225569014_p1177813318338"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p15778153118331"><a name="zh-cn_topic_0225569014_p15778153118331"></a><a name="zh-cn_topic_0225569014_p15778153118331"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1778123113337"><a name="zh-cn_topic_0225569014_p1778123113337"></a><a name="zh-cn_topic_0225569014_p1778123113337"></a>版本号，用户输入自定义版本号或者使用默认的当前时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row077853163317"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p8778113183311"><a name="zh-cn_topic_0225569014_p8778113183311"></a><a name="zh-cn_topic_0225569014_p8778113183311"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p8778431183314"><a name="zh-cn_topic_0225569014_p8778431183314"></a><a name="zh-cn_topic_0225569014_p8778431183314"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p197782315338"><a name="zh-cn_topic_0225569014_p197782315338"></a><a name="zh-cn_topic_0225569014_p197782315338"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p177791731183310"><a name="zh-cn_topic_0225569014_p177791731183310"></a><a name="zh-cn_topic_0225569014_p177791731183310"></a>分组描述信息</p>
</td>
</tr>
</tbody>
</table>

**表 5**  paths参数说明

<a name="zh-cn_topic_0225569014_table4779143143311"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row1977953115332"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p07801431173316"><a name="zh-cn_topic_0225569014_p07801431173316"></a><a name="zh-cn_topic_0225569014_p07801431173316"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p4780531143317"><a name="zh-cn_topic_0225569014_p4780531143317"></a><a name="zh-cn_topic_0225569014_p4780531143317"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p978093183319"><a name="zh-cn_topic_0225569014_p978093183319"></a><a name="zh-cn_topic_0225569014_p978093183319"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p17780163110337"><a name="zh-cn_topic_0225569014_p17780163110337"></a><a name="zh-cn_topic_0225569014_p17780163110337"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row1278010312334"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p2078003123313"><a name="zh-cn_topic_0225569014_p2078003123313"></a><a name="zh-cn_topic_0225569014_p2078003123313"></a>uri</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1478019313332"><a name="zh-cn_topic_0225569014_p1478019313332"></a><a name="zh-cn_topic_0225569014_p1478019313332"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p5780153153312"><a name="zh-cn_topic_0225569014_p5780153153312"></a><a name="zh-cn_topic_0225569014_p5780153153312"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1578083193319"><a name="zh-cn_topic_0225569014_p1578083193319"></a><a name="zh-cn_topic_0225569014_p1578083193319"></a>API访问地址，参考<a href="#zh-cn_topic_0225569014_table87808315333">表6</a></p>
</td>
</tr>
</tbody>
</table>

**表 6**  uri参数说明

<a name="zh-cn_topic_0225569014_table87808315333"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row5781163103316"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p1781131163318"><a name="zh-cn_topic_0225569014_p1781131163318"></a><a name="zh-cn_topic_0225569014_p1781131163318"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p77811031173316"><a name="zh-cn_topic_0225569014_p77811031173316"></a><a name="zh-cn_topic_0225569014_p77811031173316"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p11781143193313"><a name="zh-cn_topic_0225569014_p11781143193313"></a><a name="zh-cn_topic_0225569014_p11781143193313"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p778111311338"><a name="zh-cn_topic_0225569014_p778111311338"></a><a name="zh-cn_topic_0225569014_p778111311338"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row167811731183313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p19781203143311"><a name="zh-cn_topic_0225569014_p19781203143311"></a><a name="zh-cn_topic_0225569014_p19781203143311"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p5781831123315"><a name="zh-cn_topic_0225569014_p5781831123315"></a><a name="zh-cn_topic_0225569014_p5781831123315"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p9781133113333"><a name="zh-cn_topic_0225569014_p9781133113333"></a><a name="zh-cn_topic_0225569014_p9781133113333"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1878113112334"><a name="zh-cn_topic_0225569014_p1878113112334"></a><a name="zh-cn_topic_0225569014_p1878113112334"></a>API访问方法，参考<a href="#zh-cn_topic_0225569014_table1178111318331">表7</a></p>
</td>
</tr>
</tbody>
</table>

**表 7**  method参数说明

<a name="zh-cn_topic_0225569014_table1178111318331"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row678213153314"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p178293118331"><a name="zh-cn_topic_0225569014_p178293118331"></a><a name="zh-cn_topic_0225569014_p178293118331"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p107821531103315"><a name="zh-cn_topic_0225569014_p107821531103315"></a><a name="zh-cn_topic_0225569014_p107821531103315"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p7782153120336"><a name="zh-cn_topic_0225569014_p7782153120336"></a><a name="zh-cn_topic_0225569014_p7782153120336"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p87821031153311"><a name="zh-cn_topic_0225569014_p87821031153311"></a><a name="zh-cn_topic_0225569014_p87821031153311"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row12849144802517"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p08503484253"><a name="zh-cn_topic_0225569014_p08503484253"></a><a name="zh-cn_topic_0225569014_p08503484253"></a>operationId</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p0850204842510"><a name="zh-cn_topic_0225569014_p0850204842510"></a><a name="zh-cn_topic_0225569014_p0850204842510"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p085094842516"><a name="zh-cn_topic_0225569014_p085094842516"></a><a name="zh-cn_topic_0225569014_p085094842516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p485094872511"><a name="zh-cn_topic_0225569014_p485094872511"></a><a name="zh-cn_topic_0225569014_p485094872511"></a>API的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row37829315332"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p3783931103316"><a name="zh-cn_topic_0225569014_p3783931103316"></a><a name="zh-cn_topic_0225569014_p3783931103316"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p157839316331"><a name="zh-cn_topic_0225569014_p157839316331"></a><a name="zh-cn_topic_0225569014_p157839316331"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1678373143312"><a name="zh-cn_topic_0225569014_p1678373143312"></a><a name="zh-cn_topic_0225569014_p1678373143312"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1178393114337"><a name="zh-cn_topic_0225569014_p1178393114337"></a><a name="zh-cn_topic_0225569014_p1178393114337"></a>API的描述信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row078320314332"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p2078310314338"><a name="zh-cn_topic_0225569014_p2078310314338"></a><a name="zh-cn_topic_0225569014_p2078310314338"></a>schemes</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p578323193319"><a name="zh-cn_topic_0225569014_p578323193319"></a><a name="zh-cn_topic_0225569014_p578323193319"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p878312318330"><a name="zh-cn_topic_0225569014_p878312318330"></a><a name="zh-cn_topic_0225569014_p878312318330"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p197831317339"><a name="zh-cn_topic_0225569014_p197831317339"></a><a name="zh-cn_topic_0225569014_p197831317339"></a>API的请求协议对象数组定义，支持http、https</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row1968814364917"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1533713935518"><a name="zh-cn_topic_0225569014_p1533713935518"></a><a name="zh-cn_topic_0225569014_p1533713935518"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p2337039165520"><a name="zh-cn_topic_0225569014_p2337039165520"></a><a name="zh-cn_topic_0225569014_p2337039165520"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p7837754145511"><a name="zh-cn_topic_0225569014_p7837754145511"></a><a name="zh-cn_topic_0225569014_p7837754145511"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1337133918551"><a name="zh-cn_topic_0225569014_p1337133918551"></a><a name="zh-cn_topic_0225569014_p1337133918551"></a>API标签对象数组定义</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row07831431123313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p127831531103319"><a name="zh-cn_topic_0225569014_p127831531103319"></a><a name="zh-cn_topic_0225569014_p127831531103319"></a>parameters</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p4783203173316"><a name="zh-cn_topic_0225569014_p4783203173316"></a><a name="zh-cn_topic_0225569014_p4783203173316"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p87831631133312"><a name="zh-cn_topic_0225569014_p87831631133312"></a><a name="zh-cn_topic_0225569014_p87831631133312"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p27833313337"><a name="zh-cn_topic_0225569014_p27833313337"></a><a name="zh-cn_topic_0225569014_p27833313337"></a>请求参数对象数组定义，参考<a href="#zh-cn_topic_0225569014_table87881431123317">表 前端parameters参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row1078313110336"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p177846311333"><a name="zh-cn_topic_0225569014_p177846311333"></a><a name="zh-cn_topic_0225569014_p177846311333"></a>responses</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p8784031193315"><a name="zh-cn_topic_0225569014_p8784031193315"></a><a name="zh-cn_topic_0225569014_p8784031193315"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p2784143113334"><a name="zh-cn_topic_0225569014_p2784143113334"></a><a name="zh-cn_topic_0225569014_p2784143113334"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p11784131123317"><a name="zh-cn_topic_0225569014_p11784131123317"></a><a name="zh-cn_topic_0225569014_p11784131123317"></a>响应定义，参考<a href="#zh-cn_topic_0225569014_table1179216319331">表9</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row6852144810252"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p15852648132516"><a name="zh-cn_topic_0225569014_p15852648132516"></a><a name="zh-cn_topic_0225569014_p15852648132516"></a>security</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p985254812519"><a name="zh-cn_topic_0225569014_p985254812519"></a><a name="zh-cn_topic_0225569014_p985254812519"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p20852948192520"><a name="zh-cn_topic_0225569014_p20852948192520"></a><a name="zh-cn_topic_0225569014_p20852948192520"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1185244832513"><a name="zh-cn_topic_0225569014_p1185244832513"></a><a name="zh-cn_topic_0225569014_p1185244832513"></a>API的认证类型对象数组定义，参考<a href="#zh-cn_topic_0225569014_table986594862513">表 security参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row185314892514"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p8853748182515"><a name="zh-cn_topic_0225569014_p8853748182515"></a><a name="zh-cn_topic_0225569014_p8853748182515"></a>x-apigateway-access-control</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p18853114818258"><a name="zh-cn_topic_0225569014_p18853114818258"></a><a name="zh-cn_topic_0225569014_p18853114818258"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p885316488254"><a name="zh-cn_topic_0225569014_p885316488254"></a><a name="zh-cn_topic_0225569014_p885316488254"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p885318487254"><a name="zh-cn_topic_0225569014_p885318487254"></a><a name="zh-cn_topic_0225569014_p885318487254"></a>API绑定的访问控制对象数组定义</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row11853104814258"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1385324810256"><a name="zh-cn_topic_0225569014_p1385324810256"></a><a name="zh-cn_topic_0225569014_p1385324810256"></a>x-apigateway-backend</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p7853248172514"><a name="zh-cn_topic_0225569014_p7853248172514"></a><a name="zh-cn_topic_0225569014_p7853248172514"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p6853184852511"><a name="zh-cn_topic_0225569014_p6853184852511"></a><a name="zh-cn_topic_0225569014_p6853184852511"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p4853174816257"><a name="zh-cn_topic_0225569014_p4853174816257"></a><a name="zh-cn_topic_0225569014_p4853174816257"></a>API的后端信息，参考<a href="#zh-cn_topic_0225569014_table387619483252">表 x-apigateway-backend参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row1685384815256"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1485334813258"><a name="zh-cn_topic_0225569014_p1485334813258"></a><a name="zh-cn_topic_0225569014_p1485334813258"></a>x-apigateway-backend-policies</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p685464852511"><a name="zh-cn_topic_0225569014_p685464852511"></a><a name="zh-cn_topic_0225569014_p685464852511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p785419483251"><a name="zh-cn_topic_0225569014_p785419483251"></a><a name="zh-cn_topic_0225569014_p785419483251"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p18541148122518"><a name="zh-cn_topic_0225569014_p18541148122518"></a><a name="zh-cn_topic_0225569014_p18541148122518"></a>API的策略后端信息，参考<a href="#zh-cn_topic_0225569014_table1988034862512">表 x-apigateway-backend-policies参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row6854164802518"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1285414488259"><a name="zh-cn_topic_0225569014_p1285414488259"></a><a name="zh-cn_topic_0225569014_p1285414488259"></a>x-apigateway-cors</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p13854104814259"><a name="zh-cn_topic_0225569014_p13854104814259"></a><a name="zh-cn_topic_0225569014_p13854104814259"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p198541648152518"><a name="zh-cn_topic_0225569014_p198541648152518"></a><a name="zh-cn_topic_0225569014_p198541648152518"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1985410480253"><a name="zh-cn_topic_0225569014_p1985410480253"></a><a name="zh-cn_topic_0225569014_p1985410480253"></a>是否支持跨域</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row16854154817253"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p2085454816256"><a name="zh-cn_topic_0225569014_p2085454816256"></a><a name="zh-cn_topic_0225569014_p2085454816256"></a>x-apigateway-match-mode</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p98551248162511"><a name="zh-cn_topic_0225569014_p98551248162511"></a><a name="zh-cn_topic_0225569014_p98551248162511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p14855948102517"><a name="zh-cn_topic_0225569014_p14855948102517"></a><a name="zh-cn_topic_0225569014_p14855948102517"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p18551948122513"><a name="zh-cn_topic_0225569014_p18551948122513"></a><a name="zh-cn_topic_0225569014_p18551948122513"></a>API的匹配方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row11855164832513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1885514480253"><a name="zh-cn_topic_0225569014_p1885514480253"></a><a name="zh-cn_topic_0225569014_p1885514480253"></a>x-apigateway-ratelimit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p5855648142511"><a name="zh-cn_topic_0225569014_p5855648142511"></a><a name="zh-cn_topic_0225569014_p5855648142511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p885504815254"><a name="zh-cn_topic_0225569014_p885504815254"></a><a name="zh-cn_topic_0225569014_p885504815254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p15855124810253"><a name="zh-cn_topic_0225569014_p15855124810253"></a><a name="zh-cn_topic_0225569014_p15855124810253"></a>API绑定的流量控制名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row885554810255"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p5855144872514"><a name="zh-cn_topic_0225569014_p5855144872514"></a><a name="zh-cn_topic_0225569014_p5855144872514"></a>x-apigateway-request-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p4855144822512"><a name="zh-cn_topic_0225569014_p4855144822512"></a><a name="zh-cn_topic_0225569014_p4855144822512"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p108550488256"><a name="zh-cn_topic_0225569014_p108550488256"></a><a name="zh-cn_topic_0225569014_p108550488256"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p28561348162511"><a name="zh-cn_topic_0225569014_p28561348162511"></a><a name="zh-cn_topic_0225569014_p28561348162511"></a>API的类型</p>
</td>
</tr>
</tbody>
</table>

**表 8**  前端parameters参数说明

<a name="zh-cn_topic_0225569014_table87881431123317"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row178813319331"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p1178853117333"><a name="zh-cn_topic_0225569014_p1178853117333"></a><a name="zh-cn_topic_0225569014_p1178853117333"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p178823116333"><a name="zh-cn_topic_0225569014_p178823116333"></a><a name="zh-cn_topic_0225569014_p178823116333"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p27881931113310"><a name="zh-cn_topic_0225569014_p27881931113310"></a><a name="zh-cn_topic_0225569014_p27881931113310"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.45544554455446%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p12788133113333"><a name="zh-cn_topic_0225569014_p12788133113333"></a><a name="zh-cn_topic_0225569014_p12788133113333"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row16788133123313"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p19788331183319"><a name="zh-cn_topic_0225569014_p19788331183319"></a><a name="zh-cn_topic_0225569014_p19788331183319"></a>maximum</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1278823120331"><a name="zh-cn_topic_0225569014_p1278823120331"></a><a name="zh-cn_topic_0225569014_p1278823120331"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1578853103319"><a name="zh-cn_topic_0225569014_p1578853103319"></a><a name="zh-cn_topic_0225569014_p1578853103319"></a>Float</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p20789203117333"><a name="zh-cn_topic_0225569014_p20789203117333"></a><a name="zh-cn_topic_0225569014_p20789203117333"></a>参数为数值类型时，最大参数值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row878903118339"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p14789103114338"><a name="zh-cn_topic_0225569014_p14789103114338"></a><a name="zh-cn_topic_0225569014_p14789103114338"></a>minimum</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p117891531183316"><a name="zh-cn_topic_0225569014_p117891531183316"></a><a name="zh-cn_topic_0225569014_p117891531183316"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1978911312333"><a name="zh-cn_topic_0225569014_p1978911312333"></a><a name="zh-cn_topic_0225569014_p1978911312333"></a>Float</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p57891331193316"><a name="zh-cn_topic_0225569014_p57891331193316"></a><a name="zh-cn_topic_0225569014_p57891331193316"></a>参数为数值类型时，最小参数值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row0789193118332"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p10789163183315"><a name="zh-cn_topic_0225569014_p10789163183315"></a><a name="zh-cn_topic_0225569014_p10789163183315"></a>maxLength</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p117891316330"><a name="zh-cn_topic_0225569014_p117891316330"></a><a name="zh-cn_topic_0225569014_p117891316330"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p17789143117337"><a name="zh-cn_topic_0225569014_p17789143117337"></a><a name="zh-cn_topic_0225569014_p17789143117337"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p187891931143313"><a name="zh-cn_topic_0225569014_p187891931143313"></a><a name="zh-cn_topic_0225569014_p187891931143313"></a>参数为字符串类型时，参数的最大长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row177892031203312"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p37899310336"><a name="zh-cn_topic_0225569014_p37899310336"></a><a name="zh-cn_topic_0225569014_p37899310336"></a>minLength</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p7789131103317"><a name="zh-cn_topic_0225569014_p7789131103317"></a><a name="zh-cn_topic_0225569014_p7789131103317"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1578912315336"><a name="zh-cn_topic_0225569014_p1578912315336"></a><a name="zh-cn_topic_0225569014_p1578912315336"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p15789153115331"><a name="zh-cn_topic_0225569014_p15789153115331"></a><a name="zh-cn_topic_0225569014_p15789153115331"></a>参数为字符串类型时，参数的最小长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row9790143133311"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p979083110332"><a name="zh-cn_topic_0225569014_p979083110332"></a><a name="zh-cn_topic_0225569014_p979083110332"></a>pattern</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p879023110332"><a name="zh-cn_topic_0225569014_p879023110332"></a><a name="zh-cn_topic_0225569014_p879023110332"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p87901316339"><a name="zh-cn_topic_0225569014_p87901316339"></a><a name="zh-cn_topic_0225569014_p87901316339"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p127901319332"><a name="zh-cn_topic_0225569014_p127901319332"></a><a name="zh-cn_topic_0225569014_p127901319332"></a>参数值为正则匹配表达式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row07901831143311"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p379073113311"><a name="zh-cn_topic_0225569014_p379073113311"></a><a name="zh-cn_topic_0225569014_p379073113311"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1790133153313"><a name="zh-cn_topic_0225569014_p1790133153313"></a><a name="zh-cn_topic_0225569014_p1790133153313"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p20790123110339"><a name="zh-cn_topic_0225569014_p20790123110339"></a><a name="zh-cn_topic_0225569014_p20790123110339"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1279013133314"><a name="zh-cn_topic_0225569014_p1279013133314"></a><a name="zh-cn_topic_0225569014_p1279013133314"></a>参数类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row11790331123320"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p379018310339"><a name="zh-cn_topic_0225569014_p379018310339"></a><a name="zh-cn_topic_0225569014_p379018310339"></a>default</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p2790331153310"><a name="zh-cn_topic_0225569014_p2790331153310"></a><a name="zh-cn_topic_0225569014_p2790331153310"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1779003113338"><a name="zh-cn_topic_0225569014_p1779003113338"></a><a name="zh-cn_topic_0225569014_p1779003113338"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p179023118333"><a name="zh-cn_topic_0225569014_p179023118333"></a><a name="zh-cn_topic_0225569014_p179023118333"></a>参数默认值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row18790173123319"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p779073111339"><a name="zh-cn_topic_0225569014_p779073111339"></a><a name="zh-cn_topic_0225569014_p779073111339"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p7791113183311"><a name="zh-cn_topic_0225569014_p7791113183311"></a><a name="zh-cn_topic_0225569014_p7791113183311"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p2791123173315"><a name="zh-cn_topic_0225569014_p2791123173315"></a><a name="zh-cn_topic_0225569014_p2791123173315"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p67911731183313"><a name="zh-cn_topic_0225569014_p67911731183313"></a><a name="zh-cn_topic_0225569014_p67911731183313"></a>参数描述信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row10791231183316"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1479123117331"><a name="zh-cn_topic_0225569014_p1479123117331"></a><a name="zh-cn_topic_0225569014_p1479123117331"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p137911631153311"><a name="zh-cn_topic_0225569014_p137911631153311"></a><a name="zh-cn_topic_0225569014_p137911631153311"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p97911331173318"><a name="zh-cn_topic_0225569014_p97911331173318"></a><a name="zh-cn_topic_0225569014_p97911331173318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p979112312330"><a name="zh-cn_topic_0225569014_p979112312330"></a><a name="zh-cn_topic_0225569014_p979112312330"></a>参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row1779173173314"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1579153110335"><a name="zh-cn_topic_0225569014_p1579153110335"></a><a name="zh-cn_topic_0225569014_p1579153110335"></a>in</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p97914312337"><a name="zh-cn_topic_0225569014_p97914312337"></a><a name="zh-cn_topic_0225569014_p97914312337"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p12791173114338"><a name="zh-cn_topic_0225569014_p12791173114338"></a><a name="zh-cn_topic_0225569014_p12791173114338"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p20791331103320"><a name="zh-cn_topic_0225569014_p20791331103320"></a><a name="zh-cn_topic_0225569014_p20791331103320"></a>参数位置，支持path、header、query、formData、body</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row9791113163312"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p177922031143318"><a name="zh-cn_topic_0225569014_p177922031143318"></a><a name="zh-cn_topic_0225569014_p177922031143318"></a>required</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p9792831153314"><a name="zh-cn_topic_0225569014_p9792831153314"></a><a name="zh-cn_topic_0225569014_p9792831153314"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p679293111333"><a name="zh-cn_topic_0225569014_p679293111333"></a><a name="zh-cn_topic_0225569014_p679293111333"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1792173123313"><a name="zh-cn_topic_0225569014_p1792173123313"></a><a name="zh-cn_topic_0225569014_p1792173123313"></a>参数是否必需，参数位置为path时必需</p>
</td>
</tr>
</tbody>
</table>

**表 9**  responses参数说明

<a name="zh-cn_topic_0225569014_table1179216319331"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row8792731153315"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p1779373116337"><a name="zh-cn_topic_0225569014_p1779373116337"></a><a name="zh-cn_topic_0225569014_p1779373116337"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p16793123114337"><a name="zh-cn_topic_0225569014_p16793123114337"></a><a name="zh-cn_topic_0225569014_p16793123114337"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p979313111338"><a name="zh-cn_topic_0225569014_p979313111338"></a><a name="zh-cn_topic_0225569014_p979313111338"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p157931310332"><a name="zh-cn_topic_0225569014_p157931310332"></a><a name="zh-cn_topic_0225569014_p157931310332"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row079333183320"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p167931931183315"><a name="zh-cn_topic_0225569014_p167931931183315"></a><a name="zh-cn_topic_0225569014_p167931931183315"></a>default</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p67931731123311"><a name="zh-cn_topic_0225569014_p67931731123311"></a><a name="zh-cn_topic_0225569014_p67931731123311"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p779311315332"><a name="zh-cn_topic_0225569014_p779311315332"></a><a name="zh-cn_topic_0225569014_p779311315332"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1079363115336"><a name="zh-cn_topic_0225569014_p1079363115336"></a><a name="zh-cn_topic_0225569014_p1079363115336"></a>缺省响应，描述未定义的响应码</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row1779315314339"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p77931031143318"><a name="zh-cn_topic_0225569014_p77931031143318"></a><a name="zh-cn_topic_0225569014_p77931031143318"></a>status_code</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p079412319339"><a name="zh-cn_topic_0225569014_p079412319339"></a><a name="zh-cn_topic_0225569014_p079412319339"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p137941731133315"><a name="zh-cn_topic_0225569014_p137941731133315"></a><a name="zh-cn_topic_0225569014_p137941731133315"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p0794331153315"><a name="zh-cn_topic_0225569014_p0794331153315"></a><a name="zh-cn_topic_0225569014_p0794331153315"></a>响应状态码，值为响应对象，参考<a href="#zh-cn_topic_0225569014_table107974312335">表11</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row1774720508918"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p774812501894"><a name="zh-cn_topic_0225569014_p774812501894"></a><a name="zh-cn_topic_0225569014_p774812501894"></a>x-apigateway-result-failure-sample</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p474815020916"><a name="zh-cn_topic_0225569014_p474815020916"></a><a name="zh-cn_topic_0225569014_p474815020916"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p11749105017914"><a name="zh-cn_topic_0225569014_p11749105017914"></a><a name="zh-cn_topic_0225569014_p11749105017914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p14749750398"><a name="zh-cn_topic_0225569014_p14749750398"></a><a name="zh-cn_topic_0225569014_p14749750398"></a>失败返回示例，描述API的异常返回信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row71795541897"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1117913541917"><a name="zh-cn_topic_0225569014_p1117913541917"></a><a name="zh-cn_topic_0225569014_p1117913541917"></a>x-apigateway-result-normal-sample</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p517914541191"><a name="zh-cn_topic_0225569014_p517914541191"></a><a name="zh-cn_topic_0225569014_p517914541191"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p171791554493"><a name="zh-cn_topic_0225569014_p171791554493"></a><a name="zh-cn_topic_0225569014_p171791554493"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p111791154598"><a name="zh-cn_topic_0225569014_p111791154598"></a><a name="zh-cn_topic_0225569014_p111791154598"></a>正常响应示例，描述API的正常返回信息</p>
</td>
</tr>
</tbody>
</table>

**表 10**  security参数说明

<a name="zh-cn_topic_0225569014_table986594862513"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row086674852515"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p986654810257"><a name="zh-cn_topic_0225569014_p986654810257"></a><a name="zh-cn_topic_0225569014_p986654810257"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p986624819250"><a name="zh-cn_topic_0225569014_p986624819250"></a><a name="zh-cn_topic_0225569014_p986624819250"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p188661348112516"><a name="zh-cn_topic_0225569014_p188661348112516"></a><a name="zh-cn_topic_0225569014_p188661348112516"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.45544554455446%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p14866248132510"><a name="zh-cn_topic_0225569014_p14866248132510"></a><a name="zh-cn_topic_0225569014_p14866248132510"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row17866114810256"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p696102820583"><a name="zh-cn_topic_0225569014_p696102820583"></a><a name="zh-cn_topic_0225569014_p696102820583"></a>apig-auth-type</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p7961172855819"><a name="zh-cn_topic_0225569014_p7961172855819"></a><a name="zh-cn_topic_0225569014_p7961172855819"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1996117280588"><a name="zh-cn_topic_0225569014_p1996117280588"></a><a name="zh-cn_topic_0225569014_p1996117280588"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p696252813588"><a name="zh-cn_topic_0225569014_p696252813588"></a><a name="zh-cn_topic_0225569014_p696252813588"></a>API的认证类型对象数组定义，为空数组</p>
<p id="zh-cn_topic_0225569014_p6722101419557"><a name="zh-cn_topic_0225569014_p6722101419557"></a><a name="zh-cn_topic_0225569014_p6722101419557"></a>apig-auth-type支持：</p>
<a name="zh-cn_topic_0225569014_ul3401225145518"></a><a name="zh-cn_topic_0225569014_ul3401225145518"></a><ul id="zh-cn_topic_0225569014_ul3401225145518"><li>APP认证： apig-auth-app</li><li>IAM认证：apig-auth-iam</li><li>NONE：不填写</li></ul>
</td>
</tr>
</tbody>
</table>

**表 11**  status code参数说明

<a name="zh-cn_topic_0225569014_table107974312335"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row1798831113311"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p11798193120338"><a name="zh-cn_topic_0225569014_p11798193120338"></a><a name="zh-cn_topic_0225569014_p11798193120338"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p19798163113335"><a name="zh-cn_topic_0225569014_p19798163113335"></a><a name="zh-cn_topic_0225569014_p19798163113335"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p479813115331"><a name="zh-cn_topic_0225569014_p479813115331"></a><a name="zh-cn_topic_0225569014_p479813115331"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p18798183116337"><a name="zh-cn_topic_0225569014_p18798183116337"></a><a name="zh-cn_topic_0225569014_p18798183116337"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row67981311335"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p17798173103315"><a name="zh-cn_topic_0225569014_p17798173103315"></a><a name="zh-cn_topic_0225569014_p17798173103315"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p137981131183317"><a name="zh-cn_topic_0225569014_p137981131183317"></a><a name="zh-cn_topic_0225569014_p137981131183317"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p17798431113320"><a name="zh-cn_topic_0225569014_p17798431113320"></a><a name="zh-cn_topic_0225569014_p17798431113320"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1379983114336"><a name="zh-cn_topic_0225569014_p1379983114336"></a><a name="zh-cn_topic_0225569014_p1379983114336"></a>响应描述信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row979933133313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p20799143193310"><a name="zh-cn_topic_0225569014_p20799143193310"></a><a name="zh-cn_topic_0225569014_p20799143193310"></a>schema</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1179953153314"><a name="zh-cn_topic_0225569014_p1179953153314"></a><a name="zh-cn_topic_0225569014_p1179953153314"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p6799113103314"><a name="zh-cn_topic_0225569014_p6799113103314"></a><a name="zh-cn_topic_0225569014_p6799113103314"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p27991431193317"><a name="zh-cn_topic_0225569014_p27991431193317"></a><a name="zh-cn_topic_0225569014_p27991431193317"></a>响应正文定义，参考<a href="#zh-cn_topic_0225569014_table47999312330">表12</a></p>
</td>
</tr>
</tbody>
</table>

**表 12**  schema参数说明

<a name="zh-cn_topic_0225569014_table47999312330"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row5800143114331"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p1280083113332"><a name="zh-cn_topic_0225569014_p1280083113332"></a><a name="zh-cn_topic_0225569014_p1280083113332"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p148001231173318"><a name="zh-cn_topic_0225569014_p148001231173318"></a><a name="zh-cn_topic_0225569014_p148001231173318"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p18800123153320"><a name="zh-cn_topic_0225569014_p18800123153320"></a><a name="zh-cn_topic_0225569014_p18800123153320"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p13800113113310"><a name="zh-cn_topic_0225569014_p13800113113310"></a><a name="zh-cn_topic_0225569014_p13800113113310"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row18800173163318"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p158009313336"><a name="zh-cn_topic_0225569014_p158009313336"></a><a name="zh-cn_topic_0225569014_p158009313336"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p980016317332"><a name="zh-cn_topic_0225569014_p980016317332"></a><a name="zh-cn_topic_0225569014_p980016317332"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1800531193312"><a name="zh-cn_topic_0225569014_p1800531193312"></a><a name="zh-cn_topic_0225569014_p1800531193312"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p2800331193316"><a name="zh-cn_topic_0225569014_p2800331193316"></a><a name="zh-cn_topic_0225569014_p2800331193316"></a>BODY体描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row19800131173318"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p18800133173314"><a name="zh-cn_topic_0225569014_p18800133173314"></a><a name="zh-cn_topic_0225569014_p18800133173314"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p11800163153314"><a name="zh-cn_topic_0225569014_p11800163153314"></a><a name="zh-cn_topic_0225569014_p11800163153314"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p8801133113311"><a name="zh-cn_topic_0225569014_p8801133113311"></a><a name="zh-cn_topic_0225569014_p8801133113311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p980119311336"><a name="zh-cn_topic_0225569014_p980119311336"></a><a name="zh-cn_topic_0225569014_p980119311336"></a>BODY体类型：FORM/STREAM（表单/字节流）</p>
</td>
</tr>
</tbody>
</table>

**表 13**  securityDefinitions参数说明

<a name="zh-cn_topic_0225569014_table8801831163318"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row14801193113339"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p58010316337"><a name="zh-cn_topic_0225569014_p58010316337"></a><a name="zh-cn_topic_0225569014_p58010316337"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13.861386138613863%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p12801123110331"><a name="zh-cn_topic_0225569014_p12801123110331"></a><a name="zh-cn_topic_0225569014_p12801123110331"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p5801133113331"><a name="zh-cn_topic_0225569014_p5801133113331"></a><a name="zh-cn_topic_0225569014_p5801133113331"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.46534653465347%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p20801431193316"><a name="zh-cn_topic_0225569014_p20801431193316"></a><a name="zh-cn_topic_0225569014_p20801431193316"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row188011831183315"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p88012031193317"><a name="zh-cn_topic_0225569014_p88012031193317"></a><a name="zh-cn_topic_0225569014_p88012031193317"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p280153111337"><a name="zh-cn_topic_0225569014_p280153111337"></a><a name="zh-cn_topic_0225569014_p280153111337"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1380133119339"><a name="zh-cn_topic_0225569014_p1380133119339"></a><a name="zh-cn_topic_0225569014_p1380133119339"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="53.46534653465347%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p080211318331"><a name="zh-cn_topic_0225569014_p080211318331"></a><a name="zh-cn_topic_0225569014_p080211318331"></a>自定义鉴权方式名称，参考<a href="#zh-cn_topic_0225569014_table12802183116332">表14</a></p>
</td>
</tr>
</tbody>
</table>

**表 14**  name参数说明

<a name="zh-cn_topic_0225569014_table12802183116332"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row580253113313"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p13802331103315"><a name="zh-cn_topic_0225569014_p13802331103315"></a><a name="zh-cn_topic_0225569014_p13802331103315"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p1802133118337"><a name="zh-cn_topic_0225569014_p1802133118337"></a><a name="zh-cn_topic_0225569014_p1802133118337"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p2080263113332"><a name="zh-cn_topic_0225569014_p2080263113332"></a><a name="zh-cn_topic_0225569014_p2080263113332"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p1580263113332"><a name="zh-cn_topic_0225569014_p1580263113332"></a><a name="zh-cn_topic_0225569014_p1580263113332"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row13802193114334"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p18802133120331"><a name="zh-cn_topic_0225569014_p18802133120331"></a><a name="zh-cn_topic_0225569014_p18802133120331"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1802203115333"><a name="zh-cn_topic_0225569014_p1802203115333"></a><a name="zh-cn_topic_0225569014_p1802203115333"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1580263113333"><a name="zh-cn_topic_0225569014_p1580263113333"></a><a name="zh-cn_topic_0225569014_p1580263113333"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p128031531183313"><a name="zh-cn_topic_0225569014_p128031531183313"></a><a name="zh-cn_topic_0225569014_p128031531183313"></a>鉴权类型，支持apiKey</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row2080393143310"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1880373133318"><a name="zh-cn_topic_0225569014_p1880373133318"></a><a name="zh-cn_topic_0225569014_p1880373133318"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p18031331183311"><a name="zh-cn_topic_0225569014_p18031331183311"></a><a name="zh-cn_topic_0225569014_p18031331183311"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p8803123193312"><a name="zh-cn_topic_0225569014_p8803123193312"></a><a name="zh-cn_topic_0225569014_p8803123193312"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p9803143113331"><a name="zh-cn_topic_0225569014_p9803143113331"></a><a name="zh-cn_topic_0225569014_p9803143113331"></a>apiKey参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row5803731203310"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1380333114333"><a name="zh-cn_topic_0225569014_p1380333114333"></a><a name="zh-cn_topic_0225569014_p1380333114333"></a>in</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p5803631143310"><a name="zh-cn_topic_0225569014_p5803631143310"></a><a name="zh-cn_topic_0225569014_p5803631143310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p4803103117336"><a name="zh-cn_topic_0225569014_p4803103117336"></a><a name="zh-cn_topic_0225569014_p4803103117336"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p108031731183316"><a name="zh-cn_topic_0225569014_p108031731183316"></a><a name="zh-cn_topic_0225569014_p108031731183316"></a>apiKey参数位置</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row118031231163320"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p14803183117335"><a name="zh-cn_topic_0225569014_p14803183117335"></a><a name="zh-cn_topic_0225569014_p14803183117335"></a>x-apigateway-auth-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p48031531153311"><a name="zh-cn_topic_0225569014_p48031531153311"></a><a name="zh-cn_topic_0225569014_p48031531153311"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p2080313173313"><a name="zh-cn_topic_0225569014_p2080313173313"></a><a name="zh-cn_topic_0225569014_p2080313173313"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p10804193119337"><a name="zh-cn_topic_0225569014_p10804193119337"></a><a name="zh-cn_topic_0225569014_p10804193119337"></a>扩展鉴权类型，基于apiKey鉴权方式的扩展，网关自定义的鉴权方式，支持AppSigv1、IAM、IAM_NONE</p>
</td>
</tr>
</tbody>
</table>

**表 15**  x-apigateway-backend参数说明

<a name="zh-cn_topic_0225569014_table387619483252"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row1487734812520"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p487734814254"><a name="zh-cn_topic_0225569014_p487734814254"></a><a name="zh-cn_topic_0225569014_p487734814254"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p58771548122516"><a name="zh-cn_topic_0225569014_p58771548122516"></a><a name="zh-cn_topic_0225569014_p58771548122516"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p287774812511"><a name="zh-cn_topic_0225569014_p287774812511"></a><a name="zh-cn_topic_0225569014_p287774812511"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p13877134815251"><a name="zh-cn_topic_0225569014_p13877134815251"></a><a name="zh-cn_topic_0225569014_p13877134815251"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row10877114822512"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p2878144892516"><a name="zh-cn_topic_0225569014_p2878144892516"></a><a name="zh-cn_topic_0225569014_p2878144892516"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p15878648182515"><a name="zh-cn_topic_0225569014_p15878648182515"></a><a name="zh-cn_topic_0225569014_p15878648182515"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p587811480258"><a name="zh-cn_topic_0225569014_p587811480258"></a><a name="zh-cn_topic_0225569014_p587811480258"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p2878134802519"><a name="zh-cn_topic_0225569014_p2878134802519"></a><a name="zh-cn_topic_0225569014_p2878134802519"></a>API后端类型，支持HTTP、HTTP-VPC、FUNCTION、MOCK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row8878174811255"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p187864862516"><a name="zh-cn_topic_0225569014_p187864862516"></a><a name="zh-cn_topic_0225569014_p187864862516"></a>parameters</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p387834820252"><a name="zh-cn_topic_0225569014_p387834820252"></a><a name="zh-cn_topic_0225569014_p387834820252"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p0878848142512"><a name="zh-cn_topic_0225569014_p0878848142512"></a><a name="zh-cn_topic_0225569014_p0878848142512"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1887854802516"><a name="zh-cn_topic_0225569014_p1887854802516"></a><a name="zh-cn_topic_0225569014_p1887854802516"></a>后端参数对象数组定义，参考<a href="#zh-cn_topic_0225569014_table14884114882511">表 后端parameters参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row1387834892518"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1587934817256"><a name="zh-cn_topic_0225569014_p1587934817256"></a><a name="zh-cn_topic_0225569014_p1587934817256"></a>backend_define</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p587924822511"><a name="zh-cn_topic_0225569014_p587924822511"></a><a name="zh-cn_topic_0225569014_p587924822511"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p20879124802513"><a name="zh-cn_topic_0225569014_p20879124802513"></a><a name="zh-cn_topic_0225569014_p20879124802513"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p19879134862517"><a name="zh-cn_topic_0225569014_p19879134862517"></a><a name="zh-cn_topic_0225569014_p19879134862517"></a>API后端定义</p>
<p id="zh-cn_topic_0225569014_p9879144815251"><a name="zh-cn_topic_0225569014_p9879144815251"></a><a name="zh-cn_topic_0225569014_p9879144815251"></a>backend_define支持：</p>
<a name="zh-cn_topic_0225569014_ul587916489258"></a><a name="zh-cn_topic_0225569014_ul587916489258"></a><ul id="zh-cn_topic_0225569014_ul587916489258"><li>httpEndpoints，参考<a href="#zh-cn_topic_0225569014_table1788894822518">表 后端httpEndpoints参数说明</a></li><li>httpVpcEndpoints，参考<a href="#zh-cn_topic_0225569014_table1089314812254">表 后端httpVpcEndpoints参数说明</a></li><li>functionEndpoints，参考<a href="#zh-cn_topic_0225569014_table18971648202512">表 后端functionEndpoints参数说明</a></li><li>mockEndpoints，参考<a href="#zh-cn_topic_0225569014_table1790184862513">表 后端mockEndpoints参数说明</a></li></ul>
</td>
</tr>
</tbody>
</table>

**表 16**  x-apigateway-backend-policies参数说明

<a name="zh-cn_topic_0225569014_table1988034862512"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row788004814256"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p148801248112517"><a name="zh-cn_topic_0225569014_p148801248112517"></a><a name="zh-cn_topic_0225569014_p148801248112517"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p28801048112514"><a name="zh-cn_topic_0225569014_p28801048112514"></a><a name="zh-cn_topic_0225569014_p28801048112514"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p5880164872513"><a name="zh-cn_topic_0225569014_p5880164872513"></a><a name="zh-cn_topic_0225569014_p5880164872513"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p8881948132519"><a name="zh-cn_topic_0225569014_p8881948132519"></a><a name="zh-cn_topic_0225569014_p8881948132519"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row118811748112520"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p688117485256"><a name="zh-cn_topic_0225569014_p688117485256"></a><a name="zh-cn_topic_0225569014_p688117485256"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p688164822510"><a name="zh-cn_topic_0225569014_p688164822510"></a><a name="zh-cn_topic_0225569014_p688164822510"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p178819481257"><a name="zh-cn_topic_0225569014_p178819481257"></a><a name="zh-cn_topic_0225569014_p178819481257"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p13881448102510"><a name="zh-cn_topic_0225569014_p13881448102510"></a><a name="zh-cn_topic_0225569014_p13881448102510"></a>API后端类型，支持HTTP、HTTP-VPC、FUNCTION、MOCK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row9881134862515"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p19881204822515"><a name="zh-cn_topic_0225569014_p19881204822515"></a><a name="zh-cn_topic_0225569014_p19881204822515"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1888114862515"><a name="zh-cn_topic_0225569014_p1888114862515"></a><a name="zh-cn_topic_0225569014_p1888114862515"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p78817484250"><a name="zh-cn_topic_0225569014_p78817484250"></a><a name="zh-cn_topic_0225569014_p78817484250"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1588144814252"><a name="zh-cn_topic_0225569014_p1588144814252"></a><a name="zh-cn_topic_0225569014_p1588144814252"></a>后端策略名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row588184817258"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p2882124882517"><a name="zh-cn_topic_0225569014_p2882124882517"></a><a name="zh-cn_topic_0225569014_p2882124882517"></a>parameters</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p988244811251"><a name="zh-cn_topic_0225569014_p988244811251"></a><a name="zh-cn_topic_0225569014_p988244811251"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p5882248152519"><a name="zh-cn_topic_0225569014_p5882248152519"></a><a name="zh-cn_topic_0225569014_p5882248152519"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p188218488257"><a name="zh-cn_topic_0225569014_p188218488257"></a><a name="zh-cn_topic_0225569014_p188218488257"></a>后端参数对象数组定义，参考<a href="#zh-cn_topic_0225569014_table14884114882511">表 后端parameters参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row1188204822510"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p19882184892513"><a name="zh-cn_topic_0225569014_p19882184892513"></a><a name="zh-cn_topic_0225569014_p19882184892513"></a>backend_define</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p6882104862512"><a name="zh-cn_topic_0225569014_p6882104862512"></a><a name="zh-cn_topic_0225569014_p6882104862512"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p138821548172512"><a name="zh-cn_topic_0225569014_p138821548172512"></a><a name="zh-cn_topic_0225569014_p138821548172512"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p15882164816258"><a name="zh-cn_topic_0225569014_p15882164816258"></a><a name="zh-cn_topic_0225569014_p15882164816258"></a>API后端定义</p>
<p id="zh-cn_topic_0225569014_p188214481259"><a name="zh-cn_topic_0225569014_p188214481259"></a><a name="zh-cn_topic_0225569014_p188214481259"></a>backend_define支持：</p>
<a name="zh-cn_topic_0225569014_ul0883104814256"></a><a name="zh-cn_topic_0225569014_ul0883104814256"></a><ul id="zh-cn_topic_0225569014_ul0883104814256"><li>httpEndpoints，参考<a href="#zh-cn_topic_0225569014_table1788894822518">表 后端httpEndpoints参数说明</a></li><li>httpVpcEndpoints，参考<a href="#zh-cn_topic_0225569014_table1089314812254">表 后端httpVpcEndpoints参数说明</a></li><li>functionEndpoints，参考<a href="#zh-cn_topic_0225569014_table18971648202512">表 后端functionEndpoints参数说明</a></li><li>mockEndpoints，参考<a href="#zh-cn_topic_0225569014_table1790184862513">表 后端mockEndpoints参数说明</a></li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row48838483257"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p18883948172520"><a name="zh-cn_topic_0225569014_p18883948172520"></a><a name="zh-cn_topic_0225569014_p18883948172520"></a>conditions</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p6883184852518"><a name="zh-cn_topic_0225569014_p6883184852518"></a><a name="zh-cn_topic_0225569014_p6883184852518"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p68846483259"><a name="zh-cn_topic_0225569014_p68846483259"></a><a name="zh-cn_topic_0225569014_p68846483259"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p988404813253"><a name="zh-cn_topic_0225569014_p988404813253"></a><a name="zh-cn_topic_0225569014_p988404813253"></a>策略条件对象数组定义，参考<a href="#zh-cn_topic_0225569014_table1790444832520">表 conditions参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row8601019134513"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p7826184743414"><a name="zh-cn_topic_0225569014_p7826184743414"></a><a name="zh-cn_topic_0225569014_p7826184743414"></a>effectMode</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p15826134712343"><a name="zh-cn_topic_0225569014_p15826134712343"></a><a name="zh-cn_topic_0225569014_p15826134712343"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p58262047113410"><a name="zh-cn_topic_0225569014_p58262047113410"></a><a name="zh-cn_topic_0225569014_p58262047113410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p17355191291320"><a name="zh-cn_topic_0225569014_p17355191291320"></a><a name="zh-cn_topic_0225569014_p17355191291320"></a>关联的策略组合模式，支持ANY、ALL</p>
</td>
</tr>
</tbody>
</table>

**表 17**  后端parameters参数说明

<a name="zh-cn_topic_0225569014_table14884114882511"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row1088574822512"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p88856489251"><a name="zh-cn_topic_0225569014_p88856489251"></a><a name="zh-cn_topic_0225569014_p88856489251"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p18885048132510"><a name="zh-cn_topic_0225569014_p18885048132510"></a><a name="zh-cn_topic_0225569014_p18885048132510"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p19885124810250"><a name="zh-cn_topic_0225569014_p19885124810250"></a><a name="zh-cn_topic_0225569014_p19885124810250"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p188851448172515"><a name="zh-cn_topic_0225569014_p188851448172515"></a><a name="zh-cn_topic_0225569014_p188851448172515"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row138861748112511"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p788674832520"><a name="zh-cn_topic_0225569014_p788674832520"></a><a name="zh-cn_topic_0225569014_p788674832520"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p148868484256"><a name="zh-cn_topic_0225569014_p148868484256"></a><a name="zh-cn_topic_0225569014_p148868484256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1688664812515"><a name="zh-cn_topic_0225569014_p1688664812515"></a><a name="zh-cn_topic_0225569014_p1688664812515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p14886948102519"><a name="zh-cn_topic_0225569014_p14886948102519"></a><a name="zh-cn_topic_0225569014_p14886948102519"></a>参数名称，由字母、数字、下划线、连线、点组成，以字母开头，最长32字节</p>
<p id="zh-cn_topic_0225569014_p1988624813251"><a name="zh-cn_topic_0225569014_p1988624813251"></a><a name="zh-cn_topic_0225569014_p1988624813251"></a>header位置的参数名称不区分大小写</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row388674862513"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1888620480254"><a name="zh-cn_topic_0225569014_p1888620480254"></a><a name="zh-cn_topic_0225569014_p1888620480254"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p98861548152515"><a name="zh-cn_topic_0225569014_p98861548152515"></a><a name="zh-cn_topic_0225569014_p98861548152515"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p0886174810255"><a name="zh-cn_topic_0225569014_p0886174810255"></a><a name="zh-cn_topic_0225569014_p0886174810255"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p19886748182513"><a name="zh-cn_topic_0225569014_p19886748182513"></a><a name="zh-cn_topic_0225569014_p19886748182513"></a>参数值，当参数来源为REQUEST时，值为请求参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row10886148132513"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p13887134822517"><a name="zh-cn_topic_0225569014_p13887134822517"></a><a name="zh-cn_topic_0225569014_p13887134822517"></a>in</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1788764862518"><a name="zh-cn_topic_0225569014_p1788764862518"></a><a name="zh-cn_topic_0225569014_p1788764862518"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p18887164815251"><a name="zh-cn_topic_0225569014_p18887164815251"></a><a name="zh-cn_topic_0225569014_p18887164815251"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p8887174812258"><a name="zh-cn_topic_0225569014_p8887174812258"></a><a name="zh-cn_topic_0225569014_p8887174812258"></a>参数位置，支持header、query、path</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row788711486259"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p4887148182510"><a name="zh-cn_topic_0225569014_p4887148182510"></a><a name="zh-cn_topic_0225569014_p4887148182510"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1588714814252"><a name="zh-cn_topic_0225569014_p1588714814252"></a><a name="zh-cn_topic_0225569014_p1588714814252"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p14887144815254"><a name="zh-cn_topic_0225569014_p14887144815254"></a><a name="zh-cn_topic_0225569014_p14887144815254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p9887104882515"><a name="zh-cn_topic_0225569014_p9887104882515"></a><a name="zh-cn_topic_0225569014_p9887104882515"></a>参数映射来源，支持REQUEST、CONSTANT</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row10888204816254"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1988894882514"><a name="zh-cn_topic_0225569014_p1988894882514"></a><a name="zh-cn_topic_0225569014_p1988894882514"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1788864811250"><a name="zh-cn_topic_0225569014_p1788864811250"></a><a name="zh-cn_topic_0225569014_p1788864811250"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1288854812255"><a name="zh-cn_topic_0225569014_p1288854812255"></a><a name="zh-cn_topic_0225569014_p1288854812255"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p17888184822511"><a name="zh-cn_topic_0225569014_p17888184822511"></a><a name="zh-cn_topic_0225569014_p17888184822511"></a>参数含义描述</p>
</td>
</tr>
</tbody>
</table>

**表 18**  后端httpEndpoints参数说明

<a name="zh-cn_topic_0225569014_table1788894822518"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row988984817253"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p18892048172520"><a name="zh-cn_topic_0225569014_p18892048172520"></a><a name="zh-cn_topic_0225569014_p18892048172520"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p12889204812514"><a name="zh-cn_topic_0225569014_p12889204812514"></a><a name="zh-cn_topic_0225569014_p12889204812514"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p168897485253"><a name="zh-cn_topic_0225569014_p168897485253"></a><a name="zh-cn_topic_0225569014_p168897485253"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p4889144818251"><a name="zh-cn_topic_0225569014_p4889144818251"></a><a name="zh-cn_topic_0225569014_p4889144818251"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row7889164818257"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p158899481251"><a name="zh-cn_topic_0225569014_p158899481251"></a><a name="zh-cn_topic_0225569014_p158899481251"></a>address</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p19889134812514"><a name="zh-cn_topic_0225569014_p19889134812514"></a><a name="zh-cn_topic_0225569014_p19889134812514"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p289054818257"><a name="zh-cn_topic_0225569014_p289054818257"></a><a name="zh-cn_topic_0225569014_p289054818257"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p389044816256"><a name="zh-cn_topic_0225569014_p389044816256"></a><a name="zh-cn_topic_0225569014_p389044816256"></a>后端服务地址，格式为：&lt;域名或IP&gt;:[port]</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row13890348152517"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p48902486252"><a name="zh-cn_topic_0225569014_p48902486252"></a><a name="zh-cn_topic_0225569014_p48902486252"></a>scheme</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p198901048142519"><a name="zh-cn_topic_0225569014_p198901048142519"></a><a name="zh-cn_topic_0225569014_p198901048142519"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p188901488253"><a name="zh-cn_topic_0225569014_p188901488253"></a><a name="zh-cn_topic_0225569014_p188901488253"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p689013488253"><a name="zh-cn_topic_0225569014_p689013488253"></a><a name="zh-cn_topic_0225569014_p689013488253"></a>后端请求协议定义，支持http、https</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row88902048112520"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p13890134816252"><a name="zh-cn_topic_0225569014_p13890134816252"></a><a name="zh-cn_topic_0225569014_p13890134816252"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1089013489252"><a name="zh-cn_topic_0225569014_p1089013489252"></a><a name="zh-cn_topic_0225569014_p1089013489252"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p118901148172513"><a name="zh-cn_topic_0225569014_p118901148172513"></a><a name="zh-cn_topic_0225569014_p118901148172513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1989074812515"><a name="zh-cn_topic_0225569014_p1989074812515"></a><a name="zh-cn_topic_0225569014_p1989074812515"></a>后端请求方法，支持GET、POST、PUT、DELETE、HEAD、OPTIONS、PATCH、ANY</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row7890104822514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p5890144882519"><a name="zh-cn_topic_0225569014_p5890144882519"></a><a name="zh-cn_topic_0225569014_p5890144882519"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p28911948182519"><a name="zh-cn_topic_0225569014_p28911948182519"></a><a name="zh-cn_topic_0225569014_p28911948182519"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p68915482252"><a name="zh-cn_topic_0225569014_p68915482252"></a><a name="zh-cn_topic_0225569014_p68915482252"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p188912048192510"><a name="zh-cn_topic_0225569014_p188912048192510"></a><a name="zh-cn_topic_0225569014_p188912048192510"></a>后端请求路径，支持路径变量</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row13891204812255"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p58911948132514"><a name="zh-cn_topic_0225569014_p58911948132514"></a><a name="zh-cn_topic_0225569014_p58911948132514"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1389194814256"><a name="zh-cn_topic_0225569014_p1389194814256"></a><a name="zh-cn_topic_0225569014_p1389194814256"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p889124812510"><a name="zh-cn_topic_0225569014_p889124812510"></a><a name="zh-cn_topic_0225569014_p889124812510"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p189264813251"><a name="zh-cn_topic_0225569014_p189264813251"></a><a name="zh-cn_topic_0225569014_p189264813251"></a>后端请求超时时间，单位毫秒，缺省值为5000，取值范围为1 ~ 60000</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row7635433104612"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p191691539173611"><a name="zh-cn_topic_0225569014_p191691539173611"></a><a name="zh-cn_topic_0225569014_p191691539173611"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p916993963610"><a name="zh-cn_topic_0225569014_p916993963610"></a><a name="zh-cn_topic_0225569014_p916993963610"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p317073923616"><a name="zh-cn_topic_0225569014_p317073923616"></a><a name="zh-cn_topic_0225569014_p317073923616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p5170539163616"><a name="zh-cn_topic_0225569014_p5170539163616"></a><a name="zh-cn_topic_0225569014_p5170539163616"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 19**  后端httpVpcEndpoints参数说明

<a name="zh-cn_topic_0225569014_table1089314812254"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row489354813256"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p16893104820253"><a name="zh-cn_topic_0225569014_p16893104820253"></a><a name="zh-cn_topic_0225569014_p16893104820253"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p14893548102518"><a name="zh-cn_topic_0225569014_p14893548102518"></a><a name="zh-cn_topic_0225569014_p14893548102518"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p7893184852520"><a name="zh-cn_topic_0225569014_p7893184852520"></a><a name="zh-cn_topic_0225569014_p7893184852520"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p1789304832517"><a name="zh-cn_topic_0225569014_p1789304832517"></a><a name="zh-cn_topic_0225569014_p1789304832517"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row389304819258"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p089494814258"><a name="zh-cn_topic_0225569014_p089494814258"></a><a name="zh-cn_topic_0225569014_p089494814258"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p188941948112519"><a name="zh-cn_topic_0225569014_p188941948112519"></a><a name="zh-cn_topic_0225569014_p188941948112519"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p2089418484250"><a name="zh-cn_topic_0225569014_p2089418484250"></a><a name="zh-cn_topic_0225569014_p2089418484250"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p78948486252"><a name="zh-cn_topic_0225569014_p78948486252"></a><a name="zh-cn_topic_0225569014_p78948486252"></a>VPC通道名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row19894104862518"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1089464852513"><a name="zh-cn_topic_0225569014_p1089464852513"></a><a name="zh-cn_topic_0225569014_p1089464852513"></a>scheme</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p138945480256"><a name="zh-cn_topic_0225569014_p138945480256"></a><a name="zh-cn_topic_0225569014_p138945480256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p989454862516"><a name="zh-cn_topic_0225569014_p989454862516"></a><a name="zh-cn_topic_0225569014_p989454862516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p2894248162512"><a name="zh-cn_topic_0225569014_p2894248162512"></a><a name="zh-cn_topic_0225569014_p2894248162512"></a>后端请求协议定义，支持http、https</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row1189484812512"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1589413486258"><a name="zh-cn_topic_0225569014_p1589413486258"></a><a name="zh-cn_topic_0225569014_p1589413486258"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p148947482254"><a name="zh-cn_topic_0225569014_p148947482254"></a><a name="zh-cn_topic_0225569014_p148947482254"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1689418486254"><a name="zh-cn_topic_0225569014_p1689418486254"></a><a name="zh-cn_topic_0225569014_p1689418486254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p2089444817252"><a name="zh-cn_topic_0225569014_p2089444817252"></a><a name="zh-cn_topic_0225569014_p2089444817252"></a>后端请求方法，支持GET、POST、PUT、DELETE、HEAD、OPTIONS、PATCH、ANY</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row14895164817252"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p11895194818252"><a name="zh-cn_topic_0225569014_p11895194818252"></a><a name="zh-cn_topic_0225569014_p11895194818252"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p28958484255"><a name="zh-cn_topic_0225569014_p28958484255"></a><a name="zh-cn_topic_0225569014_p28958484255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p13895448142512"><a name="zh-cn_topic_0225569014_p13895448142512"></a><a name="zh-cn_topic_0225569014_p13895448142512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1189594813254"><a name="zh-cn_topic_0225569014_p1189594813254"></a><a name="zh-cn_topic_0225569014_p1189594813254"></a>后端请求路径，支持路径变量</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row1689594819251"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p0895104832517"><a name="zh-cn_topic_0225569014_p0895104832517"></a><a name="zh-cn_topic_0225569014_p0895104832517"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p11895184862514"><a name="zh-cn_topic_0225569014_p11895184862514"></a><a name="zh-cn_topic_0225569014_p11895184862514"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p108951948172512"><a name="zh-cn_topic_0225569014_p108951948172512"></a><a name="zh-cn_topic_0225569014_p108951948172512"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1289515487258"><a name="zh-cn_topic_0225569014_p1289515487258"></a><a name="zh-cn_topic_0225569014_p1289515487258"></a>后端请求超时时间，单位毫秒，缺省值为5000，取值范围为1 ~ 60000</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row18895184802511"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p2895134820259"><a name="zh-cn_topic_0225569014_p2895134820259"></a><a name="zh-cn_topic_0225569014_p2895134820259"></a>host</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p9895144815256"><a name="zh-cn_topic_0225569014_p9895144815256"></a><a name="zh-cn_topic_0225569014_p9895144815256"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p168952482254"><a name="zh-cn_topic_0225569014_p168952482254"></a><a name="zh-cn_topic_0225569014_p168952482254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p9896194812253"><a name="zh-cn_topic_0225569014_p9896194812253"></a><a name="zh-cn_topic_0225569014_p9896194812253"></a>VPC通道代理主机</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row126916399464"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1205124114618"><a name="zh-cn_topic_0225569014_p1205124114618"></a><a name="zh-cn_topic_0225569014_p1205124114618"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p11205204144619"><a name="zh-cn_topic_0225569014_p11205204144619"></a><a name="zh-cn_topic_0225569014_p11205204144619"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p172056411467"><a name="zh-cn_topic_0225569014_p172056411467"></a><a name="zh-cn_topic_0225569014_p172056411467"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1520564144612"><a name="zh-cn_topic_0225569014_p1520564144612"></a><a name="zh-cn_topic_0225569014_p1520564144612"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 20**  后端functionEndpoints参数说明

<a name="zh-cn_topic_0225569014_table18971648202512"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row14897184815257"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p1389711486257"><a name="zh-cn_topic_0225569014_p1389711486257"></a><a name="zh-cn_topic_0225569014_p1389711486257"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p1589724814251"><a name="zh-cn_topic_0225569014_p1589724814251"></a><a name="zh-cn_topic_0225569014_p1589724814251"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p589714815258"><a name="zh-cn_topic_0225569014_p589714815258"></a><a name="zh-cn_topic_0225569014_p589714815258"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p389818487257"><a name="zh-cn_topic_0225569014_p389818487257"></a><a name="zh-cn_topic_0225569014_p389818487257"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row58981348182516"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1689814802516"><a name="zh-cn_topic_0225569014_p1689814802516"></a><a name="zh-cn_topic_0225569014_p1689814802516"></a>function-urn</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p7898114818255"><a name="zh-cn_topic_0225569014_p7898114818255"></a><a name="zh-cn_topic_0225569014_p7898114818255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p13898114852515"><a name="zh-cn_topic_0225569014_p13898114852515"></a><a name="zh-cn_topic_0225569014_p13898114852515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p589884811259"><a name="zh-cn_topic_0225569014_p589884811259"></a><a name="zh-cn_topic_0225569014_p589884811259"></a>函数URN地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row128984488256"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p12899648152514"><a name="zh-cn_topic_0225569014_p12899648152514"></a><a name="zh-cn_topic_0225569014_p12899648152514"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1189984814258"><a name="zh-cn_topic_0225569014_p1189984814258"></a><a name="zh-cn_topic_0225569014_p1189984814258"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p178991448162510"><a name="zh-cn_topic_0225569014_p178991448162510"></a><a name="zh-cn_topic_0225569014_p178991448162510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1899174832517"><a name="zh-cn_topic_0225569014_p1899174832517"></a><a name="zh-cn_topic_0225569014_p1899174832517"></a>函数版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row0899134815250"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p9899348162513"><a name="zh-cn_topic_0225569014_p9899348162513"></a><a name="zh-cn_topic_0225569014_p9899348162513"></a>invocation-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p289910485254"><a name="zh-cn_topic_0225569014_p289910485254"></a><a name="zh-cn_topic_0225569014_p289910485254"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p18991348102516"><a name="zh-cn_topic_0225569014_p18991348102516"></a><a name="zh-cn_topic_0225569014_p18991348102516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p189984818250"><a name="zh-cn_topic_0225569014_p189984818250"></a><a name="zh-cn_topic_0225569014_p189984818250"></a>函数调用类型，支持async、sync</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row28995482255"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1290018487253"><a name="zh-cn_topic_0225569014_p1290018487253"></a><a name="zh-cn_topic_0225569014_p1290018487253"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p490010489253"><a name="zh-cn_topic_0225569014_p490010489253"></a><a name="zh-cn_topic_0225569014_p490010489253"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p3900148112515"><a name="zh-cn_topic_0225569014_p3900148112515"></a><a name="zh-cn_topic_0225569014_p3900148112515"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p3900154822516"><a name="zh-cn_topic_0225569014_p3900154822516"></a><a name="zh-cn_topic_0225569014_p3900154822516"></a>函数超时时间，单位毫秒，缺省值为5000，取值范围为1 ~ 60000</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row4948164516468"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p417724714468"><a name="zh-cn_topic_0225569014_p417724714468"></a><a name="zh-cn_topic_0225569014_p417724714468"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p20177147174614"><a name="zh-cn_topic_0225569014_p20177147174614"></a><a name="zh-cn_topic_0225569014_p20177147174614"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p2178184712466"><a name="zh-cn_topic_0225569014_p2178184712466"></a><a name="zh-cn_topic_0225569014_p2178184712466"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p131781547144613"><a name="zh-cn_topic_0225569014_p131781547144613"></a><a name="zh-cn_topic_0225569014_p131781547144613"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 21**  后端mockEndpoints参数说明

<a name="zh-cn_topic_0225569014_table1790184862513"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row1901104812518"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p6902348122511"><a name="zh-cn_topic_0225569014_p6902348122511"></a><a name="zh-cn_topic_0225569014_p6902348122511"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p690215486256"><a name="zh-cn_topic_0225569014_p690215486256"></a><a name="zh-cn_topic_0225569014_p690215486256"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p7902548202519"><a name="zh-cn_topic_0225569014_p7902548202519"></a><a name="zh-cn_topic_0225569014_p7902548202519"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p17902148202518"><a name="zh-cn_topic_0225569014_p17902148202518"></a><a name="zh-cn_topic_0225569014_p17902148202518"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row69021348202511"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p14902448112512"><a name="zh-cn_topic_0225569014_p14902448112512"></a><a name="zh-cn_topic_0225569014_p14902448112512"></a>result-content</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p8902104816254"><a name="zh-cn_topic_0225569014_p8902104816254"></a><a name="zh-cn_topic_0225569014_p8902104816254"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p19903648122510"><a name="zh-cn_topic_0225569014_p19903648122510"></a><a name="zh-cn_topic_0225569014_p19903648122510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p12903948172517"><a name="zh-cn_topic_0225569014_p12903948172517"></a><a name="zh-cn_topic_0225569014_p12903948172517"></a>MOCK返回结果</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row4433155454616"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1576125519468"><a name="zh-cn_topic_0225569014_p1576125519468"></a><a name="zh-cn_topic_0225569014_p1576125519468"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1857675514611"><a name="zh-cn_topic_0225569014_p1857675514611"></a><a name="zh-cn_topic_0225569014_p1857675514611"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p105761955174616"><a name="zh-cn_topic_0225569014_p105761955174616"></a><a name="zh-cn_topic_0225569014_p105761955174616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p05768551462"><a name="zh-cn_topic_0225569014_p05768551462"></a><a name="zh-cn_topic_0225569014_p05768551462"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 22**  conditions参数说明

<a name="zh-cn_topic_0225569014_table1790444832520"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row199040482254"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p169051248112512"><a name="zh-cn_topic_0225569014_p169051248112512"></a><a name="zh-cn_topic_0225569014_p169051248112512"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p590554862518"><a name="zh-cn_topic_0225569014_p590554862518"></a><a name="zh-cn_topic_0225569014_p590554862518"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p190564892511"><a name="zh-cn_topic_0225569014_p190564892511"></a><a name="zh-cn_topic_0225569014_p190564892511"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p4905194815251"><a name="zh-cn_topic_0225569014_p4905194815251"></a><a name="zh-cn_topic_0225569014_p4905194815251"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row390544872514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p69056485258"><a name="zh-cn_topic_0225569014_p69056485258"></a><a name="zh-cn_topic_0225569014_p69056485258"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1290514820256"><a name="zh-cn_topic_0225569014_p1290514820256"></a><a name="zh-cn_topic_0225569014_p1290514820256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p190574819257"><a name="zh-cn_topic_0225569014_p190574819257"></a><a name="zh-cn_topic_0225569014_p190574819257"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1190554892513"><a name="zh-cn_topic_0225569014_p1190554892513"></a><a name="zh-cn_topic_0225569014_p1190554892513"></a>策略条件类型，支持equal、enum、pattern</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row590619487256"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p59061248132511"><a name="zh-cn_topic_0225569014_p59061248132511"></a><a name="zh-cn_topic_0225569014_p59061248132511"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p159064483250"><a name="zh-cn_topic_0225569014_p159064483250"></a><a name="zh-cn_topic_0225569014_p159064483250"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1990644812258"><a name="zh-cn_topic_0225569014_p1990644812258"></a><a name="zh-cn_topic_0225569014_p1990644812258"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1390694812519"><a name="zh-cn_topic_0225569014_p1390694812519"></a><a name="zh-cn_topic_0225569014_p1390694812519"></a>策略条件值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row19906114813251"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p209067480258"><a name="zh-cn_topic_0225569014_p209067480258"></a><a name="zh-cn_topic_0225569014_p209067480258"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p14906184813256"><a name="zh-cn_topic_0225569014_p14906184813256"></a><a name="zh-cn_topic_0225569014_p14906184813256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1690694811252"><a name="zh-cn_topic_0225569014_p1690694811252"></a><a name="zh-cn_topic_0225569014_p1690694811252"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p159071748102517"><a name="zh-cn_topic_0225569014_p159071748102517"></a><a name="zh-cn_topic_0225569014_p159071748102517"></a>策略条件输入来源，支持source、request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row16907248202516"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p6907648162519"><a name="zh-cn_topic_0225569014_p6907648162519"></a><a name="zh-cn_topic_0225569014_p6907648162519"></a>parameter</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1290714882519"><a name="zh-cn_topic_0225569014_p1290714882519"></a><a name="zh-cn_topic_0225569014_p1290714882519"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1690719487254"><a name="zh-cn_topic_0225569014_p1690719487254"></a><a name="zh-cn_topic_0225569014_p1690719487254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p149071484250"><a name="zh-cn_topic_0225569014_p149071484250"></a><a name="zh-cn_topic_0225569014_p149071484250"></a>策略条件输入来源为request时，请求入参的名称</p>
</td>
</tr>
</tbody>
</table>

**表 23**  x-apigateway-access-controls参数说明

<a name="zh-cn_topic_0225569014_table2090754816252"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row179081748172515"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p209087484253"><a name="zh-cn_topic_0225569014_p209087484253"></a><a name="zh-cn_topic_0225569014_p209087484253"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p1490854819254"><a name="zh-cn_topic_0225569014_p1490854819254"></a><a name="zh-cn_topic_0225569014_p1490854819254"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p09082048122514"><a name="zh-cn_topic_0225569014_p09082048122514"></a><a name="zh-cn_topic_0225569014_p09082048122514"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p390944819252"><a name="zh-cn_topic_0225569014_p390944819252"></a><a name="zh-cn_topic_0225569014_p390944819252"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row5909114852510"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p18909174811252"><a name="zh-cn_topic_0225569014_p18909174811252"></a><a name="zh-cn_topic_0225569014_p18909174811252"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p109091448202516"><a name="zh-cn_topic_0225569014_p109091448202516"></a><a name="zh-cn_topic_0225569014_p109091448202516"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p79098488251"><a name="zh-cn_topic_0225569014_p79098488251"></a><a name="zh-cn_topic_0225569014_p79098488251"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p11909114819251"><a name="zh-cn_topic_0225569014_p11909114819251"></a><a name="zh-cn_topic_0225569014_p11909114819251"></a>指定名称的访问控制策略，参考<a href="#zh-cn_topic_0225569014_table39092048142510">表 acl_name参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 24**  acl\_name参数说明

<a name="zh-cn_topic_0225569014_table39092048142510"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row191014812256"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p991017483255"><a name="zh-cn_topic_0225569014_p991017483255"></a><a name="zh-cn_topic_0225569014_p991017483255"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p69108489253"><a name="zh-cn_topic_0225569014_p69108489253"></a><a name="zh-cn_topic_0225569014_p69108489253"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p1591016486250"><a name="zh-cn_topic_0225569014_p1591016486250"></a><a name="zh-cn_topic_0225569014_p1591016486250"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p891110481252"><a name="zh-cn_topic_0225569014_p891110481252"></a><a name="zh-cn_topic_0225569014_p891110481252"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row49111048102517"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p129110482258"><a name="zh-cn_topic_0225569014_p129110482258"></a><a name="zh-cn_topic_0225569014_p129110482258"></a>acl-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p20911104892511"><a name="zh-cn_topic_0225569014_p20911104892511"></a><a name="zh-cn_topic_0225569014_p20911104892511"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p13911174815258"><a name="zh-cn_topic_0225569014_p13911174815258"></a><a name="zh-cn_topic_0225569014_p13911174815258"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p17911174882519"><a name="zh-cn_topic_0225569014_p17911174882519"></a><a name="zh-cn_topic_0225569014_p17911174882519"></a>访问控制行为，支持PERMIT、DENY</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row191154882520"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1191254820251"><a name="zh-cn_topic_0225569014_p1191254820251"></a><a name="zh-cn_topic_0225569014_p1191254820251"></a>entity-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p169121248142514"><a name="zh-cn_topic_0225569014_p169121248142514"></a><a name="zh-cn_topic_0225569014_p169121248142514"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p691294818254"><a name="zh-cn_topic_0225569014_p691294818254"></a><a name="zh-cn_topic_0225569014_p691294818254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p8912948182515"><a name="zh-cn_topic_0225569014_p8912948182515"></a><a name="zh-cn_topic_0225569014_p8912948182515"></a>访问控制对象，支持IP、DOMAIN</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row1391211489258"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p11912194872511"><a name="zh-cn_topic_0225569014_p11912194872511"></a><a name="zh-cn_topic_0225569014_p11912194872511"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p3912248192514"><a name="zh-cn_topic_0225569014_p3912248192514"></a><a name="zh-cn_topic_0225569014_p3912248192514"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p6912848192513"><a name="zh-cn_topic_0225569014_p6912848192513"></a><a name="zh-cn_topic_0225569014_p6912848192513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p9913194862512"><a name="zh-cn_topic_0225569014_p9913194862512"></a><a name="zh-cn_topic_0225569014_p9913194862512"></a>访问控制策略值，多个值以“,”间隔</p>
</td>
</tr>
</tbody>
</table>

**表 25**  x-apigateway-ratelimits参数说明

<a name="zh-cn_topic_0225569014_table18913124872513"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row17913648192518"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p19913848152517"><a name="zh-cn_topic_0225569014_p19913848152517"></a><a name="zh-cn_topic_0225569014_p19913848152517"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p891324822519"><a name="zh-cn_topic_0225569014_p891324822519"></a><a name="zh-cn_topic_0225569014_p891324822519"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p591411483253"><a name="zh-cn_topic_0225569014_p591411483253"></a><a name="zh-cn_topic_0225569014_p591411483253"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p15914144811250"><a name="zh-cn_topic_0225569014_p15914144811250"></a><a name="zh-cn_topic_0225569014_p15914144811250"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row1391424802514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p99141748112512"><a name="zh-cn_topic_0225569014_p99141748112512"></a><a name="zh-cn_topic_0225569014_p99141748112512"></a>throttle_name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p149141489252"><a name="zh-cn_topic_0225569014_p149141489252"></a><a name="zh-cn_topic_0225569014_p149141489252"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p99145487257"><a name="zh-cn_topic_0225569014_p99145487257"></a><a name="zh-cn_topic_0225569014_p99145487257"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p39151248192510"><a name="zh-cn_topic_0225569014_p39151248192510"></a><a name="zh-cn_topic_0225569014_p39151248192510"></a>指定名称的流控策略，参考<a href="#zh-cn_topic_0225569014_table179155483256">表 throttle_name参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 26**  throttle\_name参数说明

<a name="zh-cn_topic_0225569014_table179155483256"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row3915114811258"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p1191616488258"><a name="zh-cn_topic_0225569014_p1191616488258"></a><a name="zh-cn_topic_0225569014_p1191616488258"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p199164484253"><a name="zh-cn_topic_0225569014_p199164484253"></a><a name="zh-cn_topic_0225569014_p199164484253"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p29161648202514"><a name="zh-cn_topic_0225569014_p29161648202514"></a><a name="zh-cn_topic_0225569014_p29161648202514"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p89168486252"><a name="zh-cn_topic_0225569014_p89168486252"></a><a name="zh-cn_topic_0225569014_p89168486252"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row39169488253"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p119161548182514"><a name="zh-cn_topic_0225569014_p119161548182514"></a><a name="zh-cn_topic_0225569014_p119161548182514"></a>api-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1391664819255"><a name="zh-cn_topic_0225569014_p1391664819255"></a><a name="zh-cn_topic_0225569014_p1391664819255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p19174485250"><a name="zh-cn_topic_0225569014_p19174485250"></a><a name="zh-cn_topic_0225569014_p19174485250"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p59171489257"><a name="zh-cn_topic_0225569014_p59171489257"></a><a name="zh-cn_topic_0225569014_p59171489257"></a>API访问次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row14917194852515"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p189171648112514"><a name="zh-cn_topic_0225569014_p189171648112514"></a><a name="zh-cn_topic_0225569014_p189171648112514"></a>user-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p18917174813252"><a name="zh-cn_topic_0225569014_p18917174813252"></a><a name="zh-cn_topic_0225569014_p18917174813252"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p199171348162512"><a name="zh-cn_topic_0225569014_p199171348162512"></a><a name="zh-cn_topic_0225569014_p199171348162512"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p4917448162510"><a name="zh-cn_topic_0225569014_p4917448162510"></a><a name="zh-cn_topic_0225569014_p4917448162510"></a>用户访问次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row129177484252"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p6918104872519"><a name="zh-cn_topic_0225569014_p6918104872519"></a><a name="zh-cn_topic_0225569014_p6918104872519"></a>app-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1091894814255"><a name="zh-cn_topic_0225569014_p1091894814255"></a><a name="zh-cn_topic_0225569014_p1091894814255"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p891804811257"><a name="zh-cn_topic_0225569014_p891804811257"></a><a name="zh-cn_topic_0225569014_p891804811257"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p1918748152512"><a name="zh-cn_topic_0225569014_p1918748152512"></a><a name="zh-cn_topic_0225569014_p1918748152512"></a>应用访问次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row5918648192514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p179181648112513"><a name="zh-cn_topic_0225569014_p179181648112513"></a><a name="zh-cn_topic_0225569014_p179181648112513"></a>ip-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p15918548132512"><a name="zh-cn_topic_0225569014_p15918548132512"></a><a name="zh-cn_topic_0225569014_p15918548132512"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p69181248132518"><a name="zh-cn_topic_0225569014_p69181248132518"></a><a name="zh-cn_topic_0225569014_p69181248132518"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p169192488255"><a name="zh-cn_topic_0225569014_p169192488255"></a><a name="zh-cn_topic_0225569014_p169192488255"></a>源IP访问次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row79191948142513"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p491994816255"><a name="zh-cn_topic_0225569014_p491994816255"></a><a name="zh-cn_topic_0225569014_p491994816255"></a>interval</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p11919114819255"><a name="zh-cn_topic_0225569014_p11919114819255"></a><a name="zh-cn_topic_0225569014_p11919114819255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p79191648132510"><a name="zh-cn_topic_0225569014_p79191648132510"></a><a name="zh-cn_topic_0225569014_p79191648132510"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p119195483257"><a name="zh-cn_topic_0225569014_p119195483257"></a><a name="zh-cn_topic_0225569014_p119195483257"></a>流控策略时间周期</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row199198489254"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p1919154812517"><a name="zh-cn_topic_0225569014_p1919154812517"></a><a name="zh-cn_topic_0225569014_p1919154812517"></a>unit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1391916487253"><a name="zh-cn_topic_0225569014_p1391916487253"></a><a name="zh-cn_topic_0225569014_p1391916487253"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p292015486259"><a name="zh-cn_topic_0225569014_p292015486259"></a><a name="zh-cn_topic_0225569014_p292015486259"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p3920748112517"><a name="zh-cn_topic_0225569014_p3920748112517"></a><a name="zh-cn_topic_0225569014_p3920748112517"></a>流控策略时间周期单位，支持SECOND、MINUTE、HOUR、DAY</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row14920174811258"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p7920948132515"><a name="zh-cn_topic_0225569014_p7920948132515"></a><a name="zh-cn_topic_0225569014_p7920948132515"></a>shared</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p192019487254"><a name="zh-cn_topic_0225569014_p192019487254"></a><a name="zh-cn_topic_0225569014_p192019487254"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1920124892513"><a name="zh-cn_topic_0225569014_p1920124892513"></a><a name="zh-cn_topic_0225569014_p1920124892513"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p17920174842518"><a name="zh-cn_topic_0225569014_p17920174842518"></a><a name="zh-cn_topic_0225569014_p17920174842518"></a>是否共享流控策略</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row1392010481255"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p6921194816259"><a name="zh-cn_topic_0225569014_p6921194816259"></a><a name="zh-cn_topic_0225569014_p6921194816259"></a>special</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p29212489254"><a name="zh-cn_topic_0225569014_p29212489254"></a><a name="zh-cn_topic_0225569014_p29212489254"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p792119480253"><a name="zh-cn_topic_0225569014_p792119480253"></a><a name="zh-cn_topic_0225569014_p792119480253"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p15921144832520"><a name="zh-cn_topic_0225569014_p15921144832520"></a><a name="zh-cn_topic_0225569014_p15921144832520"></a>特殊流控策略对象数组定义，参考<a href="#zh-cn_topic_0225569014_table6921174842513">表 special参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 27**  special参数说明

<a name="zh-cn_topic_0225569014_table6921174842513"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row5922248112514"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569014_p1492234818256"><a name="zh-cn_topic_0225569014_p1492234818256"></a><a name="zh-cn_topic_0225569014_p1492234818256"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569014_p1292214818252"><a name="zh-cn_topic_0225569014_p1292214818252"></a><a name="zh-cn_topic_0225569014_p1292214818252"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569014_p1192217488256"><a name="zh-cn_topic_0225569014_p1192217488256"></a><a name="zh-cn_topic_0225569014_p1192217488256"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569014_p19922144810251"><a name="zh-cn_topic_0225569014_p19922144810251"></a><a name="zh-cn_topic_0225569014_p19922144810251"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row109221348122519"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p4923448142518"><a name="zh-cn_topic_0225569014_p4923448142518"></a><a name="zh-cn_topic_0225569014_p4923448142518"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p792311483258"><a name="zh-cn_topic_0225569014_p792311483258"></a><a name="zh-cn_topic_0225569014_p792311483258"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p392311487256"><a name="zh-cn_topic_0225569014_p392311487256"></a><a name="zh-cn_topic_0225569014_p392311487256"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p292315488259"><a name="zh-cn_topic_0225569014_p292315488259"></a><a name="zh-cn_topic_0225569014_p292315488259"></a>特殊流控策略类型，支持APP、USER</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row1692304842514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p192311482252"><a name="zh-cn_topic_0225569014_p192311482252"></a><a name="zh-cn_topic_0225569014_p192311482252"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p1292364814256"><a name="zh-cn_topic_0225569014_p1292364814256"></a><a name="zh-cn_topic_0225569014_p1292364814256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p1092344819252"><a name="zh-cn_topic_0225569014_p1092344819252"></a><a name="zh-cn_topic_0225569014_p1092344819252"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p13923134817259"><a name="zh-cn_topic_0225569014_p13923134817259"></a><a name="zh-cn_topic_0225569014_p13923134817259"></a>访问次数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row13923948122511"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569014_p15923248172511"><a name="zh-cn_topic_0225569014_p15923248172511"></a><a name="zh-cn_topic_0225569014_p15923248172511"></a>instance</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569014_p4924448162510"><a name="zh-cn_topic_0225569014_p4924448162510"></a><a name="zh-cn_topic_0225569014_p4924448162510"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569014_p119249482253"><a name="zh-cn_topic_0225569014_p119249482253"></a><a name="zh-cn_topic_0225569014_p119249482253"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569014_p5924154822518"><a name="zh-cn_topic_0225569014_p5924154822518"></a><a name="zh-cn_topic_0225569014_p5924154822518"></a>特殊APP或USER的对象标识</p>
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

## 响应消息<a name="zh-cn_topic_0225569014_section3346174120197"></a>

**表 28**  参数说明

<a name="zh-cn_topic_0225569014_table17320161865510"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row20324111812552"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225569014_p1032791895512"><a name="zh-cn_topic_0225569014_p1032791895512"></a><a name="zh-cn_topic_0225569014_p1032791895512"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225569014_p16328111805514"><a name="zh-cn_topic_0225569014_p16328111805514"></a><a name="zh-cn_topic_0225569014_p16328111805514"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.415841584158414%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225569014_p183299183551"><a name="zh-cn_topic_0225569014_p183299183551"></a><a name="zh-cn_topic_0225569014_p183299183551"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row7519312131514"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569014_p10520712111516"><a name="zh-cn_topic_0225569014_p10520712111516"></a><a name="zh-cn_topic_0225569014_p10520712111516"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569014_p13520151211157"><a name="zh-cn_topic_0225569014_p13520151211157"></a><a name="zh-cn_topic_0225569014_p13520151211157"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569014_p352061212159"><a name="zh-cn_topic_0225569014_p352061212159"></a><a name="zh-cn_topic_0225569014_p352061212159"></a>分组ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row4331151855520"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569014_p782812469154"><a name="zh-cn_topic_0225569014_p782812469154"></a><a name="zh-cn_topic_0225569014_p782812469154"></a>success</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569014_p1029215518551"><a name="zh-cn_topic_0225569014_p1029215518551"></a><a name="zh-cn_topic_0225569014_p1029215518551"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569014_p3336918115517"><a name="zh-cn_topic_0225569014_p3336918115517"></a><a name="zh-cn_topic_0225569014_p3336918115517"></a>导入成功信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row153379185556"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569014_p1433831818554"><a name="zh-cn_topic_0225569014_p1433831818554"></a><a name="zh-cn_topic_0225569014_p1433831818554"></a>failure</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569014_p333831825520"><a name="zh-cn_topic_0225569014_p333831825520"></a><a name="zh-cn_topic_0225569014_p333831825520"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569014_p4340111810552"><a name="zh-cn_topic_0225569014_p4340111810552"></a><a name="zh-cn_topic_0225569014_p4340111810552"></a>导入失败信息</p>
</td>
</tr>
</tbody>
</table>

**表 29**  success参数说明

<a name="zh-cn_topic_0225569014_table2981672313"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row898177103111"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225569014_p109837183116"><a name="zh-cn_topic_0225569014_p109837183116"></a><a name="zh-cn_topic_0225569014_p109837183116"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225569014_p1098474319"><a name="zh-cn_topic_0225569014_p1098474319"></a><a name="zh-cn_topic_0225569014_p1098474319"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.415841584158414%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225569014_p1398197193117"><a name="zh-cn_topic_0225569014_p1398197193117"></a><a name="zh-cn_topic_0225569014_p1398197193117"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row49812719314"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569014_p18981672315"><a name="zh-cn_topic_0225569014_p18981672315"></a><a name="zh-cn_topic_0225569014_p18981672315"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569014_p209815717318"><a name="zh-cn_topic_0225569014_p209815717318"></a><a name="zh-cn_topic_0225569014_p209815717318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569014_p8980773120"><a name="zh-cn_topic_0225569014_p8980773120"></a><a name="zh-cn_topic_0225569014_p8980773120"></a>导入成功的API ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row119827123112"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569014_p159814710314"><a name="zh-cn_topic_0225569014_p159814710314"></a><a name="zh-cn_topic_0225569014_p159814710314"></a>action</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569014_p1698871311"><a name="zh-cn_topic_0225569014_p1698871311"></a><a name="zh-cn_topic_0225569014_p1698871311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569014_p43372294157"><a name="zh-cn_topic_0225569014_p43372294157"></a><a name="zh-cn_topic_0225569014_p43372294157"></a>导入行为：</p>
<a name="zh-cn_topic_0225569014_ul18322112914151"></a><a name="zh-cn_topic_0225569014_ul18322112914151"></a><ul id="zh-cn_topic_0225569014_ul18322112914151"><li>update：表示更新API</li><li>create：表示新建API</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row1919781375316"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569014_p8197131345315"><a name="zh-cn_topic_0225569014_p8197131345315"></a><a name="zh-cn_topic_0225569014_p8197131345315"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569014_p3197101395317"><a name="zh-cn_topic_0225569014_p3197101395317"></a><a name="zh-cn_topic_0225569014_p3197101395317"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569014_p41971813165317"><a name="zh-cn_topic_0225569014_p41971813165317"></a><a name="zh-cn_topic_0225569014_p41971813165317"></a>API请求方法</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row998187163114"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569014_p129814713315"><a name="zh-cn_topic_0225569014_p129814713315"></a><a name="zh-cn_topic_0225569014_p129814713315"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569014_p13987723113"><a name="zh-cn_topic_0225569014_p13987723113"></a><a name="zh-cn_topic_0225569014_p13987723113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569014_p109819712314"><a name="zh-cn_topic_0225569014_p109819712314"></a><a name="zh-cn_topic_0225569014_p109819712314"></a>API请求路径</p>
</td>
</tr>
</tbody>
</table>

**表 30**  failure参数说明

<a name="zh-cn_topic_0225569014_table15660564193"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row137265631919"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225569014_p173165641915"><a name="zh-cn_topic_0225569014_p173165641915"></a><a name="zh-cn_topic_0225569014_p173165641915"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225569014_p187385616195"><a name="zh-cn_topic_0225569014_p187385616195"></a><a name="zh-cn_topic_0225569014_p187385616195"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.415841584158414%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225569014_p1876256171919"><a name="zh-cn_topic_0225569014_p1876256171919"></a><a name="zh-cn_topic_0225569014_p1876256171919"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row138175661920"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569014_p11458112915203"><a name="zh-cn_topic_0225569014_p11458112915203"></a><a name="zh-cn_topic_0225569014_p11458112915203"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569014_p38145613190"><a name="zh-cn_topic_0225569014_p38145613190"></a><a name="zh-cn_topic_0225569014_p38145613190"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569014_p1882175612193"><a name="zh-cn_topic_0225569014_p1882175612193"></a><a name="zh-cn_topic_0225569014_p1882175612193"></a>导入失败的错误码</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row18262135516207"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569014_p142627557208"><a name="zh-cn_topic_0225569014_p142627557208"></a><a name="zh-cn_topic_0225569014_p142627557208"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569014_p1426220553205"><a name="zh-cn_topic_0225569014_p1426220553205"></a><a name="zh-cn_topic_0225569014_p1426220553205"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569014_p32621855152010"><a name="zh-cn_topic_0225569014_p32621855152010"></a><a name="zh-cn_topic_0225569014_p32621855152010"></a>导入失败的错误信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row236592717212"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569014_p1836592772116"><a name="zh-cn_topic_0225569014_p1836592772116"></a><a name="zh-cn_topic_0225569014_p1836592772116"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569014_p736592710219"><a name="zh-cn_topic_0225569014_p736592710219"></a><a name="zh-cn_topic_0225569014_p736592710219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569014_p1036518272216"><a name="zh-cn_topic_0225569014_p1036518272216"></a><a name="zh-cn_topic_0225569014_p1036518272216"></a>API请求方法</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row17854183118217"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569014_p5854731142118"><a name="zh-cn_topic_0225569014_p5854731142118"></a><a name="zh-cn_topic_0225569014_p5854731142118"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569014_p5854143112210"><a name="zh-cn_topic_0225569014_p5854143112210"></a><a name="zh-cn_topic_0225569014_p5854143112210"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569014_p128541531162113"><a name="zh-cn_topic_0225569014_p128541531162113"></a><a name="zh-cn_topic_0225569014_p128541531162113"></a>API请求路径</p>
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

## 状态码<a name="zh-cn_topic_0225569014_section67075185"></a>

**表 31**  返回消息说明

<a name="zh-cn_topic_0225569014_table15714732"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569014_row24997277"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225569014_p11513591"><a name="zh-cn_topic_0225569014_p11513591"></a><a name="zh-cn_topic_0225569014_p11513591"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225569014_p60185706"><a name="zh-cn_topic_0225569014_p60185706"></a><a name="zh-cn_topic_0225569014_p60185706"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569014_row43203997"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569014_p9862840"><a name="zh-cn_topic_0225569014_p9862840"></a><a name="zh-cn_topic_0225569014_p9862840"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569014_p73578115452"><a name="zh-cn_topic_0225569014_p73578115452"></a><a name="zh-cn_topic_0225569014_p73578115452"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row9362312"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569014_p20149775"><a name="zh-cn_topic_0225569014_p20149775"></a><a name="zh-cn_topic_0225569014_p20149775"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569014_p21519099"><a name="zh-cn_topic_0225569014_p21519099"></a><a name="zh-cn_topic_0225569014_p21519099"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row43351211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569014_p21787193"><a name="zh-cn_topic_0225569014_p21787193"></a><a name="zh-cn_topic_0225569014_p21787193"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569014_p13949586"><a name="zh-cn_topic_0225569014_p13949586"></a><a name="zh-cn_topic_0225569014_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569014_row63248959"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569014_p22892027"><a name="zh-cn_topic_0225569014_p22892027"></a><a name="zh-cn_topic_0225569014_p22892027"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569014_p14947689"><a name="zh-cn_topic_0225569014_p14947689"></a><a name="zh-cn_topic_0225569014_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

