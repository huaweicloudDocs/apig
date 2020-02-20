# API概览<a name="apig-zh-api-180713002"></a>

API网关接口的分类与说明如[表1](#table51381943105818)所示。

**表 1**  接口分类

<a name="table51381943105818"></a>
<table><thead align="left"><tr id="row131381543195812"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.3.1.1"><p id="p14138124385819"><a name="p14138124385819"></a><a name="p14138124385819"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="75%" id="mcps1.2.3.1.2"><p id="p1913824317588"><a name="p1913824317588"></a><a name="p1913824317588"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row613834325813"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p141382436588"><a name="p141382436588"></a><a name="p141382436588"></a><a href="#section9903205319458">API分组管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p1013894355820"><a name="p1013894355820"></a><a name="p1013894355820"></a>包括API分组的创建、修改、删除和查询等接口。</p>
</td>
</tr>
<tr id="row14138114313586"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p3138943185811"><a name="p3138943185811"></a><a name="p3138943185811"></a><a href="#section1823414124520">API管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p1513884314581"><a name="p1513884314581"></a><a name="p1513884314581"></a>包括API的注册、修改、删除、发布、下线和查询等接口。</p>
</td>
</tr>
<tr id="row4138104312585"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p11138164345813"><a name="p11138164345813"></a><a name="p11138164345813"></a><a href="#section12876258121114">APP管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p16138743125811"><a name="p16138743125811"></a><a name="p16138743125811"></a>包括APP的创建、修改、删除、重置密钥和查询等接口。</p>
</td>
</tr>
<tr id="row413884310584"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p913884311584"><a name="p913884311584"></a><a name="p913884311584"></a><a href="#section6865132341216">APP授权管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p1013812431588"><a name="p1013812431588"></a><a name="p1013812431588"></a>包括授权、解除授权、查询授权关系等接口。</p>
</td>
</tr>
<tr id="row81380439588"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p1013813435586"><a name="p1013813435586"></a><a name="p1013813435586"></a><a href="#section6760192691213">环境管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p19138124345817"><a name="p19138124345817"></a><a name="p19138124345817"></a>包括环境的创建、修改、删除和查询接口。</p>
</td>
</tr>
<tr id="row18138194312588"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p101381443105814"><a name="p101381443105814"></a><a name="p101381443105814"></a><a href="#section65941327111210">环境变量管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p161388432582"><a name="p161388432582"></a><a name="p161388432582"></a>包括环境变量的创建、删除和查询等接口。</p>
</td>
</tr>
<tr id="row1813884316584"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p1913824312588"><a name="p1913824312588"></a><a name="p1913824312588"></a><a href="#section111071629171218">流控策略管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p51381843165819"><a name="p51381843165819"></a><a name="p51381843165819"></a>包括流控策略的创建、修改、删除和查询等接口。</p>
</td>
</tr>
<tr id="row1113844385817"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p1713816433581"><a name="p1713816433581"></a><a name="p1713816433581"></a><a href="#section2096163010121">API绑定流控策略</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p1613884318585"><a name="p1613884318585"></a><a name="p1613884318585"></a>包括流控策略的查询、绑定和解除绑定等接口。</p>
</td>
</tr>
<tr id="row15138104395820"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p1613818437585"><a name="p1613818437585"></a><a name="p1613818437585"></a><a href="#section85591019133416">设置特殊流控</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p1113834365820"><a name="p1113834365820"></a><a name="p1113834365820"></a>包括特殊流控的创建、修改、删除和查询接口。</p>
</td>
</tr>
<tr id="row18139134310589"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p813994312584"><a name="p813994312584"></a><a name="p813994312584"></a><a href="#section45751720133416">概要查询</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p913920437580"><a name="p913920437580"></a><a name="p913920437580"></a>包括概要信息的查询接口。</p>
</td>
</tr>
<tr id="row31391743145818"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p14139743105815"><a name="p14139743105815"></a><a name="p14139743105815"></a><a href="#section1264415217349">签名密钥管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p20139124311585"><a name="p20139124311585"></a><a name="p20139124311585"></a>包括签名密钥的创建、修改、删除和查询接口。</p>
</td>
</tr>
<tr id="row1113917435581"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p161408432581"><a name="p161408432581"></a><a name="p161408432581"></a><a href="#section1060611256535">签名密钥绑定关系管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p1014094365814"><a name="p1014094365814"></a><a name="p1014094365814"></a>包括签名密钥的绑定和解除绑定接口，查询签名密钥绑定/未绑定API列表接口。</p>
</td>
</tr>
<tr id="row1414012430584"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p71401543185813"><a name="p71401543185813"></a><a name="p71401543185813"></a><a href="#section18754102615315">域名管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p17140194315810"><a name="p17140194315810"></a><a name="p17140194315810"></a>包括域名的绑定、解绑和证书的绑定、删除接口。</p>
</td>
</tr>
<tr id="row067493915114"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p17676193911115"><a name="p17676193911115"></a><a name="p17676193911115"></a><a href="#section2938112745315">VPC通道管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p10676639141114"><a name="p10676639141114"></a><a name="p10676639141114"></a>包括创建VPC通道、更新VPC通道、删除VPC通道、查看VPC通道详情和列表、添加和删除云服务器、查看云服务器列表。</p>
</td>
</tr>
</tbody>
</table>

## API分组管理<a name="section9903205319458"></a>

<a name="table19481502473"></a>
<table><thead align="left"><tr id="row13948108477"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.3.1.1"><p id="p209481607471"><a name="p209481607471"></a><a name="p209481607471"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="75%" id="mcps1.1.3.1.2"><p id="p1594819084712"><a name="p1594819084712"></a><a name="p1594819084712"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7948105472"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p1394820154718"><a name="p1394820154718"></a><a name="p1394820154718"></a><a href="创建API分组.md">创建API分组</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p6948207479"><a name="p6948207479"></a><a name="p6948207479"></a>创建一个API分组。</p>
<p id="p11858115410618"><a name="p11858115410618"></a><a name="p11858115410618"></a>API分组是API的管理单元，一个API分组等同于一个服务入口。</p>
</td>
</tr>
<tr id="row1294811018476"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p7948120164711"><a name="p7948120164711"></a><a name="p7948120164711"></a><a href="修改API分组.md">修改API分组</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p1948180144715"><a name="p1948180144715"></a><a name="p1948180144715"></a>修改API分组属性。</p>
</td>
</tr>
<tr id="row1948180114716"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p094840134715"><a name="p094840134715"></a><a name="p094840134715"></a><a href="删除API分组.md">删除API分组</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p18948170124716"><a name="p18948170124716"></a><a name="p18948170124716"></a>删除指定的API分组。</p>
</td>
</tr>
<tr id="row1594850124717"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p14948150144710"><a name="p14948150144710"></a><a name="p14948150144710"></a><a href="查看分组详情.md">查看分组详情</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p5948205478"><a name="p5948205478"></a><a name="p5948205478"></a>查询指定分组的详细信息</p>
</td>
</tr>
<tr id="row16291531736"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p26302031631"><a name="p26302031631"></a><a name="p26302031631"></a><a href="查询分组列表.md">查询分组列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p206301831734"><a name="p206301831734"></a><a name="p206301831734"></a>查询API分组列表。</p>
</td>
</tr>
</tbody>
</table>

## API管理<a name="section1823414124520"></a>

<a name="table8745105120813"></a>
<table><thead align="left"><tr id="row274519511184"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.3.1.1"><p id="p27458517819"><a name="p27458517819"></a><a name="p27458517819"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="75%" id="mcps1.1.3.1.2"><p id="p177457511816"><a name="p177457511816"></a><a name="p177457511816"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row57458511981"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p3487455989"><a name="p3487455989"></a><a name="p3487455989"></a><a href="注册API.md">注册API</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p1748613552811"><a name="p1748613552811"></a><a name="p1748613552811"></a>创建一个API。</p>
<p id="p12740174121310"><a name="p12740174121310"></a><a name="p12740174121310"></a>API即一个服务接口，具体的服务能力。</p>
</td>
</tr>
<tr id="row1774613516813"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p194841855784"><a name="p194841855784"></a><a name="p194841855784"></a><a href="修改API.md">修改API</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p1648345515819"><a name="p1648345515819"></a><a name="p1648345515819"></a>修改指定API的信息。</p>
</td>
</tr>
<tr id="row1674625116817"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p1548219555813"><a name="p1548219555813"></a><a name="p1548219555813"></a><a href="删除API.md">删除API</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p174814554818"><a name="p174814554818"></a><a name="p174814554818"></a>删除指定的API。</p>
</td>
</tr>
<tr id="row2074620516819"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p1347919552814"><a name="p1347919552814"></a><a name="p1347919552814"></a><a href="发布API.md">发布API</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p14784551880"><a name="p14784551880"></a><a name="p14784551880"></a>将一个指定的API发布到一个指定的环境，API只有发布后，才能够被调用。</p>
</td>
</tr>
<tr id="row574613513813"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p847715554817"><a name="p847715554817"></a><a name="p847715554817"></a><a href="下线API.md">下线API</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p194769551884"><a name="p194769551884"></a><a name="p194769551884"></a>将API从某个已发布的环境上下线，下线后，API将无法再被调用。</p>
</td>
</tr>
<tr id="row15734381101"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p273416818104"><a name="p273416818104"></a><a name="p273416818104"></a><a href="查看API详情.md">查看API详情</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p14734683104"><a name="p14734683104"></a><a name="p14734683104"></a>查看指定的API的详细信息。</p>
</td>
</tr>
<tr id="row2057171161011"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p45791112109"><a name="p45791112109"></a><a name="p45791112109"></a><a href="查询API列表.md">查询API列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p105721171015"><a name="p105721171015"></a><a name="p105721171015"></a>查看API列表。</p>
</td>
</tr>
</tbody>
</table>

## APP管理<a name="section12876258121114"></a>

<a name="table19685151341211"></a>
<table><thead align="left"><tr id="row18686191311125"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.3.1.1"><p id="p56861313101211"><a name="p56861313101211"></a><a name="p56861313101211"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="75%" id="mcps1.1.3.1.2"><p id="p14686713101220"><a name="p14686713101220"></a><a name="p14686713101220"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row168631371211"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p1368491615129"><a name="p1368491615129"></a><a name="p1368491615129"></a><a href="创建APP.md">创建APP</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p116863133125"><a name="p116863133125"></a><a name="p116863133125"></a>创建一个APP。</p>
<p id="p28445917181"><a name="p28445917181"></a><a name="p28445917181"></a>APP即应用，是一个可以访问API的身份标识。</p>
</td>
</tr>
<tr id="row17686181313125"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p06832016161215"><a name="p06832016161215"></a><a name="p06832016161215"></a><a href="修改APP.md">修改APP</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p168791316123"><a name="p168791316123"></a><a name="p168791316123"></a>修改指定APP的信息。</p>
</td>
</tr>
<tr id="row166872013191211"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p9682141611210"><a name="p9682141611210"></a><a name="p9682141611210"></a><a href="重置密钥.md">重置密钥</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p3687813111211"><a name="p3687813111211"></a><a name="p3687813111211"></a>重置指定APP的密钥。</p>
</td>
</tr>
<tr id="row19687513101210"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p468201619122"><a name="p468201619122"></a><a name="p468201619122"></a><a href="删除APP.md">删除APP</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p166871613111217"><a name="p166871613111217"></a><a name="p166871613111217"></a>删除指定的APP。</p>
</td>
</tr>
<tr id="row18687191314121"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p668051614120"><a name="p668051614120"></a><a name="p668051614120"></a><a href="校验APP.md">校验APP</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p868791361210"><a name="p868791361210"></a><a name="p868791361210"></a>校验APP是否存在。</p>
</td>
</tr>
<tr id="row46878132129"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p268016165124"><a name="p268016165124"></a><a name="p268016165124"></a><a href="查看APP详情.md">查看APP详情</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p568781314128"><a name="p568781314128"></a><a name="p568781314128"></a>查看指定APP的详细信息。</p>
</td>
</tr>
<tr id="row3687413141218"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p6678316101210"><a name="p6678316101210"></a><a name="p6678316101210"></a><a href="查询APP列表.md">查询APP列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p268712138126"><a name="p268712138126"></a><a name="p268712138126"></a>查询APP列表。</p>
</td>
</tr>
</tbody>
</table>

## APP授权管理<a name="section6865132341216"></a>

<a name="table2865202315124"></a>
<table><thead align="left"><tr id="row138651023121215"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.3.1.1"><p id="p6865323121214"><a name="p6865323121214"></a><a name="p6865323121214"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="75%" id="mcps1.1.3.1.2"><p id="p148651923181218"><a name="p148651923181218"></a><a name="p148651923181218"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row8865152381215"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p1686562314127"><a name="p1686562314127"></a><a name="p1686562314127"></a><a href="查看APP未绑定的API列表.md">查看APP未绑定的API列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p3866923141217"><a name="p3866923141217"></a><a name="p3866923141217"></a>查询指定环境上某个APP未绑定的API列表。</p>
</td>
</tr>
<tr id="row686682315121"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p128662232125"><a name="p128662232125"></a><a name="p128662232125"></a><a href="授权.md">授权</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p28661523121215"><a name="p28661523121215"></a><a name="p28661523121215"></a>APP创建成功后，还不能访问API，如果想要访问某个环境上的API，需要将该API在该环境上授权给APP。</p>
</td>
</tr>
<tr id="row98661323121220"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p686692317121"><a name="p686692317121"></a><a name="p686692317121"></a><a href="查看APP已绑定的API列表.md">查看APP已绑定的API列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p286682361215"><a name="p286682361215"></a><a name="p286682361215"></a>查询APP已经绑定的API列表。</p>
</td>
</tr>
<tr id="row20866172310124"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p586610238129"><a name="p586610238129"></a><a name="p586610238129"></a><a href="查看API已绑定的APP列表.md">查看API已绑定的APP列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p13866172312120"><a name="p13866172312120"></a><a name="p13866172312120"></a>查询API绑定的APP列表。</p>
</td>
</tr>
<tr id="row1286622311212"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p1086672371219"><a name="p1086672371219"></a><a name="p1086672371219"></a><a href="解除授权.md">解除授权</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p153841520102416"><a name="p153841520102416"></a><a name="p153841520102416"></a>解除API对APP的授权关系。</p>
<p id="p38668234124"><a name="p38668234124"></a><a name="p38668234124"></a>解除授权后，APP将不再能够调用该API。</p>
</td>
</tr>
</tbody>
</table>

## 环境管理<a name="section6760192691213"></a>

<a name="table11761726161215"></a>
<table><thead align="left"><tr id="row87617263127"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.3.1.1"><p id="p1876142615127"><a name="p1876142615127"></a><a name="p1876142615127"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="75%" id="mcps1.1.3.1.2"><p id="p87611526121211"><a name="p87611526121211"></a><a name="p87611526121211"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row19761152651218"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p676132618121"><a name="p676132618121"></a><a name="p676132618121"></a><a href="创建环境.md">创建环境</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p107611126201220"><a name="p107611126201220"></a><a name="p107611126201220"></a>创建一个自定义的环境。</p>
</td>
</tr>
<tr id="row11761426111219"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p157611526101210"><a name="p157611526101210"></a><a name="p157611526101210"></a><a href="修改环境.md">修改环境</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p976110262125"><a name="p976110262125"></a><a name="p976110262125"></a>修改指定环境的信息。</p>
</td>
</tr>
<tr id="row476119268128"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p576112615128"><a name="p576112615128"></a><a name="p576112615128"></a><a href="删除环境.md">删除环境</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p1776152611218"><a name="p1776152611218"></a><a name="p1776152611218"></a>删除指定的环境。</p>
</td>
</tr>
<tr id="row376115263125"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p14761326101216"><a name="p14761326101216"></a><a name="p14761326101216"></a><a href="查询环境列表.md">查询环境列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p1076152615125"><a name="p1076152615125"></a><a name="p1076152615125"></a>查询符合条件的环境列表。</p>
</td>
</tr>
</tbody>
</table>

## 环境变量管理<a name="section65941327111210"></a>

<a name="table75958271123"></a>
<table><thead align="left"><tr id="row159522771219"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.3.1.1"><p id="p16595727111218"><a name="p16595727111218"></a><a name="p16595727111218"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="75%" id="mcps1.1.3.1.2"><p id="p8595172791217"><a name="p8595172791217"></a><a name="p8595172791217"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row14595152721216"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p959632761210"><a name="p959632761210"></a><a name="p959632761210"></a><a href="新建变量.md">新建变量</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p9596142711128"><a name="p9596142711128"></a><a name="p9596142711128"></a>新建一个环境变量。</p>
<p id="p34761520153115"><a name="p34761520153115"></a><a name="p34761520153115"></a>环境变量定义在API分组上，该分组下的所有API都可以使用这些变量。</p>
</td>
</tr>
<tr id="row3596192711122"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p25961827141212"><a name="p25961827141212"></a><a name="p25961827141212"></a><a href="删除变量.md">删除变量</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p459622716122"><a name="p459622716122"></a><a name="p459622716122"></a>删除指定的环境变量。</p>
</td>
</tr>
<tr id="row9596227191215"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p125969271122"><a name="p125969271122"></a><a name="p125969271122"></a><a href="查看变量详情.md">查看变量详情</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p85961277128"><a name="p85961277128"></a><a name="p85961277128"></a>查看指定的环境变量的详情。</p>
</td>
</tr>
<tr id="row859611277125"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p359610274122"><a name="p359610274122"></a><a name="p359610274122"></a><a href="查询变量列表.md">查询变量列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p11596172771211"><a name="p11596172771211"></a><a name="p11596172771211"></a>查询分组下的所有环境变量的列表。</p>
</td>
</tr>
</tbody>
</table>

## 流控策略管理<a name="section111071629171218"></a>

<a name="table121071929161211"></a>
<table><thead align="left"><tr id="row410812920120"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.3.1.1"><p id="p7108192941215"><a name="p7108192941215"></a><a name="p7108192941215"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="75%" id="mcps1.1.3.1.2"><p id="p5108152910128"><a name="p5108152910128"></a><a name="p5108152910128"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1210862915124"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p1610815298120"><a name="p1610815298120"></a><a name="p1610815298120"></a><a href="创建流控策略.md">创建流控策略</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p1710818298123"><a name="p1710818298123"></a><a name="p1710818298123"></a>创建一个流控策略。</p>
<p id="p721216251355"><a name="p721216251355"></a><a name="p721216251355"></a>流控策略即限制API在一定长度的时间内，能够允许被访问的最大次数。</p>
</td>
</tr>
<tr id="row13108122961215"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p19108162941216"><a name="p19108162941216"></a><a name="p19108162941216"></a><a href="修改流控策略.md">修改流控策略</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p3108162941213"><a name="p3108162941213"></a><a name="p3108162941213"></a>修改指定流控策略的详细信息。</p>
</td>
</tr>
<tr id="row71081929131212"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p19108829121217"><a name="p19108829121217"></a><a name="p19108829121217"></a><a href="删除流控策略.md">删除流控策略</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p910815297126"><a name="p910815297126"></a><a name="p910815297126"></a>删除指定的流控策略，以及该流控策略与API的所有绑定关系。</p>
</td>
</tr>
<tr id="row14108182913126"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p101081929131212"><a name="p101081929131212"></a><a name="p101081929131212"></a><a href="查看流控策略详情.md">查看流控策略详情</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p1610822911126"><a name="p1610822911126"></a><a name="p1610822911126"></a>查看指定流控策略的详细信息。</p>
</td>
</tr>
<tr id="row210813291128"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p2109122916121"><a name="p2109122916121"></a><a name="p2109122916121"></a><a href="查询流控策略列表.md">查询流控策略列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p1810932921215"><a name="p1810932921215"></a><a name="p1810932921215"></a>查询所有流控策略的信息。</p>
</td>
</tr>
</tbody>
</table>

## API绑定流控策略<a name="section2096163010121"></a>

<a name="table189717305122"></a>
<table><thead align="left"><tr id="row59715304129"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.3.1.1"><p id="p297113051215"><a name="p297113051215"></a><a name="p297113051215"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="75%" id="mcps1.1.3.1.2"><p id="p20971130111216"><a name="p20971130111216"></a><a name="p20971130111216"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row79710300129"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p15979309123"><a name="p15979309123"></a><a name="p15979309123"></a><a href="查看流控策略未绑定的API列表.md">查看流控策略未绑定的API列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p119817309128"><a name="p119817309128"></a><a name="p119817309128"></a>查询所有未绑定到该流控策略上的自有API列表。</p>
</td>
</tr>
<tr id="row298153071215"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p1798130191213"><a name="p1798130191213"></a><a name="p1798130191213"></a><a href="绑定流控策略.md">绑定流控策略</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p1398153021212"><a name="p1398153021212"></a><a name="p1398153021212"></a>为指定的API绑定流控策略，绑定时，需要指定在哪个环境上生效。</p>
</td>
</tr>
<tr id="row109815301122"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p1498130131210"><a name="p1498130131210"></a><a name="p1498130131210"></a><a href="查看流控策略绑定的API列表.md">查看流控策略绑定的API列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p3983304120"><a name="p3983304120"></a><a name="p3983304120"></a>查询某个流控策略上已经绑定的API列表。</p>
</td>
</tr>
<tr id="row1198123021217"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p199853021211"><a name="p199853021211"></a><a name="p199853021211"></a><a href="查看API绑定的流控策略列表.md">查看API绑定的流控策略列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p199863011220"><a name="p199863011220"></a><a name="p199863011220"></a>查询某个API绑定的流控策略列表。</p>
</td>
</tr>
<tr id="row59883016126"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p119843012122"><a name="p119843012122"></a><a name="p119843012122"></a><a href="解除绑定.md">解除绑定</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p1598173010122"><a name="p1598173010122"></a><a name="p1598173010122"></a>解除API与流控策略的绑定关系。</p>
</td>
</tr>
</tbody>
</table>

## 设置特殊流控<a name="section85591019133416"></a>

<a name="table1856051911345"></a>
<table><thead align="left"><tr id="row195608192345"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.3.1.1"><p id="p15560101973411"><a name="p15560101973411"></a><a name="p15560101973411"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="75%" id="mcps1.1.3.1.2"><p id="p155601019203414"><a name="p155601019203414"></a><a name="p155601019203414"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row5560191910344"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p95605196346"><a name="p95605196346"></a><a name="p95605196346"></a><a href="创建特殊设置.md">创建特殊设置</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p0561319163410"><a name="p0561319163410"></a><a name="p0561319163410"></a>为流控策略添加一个特殊设置的对象。</p>
</td>
</tr>
<tr id="row15561201933418"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p10561201914347"><a name="p10561201914347"></a><a name="p10561201914347"></a><a href="修改特殊设置.md">修改特殊设置</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p856191963419"><a name="p856191963419"></a><a name="p856191963419"></a>修改某个流控策略下的某个特殊设置。</p>
</td>
</tr>
<tr id="row4561519123416"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p85611419103415"><a name="p85611419103415"></a><a name="p85611419103415"></a><a href="删除特殊设置.md">删除特殊设置</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p3561201913343"><a name="p3561201913343"></a><a name="p3561201913343"></a>删除某个流控策略的某个特殊配置。</p>
</td>
</tr>
<tr id="row95611319113414"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p1856131923415"><a name="p1856131923415"></a><a name="p1856131923415"></a><a href="查看特殊设置列表.md">查看特殊设置列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p1256151918346"><a name="p1256151918346"></a><a name="p1256151918346"></a>查看给流控策略设置的特殊配置。</p>
</td>
</tr>
</tbody>
</table>

## 概要查询<a name="section45751720133416"></a>

<a name="table1357582017340"></a>
<table><thead align="left"><tr id="row185751620123418"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.3.1.1"><p id="p1857517208345"><a name="p1857517208345"></a><a name="p1857517208345"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="75%" id="mcps1.1.3.1.2"><p id="p18575142073412"><a name="p18575142073412"></a><a name="p18575142073412"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1157617200346"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p1957602018340"><a name="p1957602018340"></a><a name="p1957602018340"></a><a href="查询API分组概况.md">查询API分组概况</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p7576122093419"><a name="p7576122093419"></a><a name="p7576122093419"></a>查询租户名下的API分组概况：上架的API分组个数，未上架的API分组个数。</p>
</td>
</tr>
<tr id="row1657618200349"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p10576182003411"><a name="p10576182003411"></a><a name="p10576182003411"></a><a href="查询API概况.md">查询API概况</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p15576920113410"><a name="p15576920113410"></a><a name="p15576920113410"></a>查询租户名下的API概况：已发布到RELEASE环境的API个数，未发布到RELEASE环境的API个数。</p>
</td>
</tr>
<tr id="row145761920133418"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p7576620163417"><a name="p7576620163417"></a><a name="p7576620163417"></a><a href="查询APP概况.md">查询APP概况</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p125761720193418"><a name="p125761720193418"></a><a name="p125761720193418"></a>查询租户名下的APP概况：已进行API访问授权的APP个数，未进行API访问授权的APP个数。</p>
</td>
</tr>
</tbody>
</table>

## 签名密钥管理<a name="section1264415217349"></a>

<a name="table116441721113419"></a>
<table><thead align="left"><tr id="row1964482110343"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.3.1.1"><p id="p964492103417"><a name="p964492103417"></a><a name="p964492103417"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="75%" id="mcps1.1.3.1.2"><p id="p0644132173414"><a name="p0644132173414"></a><a name="p0644132173414"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1064452183410"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p1164472173414"><a name="p1164472173414"></a><a name="p1164472173414"></a><a href="创建签名密钥.md">创建签名密钥</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p96451421123415"><a name="p96451421123415"></a><a name="p96451421123415"></a>创建一个签名密钥。</p>
<p id="p2573208175714"><a name="p2573208175714"></a><a name="p2573208175714"></a>签名密钥就是API安全保护机制的一种。</p>
</td>
</tr>
<tr id="row2645112118343"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p126456212342"><a name="p126456212342"></a><a name="p126456212342"></a><a href="修改签名密钥.md">修改签名密钥</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p18645102163411"><a name="p18645102163411"></a><a name="p18645102163411"></a>修改指定签名密钥的详细信息。</p>
</td>
</tr>
<tr id="row7645132112341"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p176452021173418"><a name="p176452021173418"></a><a name="p176452021173418"></a><a href="删除签名密钥.md">删除签名密钥</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p9645921173410"><a name="p9645921173410"></a><a name="p9645921173410"></a>删除指定的签名密钥。</p>
</td>
</tr>
<tr id="row12645172114349"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p464516219348"><a name="p464516219348"></a><a name="p464516219348"></a><a href="查询签名密钥列表.md">查询签名密钥列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p3645132183414"><a name="p3645132183414"></a><a name="p3645132183414"></a>查询所有签名密钥的信息。</p>
</td>
</tr>
</tbody>
</table>

## 签名密钥绑定关系管理<a name="section1060611256535"></a>

<a name="table6606925115314"></a>
<table><thead align="left"><tr id="row12606625185313"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.3.1.1"><p id="p1760632511530"><a name="p1760632511530"></a><a name="p1760632511530"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="75%" id="mcps1.1.3.1.2"><p id="p15606142515316"><a name="p15606142515316"></a><a name="p15606142515316"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row460712255538"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p1560762513533"><a name="p1560762513533"></a><a name="p1560762513533"></a><a href="查看签名密钥未绑定的API列表.md">查看签名密钥未绑定的API列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p7607152595311"><a name="p7607152595311"></a><a name="p7607152595311"></a>查询所有未绑定到该签名密钥上的API列表。</p>
</td>
</tr>
<tr id="row1060762575314"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p1607142514536"><a name="p1607142514536"></a><a name="p1607142514536"></a><a href="绑定签名密钥.md">绑定签名密钥</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p5607172515312"><a name="p5607172515312"></a><a name="p5607172515312"></a>将指定的签名密钥绑定到一个或多个已发布的API上。</p>
</td>
</tr>
<tr id="row196074256536"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p160762515316"><a name="p160762515316"></a><a name="p160762515316"></a><a href="查看签名密钥绑定的API列表.md">查看签名密钥绑定的API列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p1860752595316"><a name="p1860752595316"></a><a name="p1860752595316"></a>查询某个签名密钥上已经绑定的API列表。</p>
</td>
</tr>
<tr id="row156074256535"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p19607202514533"><a name="p19607202514533"></a><a name="p19607202514533"></a><a href="查看API绑定的签名密钥列表.md">查看API绑定的签名密钥列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p18608112515311"><a name="p18608112515311"></a><a name="p18608112515311"></a>查询某个API绑定的签名密钥列表。</p>
</td>
</tr>
<tr id="row96081525105316"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p3608425185312"><a name="p3608425185312"></a><a name="p3608425185312"></a><a href="解除绑定API.md">解除绑定</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p460862512531"><a name="p460862512531"></a><a name="p460862512531"></a>解除API与签名密钥的绑定关系。</p>
</td>
</tr>
</tbody>
</table>

## 域名管理<a name="section18754102615315"></a>

<a name="table107541526125316"></a>
<table><thead align="left"><tr id="row167546266534"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.3.1.1"><p id="p4754626135314"><a name="p4754626135314"></a><a name="p4754626135314"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="75%" id="mcps1.1.3.1.2"><p id="p2754102614538"><a name="p2754102614538"></a><a name="p2754102614538"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row475513269534"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p1575572635311"><a name="p1575572635311"></a><a name="p1575572635311"></a><a href="绑定域名.md">绑定域名</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p17755102645312"><a name="p17755102645312"></a><a name="p17755102645312"></a>为API分组绑定域名。</p>
<p id="p166201413141116"><a name="p166201413141116"></a><a name="p166201413141116"></a>绑定域名后，用户可通过自定义域名调用API。</p>
</td>
</tr>
<tr id="row1875512615536"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p16755112685314"><a name="p16755112685314"></a><a name="p16755112685314"></a><a href="解绑域名.md">解绑域名</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p175514260537"><a name="p175514260537"></a><a name="p175514260537"></a>如果API分组不再需要绑定某个自定义域名，则可以为此API分组解绑此域名。</p>
</td>
</tr>
<tr id="row187551826175318"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p3755126195318"><a name="p3755126195318"></a><a name="p3755126195318"></a><a href="绑定域名证书.md">绑定域名证书</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p20755826165310"><a name="p20755826165310"></a><a name="p20755826165310"></a>如果创建API时，“定义API请求”使用HTTPS请求协议，那么在独立域名中需要添加SSL证书。</p>
</td>
</tr>
<tr id="row137554261538"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p575502614530"><a name="p575502614530"></a><a name="p575502614530"></a><a href="删除域名证书.md">删除域名证书</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p147551226195313"><a name="p147551226195313"></a><a name="p147551226195313"></a>如果域名证书不再需要或者已过期，则可以删除证书内容。</p>
</td>
</tr>
</tbody>
</table>

## VPC通道管理<a name="section2938112745315"></a>

<a name="table6938827205310"></a>
<table><thead align="left"><tr id="row7938127195310"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.3.1.1"><p id="p893818274537"><a name="p893818274537"></a><a name="p893818274537"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="75%" id="mcps1.1.3.1.2"><p id="p14938142775316"><a name="p14938142775316"></a><a name="p14938142775316"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row8938122710536"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p16938152712536"><a name="p16938152712536"></a><a name="p16938152712536"></a><a href="创建VPC通道.md">创建VPC通道</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p593812274539"><a name="p593812274539"></a><a name="p593812274539"></a>在API网关中创建连接私有VPC资源的通道。</p>
</td>
</tr>
<tr id="row793813274536"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p79381327175318"><a name="p79381327175318"></a><a name="p79381327175318"></a><a href="更新VPC通道.md">更新VPC通道</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p49394271538"><a name="p49394271538"></a><a name="p49394271538"></a>更新指定VPC通道的参数。</p>
</td>
</tr>
<tr id="row16939127165314"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p1993912765310"><a name="p1993912765310"></a><a name="p1993912765310"></a><a href="删除VPC通道.md">删除VPC通道</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p1493922745310"><a name="p1493922745310"></a><a name="p1493922745310"></a>删除指定的VPC通道。</p>
</td>
</tr>
<tr id="row1693922735318"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p13939162714533"><a name="p13939162714533"></a><a name="p13939162714533"></a><a href="查看VPC通道详情.md">查看VPC通道详情</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p10939152714535"><a name="p10939152714535"></a><a name="p10939152714535"></a>查看指定的VPC通道详情。</p>
</td>
</tr>
<tr id="row9939142711531"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p1293910278531"><a name="p1293910278531"></a><a name="p1293910278531"></a><a href="查看VPC通道列表.md">查看VPC通道列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p4939427175311"><a name="p4939427175311"></a><a name="p4939427175311"></a>查看VPC通道列表。</p>
</td>
</tr>
<tr id="row993982715531"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p14939152710537"><a name="p14939152710537"></a><a name="p14939152710537"></a><a href="添加后端实例（云服务器）.md">添加后端实例（云服务器）</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p693942755311"><a name="p693942755311"></a><a name="p693942755311"></a>为指定的VPC通道添加云服务器。</p>
</td>
</tr>
<tr id="row79391427195314"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p393932712533"><a name="p393932712533"></a><a name="p393932712533"></a><a href="删除后端实例（云服务器）.md">删除后端实例（云服务器）</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p9939327185312"><a name="p9939327185312"></a><a name="p9939327185312"></a>删除指定VPC通道中的云服务器。</p>
</td>
</tr>
<tr id="row3939182715314"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.3.1.1 "><p id="p169401327135317"><a name="p169401327135317"></a><a name="p169401327135317"></a><a href="查看后端实例列表（云服务器列表）.md">查看后端实例列表（云服务器列表）</a></p>
</td>
<td class="cellrowborder" valign="top" width="75%" headers="mcps1.1.3.1.2 "><p id="p1094020274539"><a name="p1094020274539"></a><a name="p1094020274539"></a>查看指定VPC通道的云服务器列表。</p>
</td>
</tr>
</tbody>
</table>

