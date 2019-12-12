# APIG错误码<a name="apig-zh-api-180713213"></a>

通过本文档管理API，发生错误时，产生的错误码如[表1](#table13193435)所示。

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   调用API，发生错误时，产生的错误码请参考[错误码](https://support.huaweicloud.com/ugcall-apig/apig-zh-ug-180530090.html)。  
>-   使用APIG错误码时，请以错误码（如APIG.1000）为准，错误描述信息并非固定不变，有时会对错误描述信息进行优化修改。  

**表 1**  错误码

<a name="table13193435"></a>
<table><thead align="left"><tr id="row65754027"><th class="cellrowborder" valign="top" width="14.93%" id="mcps1.2.4.1.1"><p id="p24475999"><a name="p24475999"></a><a name="p24475999"></a>错误码</p>
</th>
<th class="cellrowborder" valign="top" width="46.07%" id="mcps1.2.4.1.2"><p id="p59154676"><a name="p59154676"></a><a name="p59154676"></a>错误描述（English）</p>
</th>
<th class="cellrowborder" valign="top" width="39%" id="mcps1.2.4.1.3"><p id="p23274785"><a name="p23274785"></a><a name="p23274785"></a>错误描述（中文）</p>
</th>
</tr>
</thead>
<tbody><tr id="row55884709"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p30367563"><a name="p30367563"></a><a name="p30367563"></a>APIG.0000</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p4402438319"><a name="p4402438319"></a><a name="p4402438319"></a>Successful.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p62478654"><a name="p62478654"></a><a name="p62478654"></a>请求成功</p>
</td>
</tr>
<tr id="row13673626"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p33821912"><a name="p33821912"></a><a name="p33821912"></a>APIG.1000</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1963619501133"><a name="p1963619501133"></a><a name="p1963619501133"></a>The token is missing.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p43663746"><a name="p43663746"></a><a name="p43663746"></a>未识别到用户认证信息，请重新登录或稍后重试</p>
</td>
</tr>
<tr id="row57429397"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p21269550"><a name="p21269550"></a><a name="p21269550"></a>APIG.1001</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p196451951135819"><a name="p196451951135819"></a><a name="p196451951135819"></a>The token has expired.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p30189409"><a name="p30189409"></a><a name="p30189409"></a>会话过期，请稍后重试</p>
</td>
</tr>
<tr id="row3269227"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p63480873"><a name="p63480873"></a><a name="p63480873"></a>APIG.1002</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p022649165910"><a name="p022649165910"></a><a name="p022649165910"></a>Incorrect token or token resolution failed.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p20401882"><a name="p20401882"></a><a name="p20401882"></a>认证信息无法识别</p>
</td>
</tr>
<tr id="row49399213"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p41913354"><a name="p41913354"></a><a name="p41913354"></a>APIG.1003</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1874975010594"><a name="p1874975010594"></a><a name="p1874975010594"></a>The token does not contain project information.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p48502156"><a name="p48502156"></a><a name="p48502156"></a>认证不包含租户信息</p>
</td>
</tr>
<tr id="row33866226"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p58809751"><a name="p58809751"></a><a name="p58809751"></a>APIG.1004</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p194211512908"><a name="p194211512908"></a><a name="p194211512908"></a>The token does not contain domain information.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p04511953173610"><a name="p04511953173610"></a><a name="p04511953173610"></a>认证不包含Domain信息</p>
</td>
</tr>
<tr id="row41723287"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p24143071"><a name="p24143071"></a><a name="p24143071"></a>APIG.1005</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p6941142162110"><a name="p6941142162110"></a><a name="p6941142162110"></a>No permissions to request this method.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p4202162833913"><a name="p4202162833913"></a><a name="p4202162833913"></a>租户操作受限，请前往用户中心核实</p>
</td>
</tr>
<tr id="row30613636"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p63785465"><a name="p63785465"></a><a name="p63785465"></a>APIG.1006</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p66349026"><a name="p66349026"></a><a name="p66349026"></a>The project information is missing.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p9265152104718"><a name="p9265152104718"></a><a name="p9265152104718"></a>认证不包含租户信息</p>
</td>
</tr>
<tr id="row50058217"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p28183748"><a name="p28183748"></a><a name="p28183748"></a>APIG.1007</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1327535411"><a name="p1327535411"></a><a name="p1327535411"></a>The domain information is missing.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p177268397471"><a name="p177268397471"></a><a name="p177268397471"></a>认证不包含Domain信息</p>
</td>
</tr>
<tr id="row56558587"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p17842855"><a name="p17842855"></a><a name="p17842855"></a>APIG.1008</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p58423186118"><a name="p58423186118"></a><a name="p58423186118"></a>Unknown domain.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p29118797"><a name="p29118797"></a><a name="p29118797"></a>无法识别用户Domain信息</p>
</td>
</tr>
<tr id="row22981276495"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p72981977490"><a name="p72981977490"></a><a name="p72981977490"></a>APIG.1009</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1034412911493"><a name="p1034412911493"></a><a name="p1034412911493"></a>The token does not contain user information.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1529811717492"><a name="p1529811717492"></a><a name="p1529811717492"></a>认证不包含用户信息</p>
</td>
</tr>
<tr id="row661814126574"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1861817126572"><a name="p1861817126572"></a><a name="p1861817126572"></a>APIG.1010</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p19619141219571"><a name="p19619141219571"></a><a name="p19619141219571"></a>PDP server connection failed.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p2061971235720"><a name="p2061971235720"></a><a name="p2061971235720"></a>连接细粒度授权服务器失败</p>
</td>
</tr>
<tr id="row15180135915193"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p026310181694"><a name="p026310181694"></a><a name="p026310181694"></a>APIG.1011</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1626315185917"><a name="p1626315185917"></a><a name="p1626315185917"></a>You can request resources only after you complete real-name authentication.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p72639183910"><a name="p72639183910"></a><a name="p72639183910"></a>您的账号未实名认证，暂时无法进行其他操作</p>
</td>
</tr>
<tr id="row9935813206"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p128049203915"><a name="p128049203915"></a><a name="p128049203915"></a>APIG.1012</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p14804520497"><a name="p14804520497"></a><a name="p14804520497"></a>Your account balance is insufficient. Top up your account.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1580417201593"><a name="p1580417201593"></a><a name="p1580417201593"></a>您的账户余额不足，请前往用户中心解决</p>
</td>
</tr>
<tr id="row1683916412205"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p6625182317913"><a name="p6625182317913"></a><a name="p6625182317913"></a>APIG.1013</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1662514234913"><a name="p1662514234913"></a><a name="p1662514234913"></a>Your account has been frozen. Some functions become unavailable. To unfreeze your account, contact customer service at 4000-955-988.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1662515231598"><a name="p1662515231598"></a><a name="p1662515231598"></a>您的账户已被冻结，部分功能会受到影响，请联系客服4000-955-988解除</p>
</td>
</tr>
<tr id="row4305583"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p13207931"><a name="p13207931"></a><a name="p13207931"></a>APIG.1101</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1194162722"><a name="p1194162722"></a><a name="p1194162722"></a>No permissions to perform operations on this API group.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p19691879"><a name="p19691879"></a><a name="p19691879"></a>没有权限操作该API分组</p>
</td>
</tr>
<tr id="row43009190"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p61192352"><a name="p61192352"></a><a name="p61192352"></a>APIG.1102</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1113052275"><a name="p1113052275"></a><a name="p1113052275"></a>No permissions to perform operations on this API.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p37801855"><a name="p37801855"></a><a name="p37801855"></a>没有权限操作该API</p>
</td>
</tr>
<tr id="row4672375"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p42918090"><a name="p42918090"></a><a name="p42918090"></a>APIG.1103</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p145281643323"><a name="p145281643323"></a><a name="p145281643323"></a>No permissions to perform operations on this environment.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p63907918"><a name="p63907918"></a><a name="p63907918"></a>没有权限操作该环境</p>
</td>
</tr>
<tr id="row38300353"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p15320903"><a name="p15320903"></a><a name="p15320903"></a>APIG.1104</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p59663633"><a name="p59663633"></a><a name="p59663633"></a>No permissions to perform operations on this app.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p58478980"><a name="p58478980"></a><a name="p58478980"></a>没有权限操作该应用</p>
</td>
</tr>
<tr id="row56548780"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p17048430"><a name="p17048430"></a><a name="p17048430"></a>APIG.1105</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p4775162311814"><a name="p4775162311814"></a><a name="p4775162311814"></a>No permissions to perform operations on this request throttling policy.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p51386329"><a name="p51386329"></a><a name="p51386329"></a>没有权限操作该流控策略</p>
</td>
</tr>
<tr id="row59823781"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p13888094"><a name="p13888094"></a><a name="p13888094"></a>APIG.1106</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p104963401636"><a name="p104963401636"></a><a name="p104963401636"></a>No permissions to perform operations on this access control policy.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p53062347"><a name="p53062347"></a><a name="p53062347"></a>没有权限操作该ACL策略</p>
</td>
</tr>
<tr id="row7799077"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p27745471"><a name="p27745471"></a><a name="p27745471"></a>APIG.1107</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p649701341"><a name="p649701341"></a><a name="p649701341"></a>No permissions to perform operations on this configuration.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p38797921"><a name="p38797921"></a><a name="p38797921"></a>没有权限操作该配置信息</p>
</td>
</tr>
<tr id="row13636969"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p30852734"><a name="p30852734"></a><a name="p30852734"></a>APIG.1108</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1817019481345"><a name="p1817019481345"></a><a name="p1817019481345"></a>No permissions to perform operations on this excluded configuration.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p24458986"><a name="p24458986"></a><a name="p24458986"></a>没有权限操作该特殊配置信息</p>
</td>
</tr>
<tr id="row18804282"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p46751892"><a name="p46751892"></a><a name="p46751892"></a>APIG.1109</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p380313820519"><a name="p380313820519"></a><a name="p380313820519"></a>No permissions to perform operations on this app authorization record.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p51657405"><a name="p51657405"></a><a name="p51657405"></a>没有权限操作该APP授权信息</p>
</td>
</tr>
<tr id="row62263462"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p10175679"><a name="p10175679"></a><a name="p10175679"></a>APIG.1110</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p194452037268"><a name="p194452037268"></a><a name="p194452037268"></a>No permissions to perform operations on this environment variable.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p56419833"><a name="p56419833"></a><a name="p56419833"></a>没有权限操作该环境变量</p>
</td>
</tr>
<tr id="row38016452"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p59433797"><a name="p59433797"></a><a name="p59433797"></a>APIG.1111</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p49408291"><a name="p49408291"></a><a name="p49408291"></a>No permissions to perform operations on this subscription record.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p42648645"><a name="p42648645"></a><a name="p42648645"></a>没有权限操作该订购信息</p>
</td>
</tr>
<tr id="row267255926"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p4672551625"><a name="p4672551625"></a><a name="p4672551625"></a>APIG.1112</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p171615432043"><a name="p171615432043"></a><a name="p171615432043"></a>No permissions to perform operations on this signature key.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p156721451729"><a name="p156721451729"></a><a name="p156721451729"></a>没有权限操作该签名密钥</p>
</td>
</tr>
<tr id="row178956816519"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p128951288516"><a name="p128951288516"></a><a name="p128951288516"></a>APIG.1113</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1533864818312"><a name="p1533864818312"></a><a name="p1533864818312"></a>No permissions to perform operations on this VPC channel.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1389510845118"><a name="p1389510845118"></a><a name="p1389510845118"></a>没有权限操作该VPC通道</p>
</td>
</tr>
<tr id="row19103314161512"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p3104141471518"><a name="p3104141471518"></a><a name="p3104141471518"></a>APIG.1114</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p430819511229"><a name="p430819511229"></a><a name="p430819511229"></a>No permissions to perform operations on this AZ.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1761864232013"><a name="p1761864232013"></a><a name="p1761864232013"></a>没有权限操作该业务区</p>
</td>
</tr>
<tr id="row96841177158"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p36856174153"><a name="p36856174153"></a><a name="p36856174153"></a>APIG.1115</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p166851517171519"><a name="p166851517171519"></a><a name="p166851517171519"></a>No permissions to perform operations on this certificate.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p14685217201513"><a name="p14685217201513"></a><a name="p14685217201513"></a>没有权限操作该证书</p>
</td>
</tr>
<tr id="row119264613522"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p199214675217"><a name="p199214675217"></a><a name="p199214675217"></a>APIG.1116</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1317082817229"><a name="p1317082817229"></a><a name="p1317082817229"></a>No permissions to perform operations on this on-sale API.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p7119196201013"><a name="p7119196201013"></a><a name="p7119196201013"></a>没有权限操作该上架中的API</p>
</td>
</tr>
<tr id="row410795025213"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p17107450185219"><a name="p17107450185219"></a><a name="p17107450185219"></a>APIG.1117</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p4107175075211"><a name="p4107175075211"></a><a name="p4107175075211"></a>No permissions to perform operations on this BI reporting record.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p20107150125218"><a name="p20107150125218"></a><a name="p20107150125218"></a>没有权限操作BI上报记录</p>
</td>
</tr>
<tr id="row1855232514588"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1055316254585"><a name="p1055316254585"></a><a name="p1055316254585"></a>APIG.1119</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p11553112519585"><a name="p11553112519585"></a><a name="p11553112519585"></a>No permissions to perform operations on this method.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1155317251584"><a name="p1155317251584"></a><a name="p1155317251584"></a>细粒度授权失败，无权限执行此操作</p>
</td>
</tr>
<tr id="row3922191253413"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p20922101217340"><a name="p20922101217340"></a><a name="p20922101217340"></a>APIG.1120</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p149231812183410"><a name="p149231812183410"></a><a name="p149231812183410"></a>No permissions to create ELB channels.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p492312121342"><a name="p492312121342"></a><a name="p492312121342"></a>没有权限创建私网ELB通道</p>
</td>
</tr>
<tr id="row48511259"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p37097900"><a name="p37097900"></a><a name="p37097900"></a>APIG.1201</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p154900450614"><a name="p154900450614"></a><a name="p154900450614"></a>The resources belong to different tenants.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p62581458"><a name="p62581458"></a><a name="p62581458"></a>操作的资源不属于同一租户</p>
</td>
</tr>
<tr id="row34341398"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p30189854"><a name="p30189854"></a><a name="p30189854"></a>APIG.2000</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p29459123"><a name="p29459123"></a><a name="p29459123"></a>Parameter error.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p37378748"><a name="p37378748"></a><a name="p37378748"></a>请求参数错误</p>
</td>
</tr>
<tr id="row864416"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p2908851"><a name="p2908851"></a><a name="p2908851"></a>APIG.2001</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p34290350"><a name="p34290350"></a><a name="p34290350"></a>The request parameters must be specified.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p15170114115175"><a name="p15170114115175"></a><a name="p15170114115175"></a>请求参数为空</p>
</td>
</tr>
<tr id="row33168142"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p2264949"><a name="p2264949"></a><a name="p2264949"></a>APIG.2002</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p135674351274"><a name="p135674351274"></a><a name="p135674351274"></a>The parameter value is too small.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p29276378"><a name="p29276378"></a><a name="p29276378"></a>参数值小于最小值</p>
</td>
</tr>
<tr id="row62160815"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1861221"><a name="p1861221"></a><a name="p1861221"></a>APIG.2003</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p16541212"><a name="p16541212"></a><a name="p16541212"></a>The parameter value is too large.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p64769787"><a name="p64769787"></a><a name="p64769787"></a>参数值大于最大值</p>
</td>
</tr>
<tr id="row46057178"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p39643913"><a name="p39643913"></a><a name="p39643913"></a>APIG.2004</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1457335417720"><a name="p1457335417720"></a><a name="p1457335417720"></a>The parameter value is outside the allowable range.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p56867461"><a name="p56867461"></a><a name="p56867461"></a>参数值不在可选范围内</p>
</td>
</tr>
<tr id="row42045102"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p50210096"><a name="p50210096"></a><a name="p50210096"></a>APIG.2005</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p18253813816"><a name="p18253813816"></a><a name="p18253813816"></a>The parameter is too short.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p58137509"><a name="p58137509"></a><a name="p58137509"></a>参数长度太短</p>
</td>
</tr>
<tr id="row53475538"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p36551345"><a name="p36551345"></a><a name="p36551345"></a>APIG.2006</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p77519166818"><a name="p77519166818"></a><a name="p77519166818"></a>The parameter is too long.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p33406356"><a name="p33406356"></a><a name="p33406356"></a>参数长度太长</p>
</td>
</tr>
<tr id="row32221750"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p59824939"><a name="p59824939"></a><a name="p59824939"></a>APIG.2007</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p13981905"><a name="p13981905"></a><a name="p13981905"></a>Invalid length.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p58792527"><a name="p58792527"></a><a name="p58792527"></a>参数长度非法</p>
</td>
</tr>
<tr id="row59370703"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p44297670"><a name="p44297670"></a><a name="p44297670"></a>APIG.2008</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p31341480"><a name="p31341480"></a><a name="p31341480"></a>Only letters are allowed.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p55631967"><a name="p55631967"></a><a name="p55631967"></a>参数只能是字母</p>
</td>
</tr>
<tr id="row30925662"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p21950703"><a name="p21950703"></a><a name="p21950703"></a>APIG.2009</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p197331437299"><a name="p197331437299"></a><a name="p197331437299"></a>Only digits are allowed.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p2943634"><a name="p2943634"></a><a name="p2943634"></a>参数只能是数字</p>
</td>
</tr>
<tr id="row26492713"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p65535007"><a name="p65535007"></a><a name="p65535007"></a>APIG.2010</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p8699204614913"><a name="p8699204614913"></a><a name="p8699204614913"></a>Only letters and digits are allowed.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p8690111"><a name="p8690111"></a><a name="p8690111"></a>参数只能是字母或数字</p>
</td>
</tr>
<tr id="row11102143"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p26858387"><a name="p26858387"></a><a name="p26858387"></a>APIG.2011</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p9920105616912"><a name="p9920105616912"></a><a name="p9920105616912"></a>Invalid parameter value.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p57114758"><a name="p57114758"></a><a name="p57114758"></a>参数规则不匹配</p>
</td>
</tr>
<tr id="row44270775"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p29163028"><a name="p29163028"></a><a name="p29163028"></a>APIG.2012</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p12546161414107"><a name="p12546161414107"></a><a name="p12546161414107"></a>Invalid parameter value.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p11260172"><a name="p11260172"></a><a name="p11260172"></a>参数匹配到不期望匹配的规则</p>
</td>
</tr>
<tr id="row34232688"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p21384368"><a name="p21384368"></a><a name="p21384368"></a>APIG.2013</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p54412265"><a name="p54412265"></a><a name="p54412265"></a>Only letters, digits, hyphens (-), and underscores (_) are allowed.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p45317314"><a name="p45317314"></a><a name="p45317314"></a>参数只能是字母、数字、下划线或中划线</p>
</td>
</tr>
<tr id="row5202642"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p18760830"><a name="p18760830"></a><a name="p18760830"></a>APIG.2014</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p208034412109"><a name="p208034412109"></a><a name="p208034412109"></a>Invalid email address.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p12154397"><a name="p12154397"></a><a name="p12154397"></a>无效的邮件地址</p>
</td>
</tr>
<tr id="row42280714"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p2185822"><a name="p2185822"></a><a name="p2185822"></a>APIG.2015</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p42833857"><a name="p42833857"></a><a name="p42833857"></a>Invalid IP address.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p46990430"><a name="p46990430"></a><a name="p46990430"></a>无效的IP地址</p>
</td>
</tr>
<tr id="row20260689"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p30503093"><a name="p30503093"></a><a name="p30503093"></a>APIG.2016</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p123113195114"><a name="p123113195114"></a><a name="p123113195114"></a>The characters are not encoded using Base64.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p12163403"><a name="p12163403"></a><a name="p12163403"></a>不是base64编码的字符</p>
</td>
</tr>
<tr id="row42361764"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p8750899"><a name="p8750899"></a><a name="p8750899"></a>APIG.2017</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p17188142712115"><a name="p17188142712115"></a><a name="p17188142712115"></a>Invalid mobile number.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p36575475"><a name="p36575475"></a><a name="p36575475"></a>无效的手机号码</p>
</td>
</tr>
<tr id="row60743820"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p21302416"><a name="p21302416"></a><a name="p21302416"></a>APIG.2018</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p47774136"><a name="p47774136"></a><a name="p47774136"></a>Invalid telephone number.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p44499821"><a name="p44499821"></a><a name="p44499821"></a>无效的固话号码</p>
</td>
</tr>
<tr id="row64954071"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p26788426"><a name="p26788426"></a><a name="p26788426"></a>APIG.2019</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p22378877"><a name="p22378877"></a><a name="p22378877"></a>Invalid telephone or mobile number.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p749720"><a name="p749720"></a><a name="p749720"></a>无效的电话号码</p>
</td>
</tr>
<tr id="row6747484"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p9675368"><a name="p9675368"></a><a name="p9675368"></a>APIG.2020</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p6793820181212"><a name="p6793820181212"></a><a name="p6793820181212"></a>Invalid postal code.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p62213595"><a name="p62213595"></a><a name="p62213595"></a>无效的邮政编码</p>
</td>
</tr>
<tr id="row23051451"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p55228217"><a name="p55228217"></a><a name="p55228217"></a>APIG.2021</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p44300559"><a name="p44300559"></a><a name="p44300559"></a>The URL domain is not included in the IP address whitelist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p31575526"><a name="p31575526"></a><a name="p31575526"></a>域名不在允许的白名单内</p>
</td>
</tr>
<tr id="row36427018456"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1064211016457"><a name="p1064211016457"></a><a name="p1064211016457"></a>APIG.2022</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p011504671211"><a name="p011504671211"></a><a name="p011504671211"></a>The URL domain is included in the IP address blacklist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p86429016450"><a name="p86429016450"></a><a name="p86429016450"></a>域名处于禁止的黑名单内</p>
</td>
</tr>
<tr id="row15774163925416"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p77748397546"><a name="p77748397546"></a><a name="p77748397546"></a>APIG.2023</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1593345861210"><a name="p1593345861210"></a><a name="p1593345861210"></a>URL domain CNAME resolution failed.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1077414395544"><a name="p1077414395544"></a><a name="p1077414395544"></a>域名cname失败</p>
</td>
</tr>
<tr id="row199751949113514"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p16975349203517"><a name="p16975349203517"></a><a name="p16975349203517"></a>APIG.2024</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p194932842317"><a name="p194932842317"></a><a name="p194932842317"></a>Invalid URL domain.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p197574963516"><a name="p197574963516"></a><a name="p197574963516"></a>域名非法</p>
</td>
</tr>
<tr id="row19677234195219"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1567713416527"><a name="p1567713416527"></a><a name="p1567713416527"></a>APIG.2025</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p18328182210137"><a name="p18328182210137"></a><a name="p18328182210137"></a>Invalid backend port number.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1667733413521"><a name="p1667733413521"></a><a name="p1667733413521"></a>无效的端口号</p>
</td>
</tr>
<tr id="row1380419107174"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p580541013171"><a name="p580541013171"></a><a name="p580541013171"></a>APIG.2026</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p08051103170"><a name="p08051103170"></a><a name="p08051103170"></a>The request path parameters do not match the request URI.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p14805181018173"><a name="p14805181018173"></a><a name="p14805181018173"></a>请求的路径参数未在请求路径中定义</p>
</td>
</tr>
<tr id="row21259135176"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1212591371710"><a name="p1212591371710"></a><a name="p1212591371710"></a>APIG.2027</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p10657450171312"><a name="p10657450171312"></a><a name="p10657450171312"></a>The backend path parameters do not match the backend URI.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p131251313101716"><a name="p131251313101716"></a><a name="p131251313101716"></a>后端的路径参数未在后端路径中定义</p>
</td>
</tr>
<tr id="row832018169176"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p33201116161710"><a name="p33201116161710"></a><a name="p33201116161710"></a>APIG.2028</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p109005321414"><a name="p109005321414"></a><a name="p109005321414"></a>The backend parameters are not mapped to the request parameters.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p16320916131714"><a name="p16320916131714"></a><a name="p16320916131714"></a>后端参数映射的请求参数未定义</p>
</td>
</tr>
<tr id="row830320141710"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p7301920201712"><a name="p7301920201712"></a><a name="p7301920201712"></a>APIG.2029</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p15828420111418"><a name="p15828420111418"></a><a name="p15828420111418"></a>The default certificate already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p11301520101711"><a name="p11301520101711"></a><a name="p11301520101711"></a>默认证书已存在</p>
</td>
</tr>
<tr id="row5517183925314"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p151783913536"><a name="p151783913536"></a><a name="p151783913536"></a>APIG.2030</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p637554619236"><a name="p637554619236"></a><a name="p637554619236"></a>Bad request for debugging the API.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p451713919536"><a name="p451713919536"></a><a name="p451713919536"></a>调试API请求消息不合法</p>
</td>
</tr>
<tr id="row1827134824914"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1528184814918"><a name="p1528184814918"></a><a name="p1528184814918"></a>APIG.2034</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1528124874914"><a name="p1528124874914"></a><a name="p1528124874914"></a>The domain name has not been filed. File it first.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p9281048204914"><a name="p9281048204914"></a><a name="p9281048204914"></a>域名未备案，请进入备案系统进行备案</p>
</td>
</tr>
<tr id="row1279775212499"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1879718523498"><a name="p1879718523498"></a><a name="p1879718523498"></a>APIG.2035</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p0797155274912"><a name="p0797155274912"></a><a name="p0797155274912"></a>The ICP Filing System is busy. Please try again later.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p17797205215496"><a name="p17797205215496"></a><a name="p17797205215496"></a>备案系统繁忙，请稍后重试</p>
</td>
</tr>
<tr id="row65730529358"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p4573652203511"><a name="p4573652203511"></a><a name="p4573652203511"></a>APIG.2101</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p79031534111419"><a name="p79031534111419"></a><a name="p79031534111419"></a>The certificate and private key do not match.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p135733522359"><a name="p135733522359"></a><a name="p135733522359"></a>证书与私钥不匹配</p>
</td>
</tr>
<tr id="row9581657143613"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1459195793612"><a name="p1459195793612"></a><a name="p1459195793612"></a>APIG.2102</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p18262947153212"><a name="p18262947153212"></a><a name="p18262947153212"></a>The certificate has expired.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p35916571362"><a name="p35916571362"></a><a name="p35916571362"></a>证书过期</p>
</td>
</tr>
<tr id="row71088023710"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1610800123719"><a name="p1610800123719"></a><a name="p1610800123719"></a>APIG.2103</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p71499712153"><a name="p71499712153"></a><a name="p71499712153"></a>The certificate common name does not match the domain name.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1810817043716"><a name="p1810817043716"></a><a name="p1810817043716"></a>证书内域名与自定义域名不匹配</p>
</td>
</tr>
<tr id="row11631192103716"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p7631523379"><a name="p7631523379"></a><a name="p7631523379"></a>APIG.2104</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1865462212153"><a name="p1865462212153"></a><a name="p1865462212153"></a>The certificate chain is not matched.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p116316213710"><a name="p116316213710"></a><a name="p116316213710"></a>证书链不匹配</p>
</td>
</tr>
<tr id="row1717105133714"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p717253378"><a name="p717253378"></a><a name="p717253378"></a>APIG.2105</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p8788326181618"><a name="p8788326181618"></a><a name="p8788326181618"></a>Encrypted private keys are not supported.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p13178511379"><a name="p13178511379"></a><a name="p13178511379"></a>不支持加密的私钥</p>
</td>
</tr>
<tr id="row199251717373"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p89261476375"><a name="p89261476375"></a><a name="p89261476375"></a>APIG.2106</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p7143541121614"><a name="p7143541121614"></a><a name="p7143541121614"></a>Invalid certificate or private key.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p5926372373"><a name="p5926372373"></a><a name="p5926372373"></a>无效的证书或私钥</p>
</td>
</tr>
<tr id="row1411214221265"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p11121522142615"><a name="p11121522142615"></a><a name="p11121522142615"></a>APIG.2107</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p811214221267"><a name="p811214221267"></a><a name="p811214221267"></a>The default zone is invalid.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p611242211264"><a name="p611242211264"></a><a name="p611242211264"></a>默认集群非法</p>
</td>
</tr>
<tr id="row10702311"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p61580824"><a name="p61580824"></a><a name="p61580824"></a>APIG.3001</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1912041181716"><a name="p1912041181716"></a><a name="p1912041181716"></a>The API group does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p36427764"><a name="p36427764"></a><a name="p36427764"></a>指定的API分组不存在</p>
</td>
</tr>
<tr id="row59414426"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p47839212"><a name="p47839212"></a><a name="p47839212"></a>APIG.3002</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p16477115371716"><a name="p16477115371716"></a><a name="p16477115371716"></a>The API does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p4918142"><a name="p4918142"></a><a name="p4918142"></a>指定的API不存在</p>
</td>
</tr>
<tr id="row44263283"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p28556160"><a name="p28556160"></a><a name="p28556160"></a>APIG.3003</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p15529131171816"><a name="p15529131171816"></a><a name="p15529131171816"></a>The environment does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p56128091"><a name="p56128091"></a><a name="p56128091"></a>指定的环境不存在</p>
</td>
</tr>
<tr id="row35390776"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p48080585"><a name="p48080585"></a><a name="p48080585"></a>APIG.3004</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p10751410181810"><a name="p10751410181810"></a><a name="p10751410181810"></a>The app does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p45063138"><a name="p45063138"></a><a name="p45063138"></a>指定的应用不存在</p>
</td>
</tr>
<tr id="row2915064"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p34793608"><a name="p34793608"></a><a name="p34793608"></a>APIG.3005</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p751612012184"><a name="p751612012184"></a><a name="p751612012184"></a>The request throttling policy does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p43619634"><a name="p43619634"></a><a name="p43619634"></a>指定的流控策略不存在</p>
</td>
</tr>
<tr id="row57032394"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p56221187"><a name="p56221187"></a><a name="p56221187"></a>APIG.3006</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p7761193651810"><a name="p7761193651810"></a><a name="p7761193651810"></a>The access control policy does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p36894451"><a name="p36894451"></a><a name="p36894451"></a>指定的ACL策略不存在</p>
</td>
</tr>
<tr id="row63614605"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p52509385"><a name="p52509385"></a><a name="p52509385"></a>APIG.3007</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p176264841815"><a name="p176264841815"></a><a name="p176264841815"></a>The configuration does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p44279058"><a name="p44279058"></a><a name="p44279058"></a>指定的配置不存在</p>
</td>
</tr>
<tr id="row62967208"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p70257"><a name="p70257"></a><a name="p70257"></a>APIG.3008</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p5690862"><a name="p5690862"></a><a name="p5690862"></a>The excluded configuration does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p58306696"><a name="p58306696"></a><a name="p58306696"></a>指定的特殊配置不存在</p>
</td>
</tr>
<tr id="row54998219"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p25670746"><a name="p25670746"></a><a name="p25670746"></a>APIG.3009</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1491701820191"><a name="p1491701820191"></a><a name="p1491701820191"></a>The app authorization record does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p49629971"><a name="p49629971"></a><a name="p49629971"></a>指定的APP授权信息不存在</p>
</td>
</tr>
<tr id="row44016556"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p8571244"><a name="p8571244"></a><a name="p8571244"></a>APIG.3010</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p0120193331919"><a name="p0120193331919"></a><a name="p0120193331919"></a>The access control policy binding record does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p65813753"><a name="p65813753"></a><a name="p65813753"></a>指定的ACL策略绑定记录不存在</p>
</td>
</tr>
<tr id="row55452873"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p62497748"><a name="p62497748"></a><a name="p62497748"></a>APIG.3011</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p432644517197"><a name="p432644517197"></a><a name="p432644517197"></a>The environment variable does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p12569803"><a name="p12569803"></a><a name="p12569803"></a>指定的环境变量不存在</p>
</td>
</tr>
<tr id="row46019371"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p36581579"><a name="p36581579"></a><a name="p36581579"></a>APIG.3012</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1289195541916"><a name="p1289195541916"></a><a name="p1289195541916"></a>The request throttling policy binding record does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p30443808"><a name="p30443808"></a><a name="p30443808"></a>指定的流控策略绑定记录不存在</p>
</td>
</tr>
<tr id="row5558816"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p47610958"><a name="p47610958"></a><a name="p47610958"></a>APIG.3013</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p185081516182012"><a name="p185081516182012"></a><a name="p185081516182012"></a>The excluded request throttling configuration does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p50848853"><a name="p50848853"></a><a name="p50848853"></a>指定的流控策略特殊配置不存在</p>
</td>
</tr>
<tr id="row54986495"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p24721126"><a name="p24721126"></a><a name="p24721126"></a>APIG.3014</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p7730132642013"><a name="p7730132642013"></a><a name="p7730132642013"></a>The pre-subscription record does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p60297810"><a name="p60297810"></a><a name="p60297810"></a>指定的订购信息不存在</p>
</td>
</tr>
<tr id="row5809383"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p798049"><a name="p798049"></a><a name="p798049"></a>APIG.3015</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p64642036"><a name="p64642036"></a><a name="p64642036"></a>The API publication record does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1513543"><a name="p1513543"></a><a name="p1513543"></a>指定的API发布记录不存在</p>
</td>
</tr>
<tr id="row13621888"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p29631126"><a name="p29631126"></a><a name="p29631126"></a>APIG.3016</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1034914506207"><a name="p1034914506207"></a><a name="p1034914506207"></a>The API group listing information does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p62553705"><a name="p62553705"></a><a name="p62553705"></a>指定的API分组上架信息不存在</p>
</td>
</tr>
<tr id="row46312121079"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1263912576"><a name="p1263912576"></a><a name="p1263912576"></a>APIG.3017</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p13644166182114"><a name="p13644166182114"></a><a name="p13644166182114"></a>The signature key does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p96321216714"><a name="p96321216714"></a><a name="p96321216714"></a>指定的签名密钥不存在</p>
</td>
</tr>
<tr id="row53601991173"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p16360395720"><a name="p16360395720"></a><a name="p16360395720"></a>APIG.3018</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p4360595718"><a name="p4360595718"></a><a name="p4360595718"></a>The signature key binding record does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p183601491572"><a name="p183601491572"></a><a name="p183601491572"></a>指定的签名密钥绑定记录不存在</p>
</td>
</tr>
<tr id="row15786719282"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p178619117289"><a name="p178619117289"></a><a name="p178619117289"></a>APIG.3019</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p162312432214"><a name="p162312432214"></a><a name="p162312432214"></a>The function URN does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p47861112287"><a name="p47861112287"></a><a name="p47861112287"></a>指定的函数URN不存在</p>
</td>
</tr>
<tr id="row3100205014315"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p8100125018316"><a name="p8100125018316"></a><a name="p8100125018316"></a>APIG.3020</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p22161656132115"><a name="p22161656132115"></a><a name="p22161656132115"></a>The URL domain does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p12100105093118"><a name="p12100105093118"></a><a name="p12100105093118"></a>指定的域名不存在</p>
</td>
</tr>
<tr id="row523485433118"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p223416542313"><a name="p223416542313"></a><a name="p223416542313"></a>APIG.3021</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p10550153116224"><a name="p10550153116224"></a><a name="p10550153116224"></a>The SSL certificate does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p62341854183112"><a name="p62341854183112"></a><a name="p62341854183112"></a>指定的证书不存在</p>
</td>
</tr>
<tr id="row144371557183111"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1743718577312"><a name="p1743718577312"></a><a name="p1743718577312"></a>APIG.3022</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p18822941192212"><a name="p18822941192212"></a><a name="p18822941192212"></a>The API version does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1743711577314"><a name="p1743711577314"></a><a name="p1743711577314"></a>指定的API历史版本不存在</p>
</td>
</tr>
<tr id="row04071836175415"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p17407133685416"><a name="p17407133685416"></a><a name="p17407133685416"></a>APIG.3023</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p6407103616548"><a name="p6407103616548"></a><a name="p6407103616548"></a>The VPC channel does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1740717360547"><a name="p1740717360547"></a><a name="p1740717360547"></a>指定的VPC通道不存在</p>
</td>
</tr>
<tr id="row14814133912547"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p13814183919547"><a name="p13814183919547"></a><a name="p13814183919547"></a>APIG.3024</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p204961611233"><a name="p204961611233"></a><a name="p204961611233"></a>The instance does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p17814193912545"><a name="p17814193912545"></a><a name="p17814193912545"></a>指定的云主机不存在</p>
</td>
</tr>
<tr id="row19790153716287"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p679053712815"><a name="p679053712815"></a><a name="p679053712815"></a>APIG.3025</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p109356811236"><a name="p109356811236"></a><a name="p109356811236"></a>The certificate does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p20790163702819"><a name="p20790163702819"></a><a name="p20790163702819"></a>指定的证书不存在</p>
</td>
</tr>
<tr id="row14550177183016"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1755011743011"><a name="p1755011743011"></a><a name="p1755011743011"></a>APIG.3026</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p55508793020"><a name="p55508793020"></a><a name="p55508793020"></a>The cluster host does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p85503714301"><a name="p85503714301"></a><a name="p85503714301"></a>指定的集群主机不存在</p>
</td>
</tr>
<tr id="row38835411307"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p488416417309"><a name="p488416417309"></a><a name="p488416417309"></a>APIG.3027</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p14856202913234"><a name="p14856202913234"></a><a name="p14856202913234"></a>The zone does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p148841645303"><a name="p148841645303"></a><a name="p148841645303"></a>指定的集群不存在</p>
</td>
</tr>
<tr id="row177853403546"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1785144016541"><a name="p1785144016541"></a><a name="p1785144016541"></a>APIG.3028</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p10785124014544"><a name="p10785124014544"></a><a name="p10785124014544"></a>The DNS has not been configured in the AZ.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p15785124017541"><a name="p15785124017541"></a><a name="p15785124017541"></a>业务区中的DNS未配置</p>
</td>
</tr>
<tr id="row10860243151219"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p9860204331212"><a name="p9860204331212"></a><a name="p9860204331212"></a>APIG.3029</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p27203213245"><a name="p27203213245"></a><a name="p27203213245"></a>The user does not exist in the AZ.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p386044317123"><a name="p386044317123"></a><a name="p386044317123"></a>业务区中不存在该用户</p>
</td>
</tr>
<tr id="row25309573"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p36809523"><a name="p36809523"></a><a name="p36809523"></a>APIG.3100</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1854185532414"><a name="p1854185532414"></a><a name="p1854185532414"></a>The number of resources exceeds the maximum allowed limit.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p49591229"><a name="p49591229"></a><a name="p49591229"></a>请求的资源数量超过限额</p>
</td>
</tr>
<tr id="row43667880"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p47437361"><a name="p47437361"></a><a name="p47437361"></a>APIG.3101</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p376715672519"><a name="p376715672519"></a><a name="p376715672519"></a>The number of API groups exceeds the maximum allowed limit.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p52723268"><a name="p52723268"></a><a name="p52723268"></a>API分组数量超过限额</p>
</td>
</tr>
<tr id="row4747366"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p48992404"><a name="p48992404"></a><a name="p48992404"></a>APIG.3102</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p941391319254"><a name="p941391319254"></a><a name="p941391319254"></a>The number of APIs exceeds the maximum allowed limit.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p54817061"><a name="p54817061"></a><a name="p54817061"></a>API数量超过限额</p>
</td>
</tr>
<tr id="row23591504"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p31863709"><a name="p31863709"></a><a name="p31863709"></a>APIG.3103</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p181262903113"><a name="p181262903113"></a><a name="p181262903113"></a>The number of apps exceeds the maximum allowed limit.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p13685759"><a name="p13685759"></a><a name="p13685759"></a>应用数量超过限额</p>
</td>
</tr>
<tr id="row126020745513"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1360277195512"><a name="p1360277195512"></a><a name="p1360277195512"></a>APIG.3104</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p18250104217258"><a name="p18250104217258"></a><a name="p18250104217258"></a>The number of environments exceeds the maximum allowed limit.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p26021072556"><a name="p26021072556"></a><a name="p26021072556"></a>环境数量超过限额</p>
</td>
</tr>
<tr id="row1413318188552"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p13133121814552"><a name="p13133121814552"></a><a name="p13133121814552"></a>APIG.3105</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p52331620268"><a name="p52331620268"></a><a name="p52331620268"></a>The number of signature keys exceeds the maximum allowed limit.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p12133201812557"><a name="p12133201812557"></a><a name="p12133201812557"></a>签名密钥数量超过限额</p>
</td>
</tr>
<tr id="row17383115185510"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p14383515185513"><a name="p14383515185513"></a><a name="p14383515185513"></a>APIG.3106</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p636218317265"><a name="p636218317265"></a><a name="p636218317265"></a>The number of variables exceeds the maximum allowed limit.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1938321517557"><a name="p1938321517557"></a><a name="p1938321517557"></a>变量个数超过限额</p>
</td>
</tr>
<tr id="row183059134558"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p4305191315518"><a name="p4305191315518"></a><a name="p4305191315518"></a>APIG.3107</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p3532144032616"><a name="p3532144032616"></a><a name="p3532144032616"></a>The number of request throttling policies exceeds the maximum allowed limit.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p33051213135511"><a name="p33051213135511"></a><a name="p33051213135511"></a>流控策略个数超过限额</p>
</td>
</tr>
<tr id="row14992310155516"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p79926104551"><a name="p79926104551"></a><a name="p79926104551"></a>APIG.3108</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p7840819193214"><a name="p7840819193214"></a><a name="p7840819193214"></a>The number of domain names exceeds the maximum allowed limit.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p18992110115517"><a name="p18992110115517"></a><a name="p18992110115517"></a>分组自定义域名个数超过限额</p>
</td>
</tr>
<tr id="row9383515105617"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p43834156560"><a name="p43834156560"></a><a name="p43834156560"></a>APIG.3109</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p69445376271"><a name="p69445376271"></a><a name="p69445376271"></a>The number of VPC channels exceeds the maximum allowed limit.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p9383141585615"><a name="p9383141585615"></a><a name="p9383141585615"></a>VPC通道数量超过限额</p>
</td>
</tr>
<tr id="row523619185612"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p223121919568"><a name="p223121919568"></a><a name="p223121919568"></a>APIG.3110</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p36315493271"><a name="p36315493271"></a><a name="p36315493271"></a>The number of instances exceeds the maximum allowed limit.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p123819165615"><a name="p123819165615"></a><a name="p123819165615"></a>VPC通道中的云主机数量超过限额</p>
</td>
</tr>
<tr id="row126638301337"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p166636309334"><a name="p166636309334"></a><a name="p166636309334"></a>APIG.3111</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1559176165914"><a name="p1559176165914"></a><a name="p1559176165914"></a>The number of parameters in req_params exceeds the maximum allowed limit.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p146631030123315"><a name="p146631030123315"></a><a name="p146631030123315"></a>API参数个数超过限额</p>
</td>
</tr>
<tr id="row3607933173316"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p126074335337"><a name="p126074335337"></a><a name="p126074335337"></a>APIG.3112</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1331641813283"><a name="p1331641813283"></a><a name="p1331641813283"></a>The number of access control policies exceeds the maximum allowed limit.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p160733313319"><a name="p160733313319"></a><a name="p160733313319"></a>ACL策略个数超过限额</p>
</td>
</tr>
<tr id="row137501049174315"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1775294934319"><a name="p1775294934319"></a><a name="p1775294934319"></a>APIG.3113</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1075204912432"><a name="p1075204912432"></a><a name="p1075204912432"></a>The maximum number of API backend policies has been reached.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p175219490438"><a name="p175219490438"></a><a name="p175219490438"></a>API的策略后端个数超过限额</p>
</td>
</tr>
<tr id="row038123816553"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p113814385557"><a name="p113814385557"></a><a name="p113814385557"></a>APIG.3114</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p193818389559"><a name="p193818389559"></a><a name="p193818389559"></a>The maximum number of policy conditions has been reached.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p183820380556"><a name="p183820380556"></a><a name="p183820380556"></a>策略后端的策略条件个数超过限额</p>
</td>
</tr>
<tr id="row196251125152116"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1462752522110"><a name="p1462752522110"></a><a name="p1462752522110"></a>APIG.3125</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p12627132542118"><a name="p12627132542118"></a><a name="p12627132542118"></a>The maximum number of APIs for one API group has been reached.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p8627142517214"><a name="p8627142517214"></a><a name="p8627142517214"></a>分组内的API数量达到上限</p>
</td>
</tr>
<tr id="row929832318165"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p132991423161612"><a name="p132991423161612"></a><a name="p132991423161612"></a>APIG.3127</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p7509115514167"><a name="p7509115514167"></a><a name="p7509115514167"></a>The number of APIs has reached the upper limit. A maximum of xxx APIs can be imported at a time.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p27217114175"><a name="p27217114175"></a><a name="p27217114175"></a>导入API数量超过限制，每次最多导入数量为：xxx</p>
</td>
</tr>
<tr id="row37459402"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p14312706"><a name="p14312706"></a><a name="p14312706"></a>APIG.3201</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1427942942816"><a name="p1427942942816"></a><a name="p1427942942816"></a>The API group name already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p20364675"><a name="p20364675"></a><a name="p20364675"></a>指定的API分组名称已存在</p>
</td>
</tr>
<tr id="row49064351"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p14789508"><a name="p14789508"></a><a name="p14789508"></a>APIG.3202</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p249153952811"><a name="p249153952811"></a><a name="p249153952811"></a>The API name already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p61655571"><a name="p61655571"></a><a name="p61655571"></a>指定的API名称已存在</p>
</td>
</tr>
<tr id="row18029228"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p51081335"><a name="p51081335"></a><a name="p51081335"></a>APIG.3203</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p552919496287"><a name="p552919496287"></a><a name="p552919496287"></a>The app name already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p2975719"><a name="p2975719"></a><a name="p2975719"></a>指定的应用名称已存在</p>
</td>
</tr>
<tr id="row26781478"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p21816130"><a name="p21816130"></a><a name="p21816130"></a>APIG.3204</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p22276139"><a name="p22276139"></a><a name="p22276139"></a>The request throttling policy name already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p59536840"><a name="p59536840"></a><a name="p59536840"></a>指定的流控策略名称已存在</p>
</td>
</tr>
<tr id="row66069518"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p50030741"><a name="p50030741"></a><a name="p50030741"></a>APIG.3205</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p868557298"><a name="p868557298"></a><a name="p868557298"></a>The environment name already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p22240452"><a name="p22240452"></a><a name="p22240452"></a>指定的环境名称已存在</p>
</td>
</tr>
<tr id="row65946346"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p40053798"><a name="p40053798"></a><a name="p40053798"></a>APIG.3206</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p23132166"><a name="p23132166"></a><a name="p23132166"></a>The access control policy name already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p61766130"><a name="p61766130"></a><a name="p61766130"></a>指定的ACL策略名称已存在</p>
</td>
</tr>
<tr id="row1094905081112"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p094995031110"><a name="p094995031110"></a><a name="p094995031110"></a>APIG.3207</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p643215207299"><a name="p643215207299"></a><a name="p643215207299"></a>The signature key name already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p994985011114"><a name="p994985011114"></a><a name="p994985011114"></a>指定的签名密钥名称已存在</p>
</td>
</tr>
<tr id="row11693133115813"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p16937310583"><a name="p16937310583"></a><a name="p16937310583"></a>APIG.3208</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p2347133417464"><a name="p2347133417464"></a><a name="p2347133417464"></a>The VPC channel name already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p769333125817"><a name="p769333125817"></a><a name="p769333125817"></a>VPC通道名称已存在</p>
</td>
</tr>
<tr id="row681542415385"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p18815192417388"><a name="p18815192417388"></a><a name="p18815192417388"></a>APIG.3209</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p378911434467"><a name="p378911434467"></a><a name="p378911434467"></a>The parameter name already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p98151124143816"><a name="p98151124143816"></a><a name="p98151124143816"></a>参数名称已存在</p>
</td>
</tr>
<tr id="row1955683612572"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p15556436165718"><a name="p15556436165718"></a><a name="p15556436165718"></a>APIG.3210</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p13556736145719"><a name="p13556736145719"></a><a name="p13556736145719"></a>The backend policy name already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1755663611574"><a name="p1755663611574"></a><a name="p1755663611574"></a>策略后端名称已存在</p>
</td>
</tr>
<tr id="row32385986"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p6019205"><a name="p6019205"></a><a name="p6019205"></a>APIG.3301</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p230544317299"><a name="p230544317299"></a><a name="p230544317299"></a>The API already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p31995881"><a name="p31995881"></a><a name="p31995881"></a>API已存在</p>
</td>
</tr>
<tr id="row19527476"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p38221738"><a name="p38221738"></a><a name="p38221738"></a>APIG.3302</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p6548205510294"><a name="p6548205510294"></a><a name="p6548205510294"></a>The excluded configuration already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p54110919"><a name="p54110919"></a><a name="p54110919"></a>特殊配置已存在</p>
</td>
</tr>
<tr id="row17236231"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p53957433"><a name="p53957433"></a><a name="p53957433"></a>APIG.3303</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1087862014478"><a name="p1087862014478"></a><a name="p1087862014478"></a>The environment variable already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p15464836"><a name="p15464836"></a><a name="p15464836"></a>环境变量已存在</p>
</td>
</tr>
<tr id="row7159834181511"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p71592034141520"><a name="p71592034141520"></a><a name="p71592034141520"></a>APIG.3304</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p16413529163010"><a name="p16413529163010"></a><a name="p16413529163010"></a>The purchasing order already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p515943431516"><a name="p515943431516"></a><a name="p515943431516"></a>订单已存在</p>
</td>
</tr>
<tr id="row204561731131514"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p64561331131512"><a name="p64561331131512"></a><a name="p64561331131512"></a>APIG.3305</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1695814426475"><a name="p1695814426475"></a><a name="p1695814426475"></a>The URL domain name already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p11456103131513"><a name="p11456103131513"></a><a name="p11456103131513"></a>域名已存在</p>
</td>
</tr>
<tr id="row85107254015"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1751010284014"><a name="p1751010284014"></a><a name="p1751010284014"></a>APIG.3306</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p6279155813304"><a name="p6279155813304"></a><a name="p6279155813304"></a>The IP address already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p551017264018"><a name="p551017264018"></a><a name="p551017264018"></a>IP地址已存在</p>
</td>
</tr>
<tr id="row155021631155516"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1650213110553"><a name="p1650213110553"></a><a name="p1650213110553"></a>APIG.3307</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p9935049192417"><a name="p9935049192417"></a><a name="p9935049192417"></a>The project ID has already been bound to the AZ.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p95021231185519"><a name="p95021231185519"></a><a name="p95021231185519"></a>租户已经与业务区绑定</p>
</td>
</tr>
<tr id="row196756022511"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p8675150152515"><a name="p8675150152515"></a><a name="p8675150152515"></a>APIG.3308</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p16675605251"><a name="p16675605251"></a><a name="p16675605251"></a>The excluded request throttling configuration already exists.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p16675190192519"><a name="p16675190192519"></a><a name="p16675190192519"></a>特殊流控策略已经存在</p>
</td>
</tr>
<tr id="row851217105557"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p451213102555"><a name="p451213102555"></a><a name="p451213102555"></a>APIG.3400</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p17512171017556"><a name="p17512171017556"></a><a name="p17512171017556"></a>The resource cannot be changed.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p13512151095512"><a name="p13512151095512"></a><a name="p13512151095512"></a>资源不能被修改</p>
</td>
</tr>
<tr id="row33680016"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p43726746"><a name="p43726746"></a><a name="p43726746"></a>APIG.3401</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p169301053153112"><a name="p169301053153112"></a><a name="p169301053153112"></a>The API group has already been listed on the marketplace or is under approval.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p788764"><a name="p788764"></a><a name="p788764"></a>指定的API分组处于上架状态或审核状态，不允许修改</p>
</td>
</tr>
<tr id="row9669125322815"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p766915530283"><a name="p766915530283"></a><a name="p766915530283"></a>APIG.3402</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p58271516320"><a name="p58271516320"></a><a name="p58271516320"></a>The API group has already been purchased.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p966945313283"><a name="p966945313283"></a><a name="p966945313283"></a>指定的API分组已被购买，不允许修改</p>
</td>
</tr>
<tr id="row171613218298"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1571612132913"><a name="p1571612132913"></a><a name="p1571612132913"></a>APIG.3403</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p6716629290"><a name="p6716629290"></a><a name="p6716629290"></a>The API group does not contain any APIs.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1271672112912"><a name="p1271672112912"></a><a name="p1271672112912"></a>指定的API分组下没有API</p>
</td>
</tr>
<tr id="row135291155295"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1852912542914"><a name="p1852912542914"></a><a name="p1852912542914"></a>APIG.3404</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p205291457297"><a name="p205291457297"></a><a name="p205291457297"></a>The API group is not approved.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p05291652292"><a name="p05291652292"></a><a name="p05291652292"></a>指定的API分组未通过审核</p>
</td>
</tr>
<tr id="row7098876"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p38138113"><a name="p38138113"></a><a name="p38138113"></a>APIG.3405</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1364412569326"><a name="p1364412569326"></a><a name="p1364412569326"></a>The app was generated on the marketplace.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1830242501516"><a name="p1830242501516"></a><a name="p1830242501516"></a>云市场内置应用，不允许删除</p>
</td>
</tr>
<tr id="row196852157298"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p06851715162915"><a name="p06851715162915"></a><a name="p06851715162915"></a>APIG.3406</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p132414663317"><a name="p132414663317"></a><a name="p132414663317"></a>You cannot purchase resources that you have already purchased.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p10685715142915"><a name="p10685715142915"></a><a name="p10685715142915"></a>无需购买自己的资源</p>
</td>
</tr>
<tr id="row32631419192915"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1226381919295"><a name="p1226381919295"></a><a name="p1226381919295"></a>APIG.3407</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p139801319173318"><a name="p139801319173318"></a><a name="p139801319173318"></a>The billing mode cannot be changed.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p17263131942911"><a name="p17263131942911"></a><a name="p17263131942911"></a>计费类型不可更改</p>
</td>
</tr>
<tr id="row918218334411"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p31831433124119"><a name="p31831433124119"></a><a name="p31831433124119"></a>APIG.3408</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1518314339410"><a name="p1518314339410"></a><a name="p1518314339410"></a>The API is not accessed through App authentication.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p8183103384115"><a name="p8183103384115"></a><a name="p8183103384115"></a>API的认证类型不是APP</p>
</td>
</tr>
<tr id="row1581012240295"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1810224112918"><a name="p1810224112918"></a><a name="p1810224112918"></a>APIG.3409</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p522139193317"><a name="p522139193317"></a><a name="p522139193317"></a>Apps of other tenants cannot be authorized to call APIs you have purchased.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p447182716202"><a name="p447182716202"></a><a name="p447182716202"></a>购买的API不能给非自有APP授权</p>
</td>
</tr>
<tr id="row1049712712912"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p3497227142918"><a name="p3497227142918"></a><a name="p3497227142918"></a>APIG.3410</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p48531387494"><a name="p48531387494"></a><a name="p48531387494"></a>Apps cannot be authorized to call purchased APIs in a non-RELEASE environment.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p44971227102920"><a name="p44971227102920"></a><a name="p44971227102920"></a>购买的API不能在非RELEASE环境给APP授权</p>
</td>
</tr>
<tr id="row45330613"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p47901055"><a name="p47901055"></a><a name="p47901055"></a>APIG.3411</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p12874417153419"><a name="p12874417153419"></a><a name="p12874417153419"></a>The APIs belong to different tenants.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p138888472399"><a name="p138888472399"></a><a name="p138888472399"></a>指定的API不属于同一个租户，无法授权</p>
</td>
</tr>
<tr id="row10871532302"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1087111321509"><a name="p1087111321509"></a><a name="p1087111321509"></a>APIG.3412</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p3448530103414"><a name="p3448530103414"></a><a name="p3448530103414"></a>The API provider has been frozen.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p48711332204"><a name="p48711332204"></a><a name="p48711332204"></a>该API提供者已经被冻结</p>
</td>
</tr>
<tr id="row12109514256"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p610914141953"><a name="p610914141953"></a><a name="p610914141953"></a>APIG.3414</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p17150145820346"><a name="p17150145820346"></a><a name="p17150145820346"></a>The VPC channel is already being used by another API.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p181093141551"><a name="p181093141551"></a><a name="p181093141551"></a>指定的VPC通道已经被API占用</p>
</td>
</tr>
<tr id="row14143111115610"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p20143121110618"><a name="p20143121110618"></a><a name="p20143121110618"></a>APIG.3415</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p15143141113613"><a name="p15143141113613"></a><a name="p15143141113613"></a>The API group cannot be deleted because it contains APIs.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1814320119613"><a name="p1814320119613"></a><a name="p1814320119613"></a>指定的API分组下存在API</p>
</td>
</tr>
<tr id="row12311317352"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p931161719516"><a name="p931161719516"></a><a name="p931161719516"></a>APIG.3416</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p171441940193515"><a name="p171441940193515"></a><a name="p171441940193515"></a>The API cannot be deleted because it has been published.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p23111171358"><a name="p23111171358"></a><a name="p23111171358"></a>指定的API已经发布</p>
</td>
</tr>
<tr id="row971019326405"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p571013284013"><a name="p571013284013"></a><a name="p571013284013"></a>APIG.3417</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p92892506350"><a name="p92892506350"></a><a name="p92892506350"></a>The account is being used.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p8710163254020"><a name="p8710163254020"></a><a name="p8710163254020"></a>账号已经被使用</p>
</td>
</tr>
<tr id="row4454153804810"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p184541438174811"><a name="p184541438174811"></a><a name="p184541438174811"></a>APIG.3418</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p14346817123615"><a name="p14346817123615"></a><a name="p14346817123615"></a>The environment contains published APIs.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p44548383488"><a name="p44548383488"></a><a name="p44548383488"></a>指定的环境下存在已发布的API</p>
</td>
</tr>
<tr id="row12877152765610"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p3877172710562"><a name="p3877172710562"></a><a name="p3877172710562"></a>APIG.3419</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p17544103012256"><a name="p17544103012256"></a><a name="p17544103012256"></a>The default AZ cannot be bound to users.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p287752716562"><a name="p287752716562"></a><a name="p287752716562"></a>默认业务区不允许绑定用户</p>
</td>
</tr>
<tr id="row646317712422"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1146367154216"><a name="p1146367154216"></a><a name="p1146367154216"></a>APIG.3420</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1846317717427"><a name="p1846317717427"></a><a name="p1846317717427"></a>The API group is no longer available on the marketplace.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p04634774212"><a name="p04634774212"></a><a name="p04634774212"></a>指定的API分组已经退市</p>
</td>
</tr>
<tr id="row639411226442"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1073725184517"><a name="p1073725184517"></a><a name="p1073725184517"></a>APIG.3447</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p139442234411"><a name="p139442234411"></a><a name="p139442234411"></a>The Acl Strategy has already binded to APIs.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p039416223445"><a name="p039416223445"></a><a name="p039416223445"></a>指定的ACL策略绑定了API，无法删除</p>
</td>
</tr>
<tr id="row382012774318"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p88218764318"><a name="p88218764318"></a><a name="p88218764318"></a>APIG.3451</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p682157134313"><a name="p682157134313"></a><a name="p682157134313"></a>The Throttle Strategy has already binded to APIs.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1182120715430"><a name="p1182120715430"></a><a name="p1182120715430"></a>指定的流控策略绑定了API，无法删除</p>
</td>
</tr>
<tr id="row47861616513"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p878171617513"><a name="p878171617513"></a><a name="p878171617513"></a>APIG.3471</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p147831625117"><a name="p147831625117"></a><a name="p147831625117"></a>No permissions to perform operations on this type of VPC channel.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p078171645115"><a name="p078171645115"></a><a name="p078171645115"></a>不能对该类型的VPC通道执行此操作</p>
</td>
</tr>
<tr id="row3795142095120"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p77951201519"><a name="p77951201519"></a><a name="p77951201519"></a>APIG.3472</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1179552019511"><a name="p1179552019511"></a><a name="p1179552019511"></a>The load balancer is already being used by another VPC channel.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p17795520155120"><a name="p17795520155120"></a><a name="p17795520155120"></a>后端实例已经被其它通道使用</p>
</td>
</tr>
<tr id="row1797622219514"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1297632215118"><a name="p1297632215118"></a><a name="p1297632215118"></a>APIG.3473</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p7976172245118"><a name="p7976172245118"></a><a name="p7976172245118"></a>The load balancer has already been bound to another endpoint service.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1597692285110"><a name="p1597692285110"></a><a name="p1597692285110"></a>后端实例已经绑定了其它endpoint service</p>
</td>
</tr>
<tr id="row29011114102712"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p6901714192710"><a name="p6901714192710"></a><a name="p6901714192710"></a>APIG.3474</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p109016149279"><a name="p109016149279"></a><a name="p109016149279"></a>The API group ID in the URL does not match the API group to which the URL domain has been bound.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p5901191442710"><a name="p5901191442710"></a><a name="p5901191442710"></a>url中的分组id和url中的域名绑定的分组id不匹配</p>
</td>
</tr>
<tr id="row249611140209"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p0496111442013"><a name="p0496111442013"></a><a name="p0496111442013"></a>APIG.3500</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p8377935193614"><a name="p8377935193614"></a><a name="p8377935193614"></a>Failed to synchronize data to etcd.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p749621420202"><a name="p749621420202"></a><a name="p749621420202"></a>同步路由至ETCD异常</p>
</td>
</tr>
<tr id="row469016331878"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p669010333711"><a name="p669010333711"></a><a name="p669010333711"></a>APIG.3600</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1669083316714"><a name="p1669083316714"></a><a name="p1669083316714"></a>Json or Yaml format error.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p166902331077"><a name="p166902331077"></a><a name="p166902331077"></a>Json或Yaml格式错误</p>
</td>
</tr>
<tr id="row1363610361718"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1663610363714"><a name="p1663610363714"></a><a name="p1663610363714"></a>APIG.3601</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1163623614720"><a name="p1163623614720"></a><a name="p1163623614720"></a>The Swagger file version must be 2.0.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p063703612719"><a name="p063703612719"></a><a name="p063703612719"></a>swagger版本不是2.0</p>
</td>
</tr>
<tr id="row186110391777"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p18611153914714"><a name="p18611153914714"></a><a name="p18611153914714"></a>APIG.3602</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p5611839972"><a name="p5611839972"></a><a name="p5611839972"></a>Syntax error in the Swagger file.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p36111239473"><a name="p36111239473"></a><a name="p36111239473"></a>swagger语法错误</p>
</td>
</tr>
<tr id="row1934154316716"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1334124316712"><a name="p1334124316712"></a><a name="p1334124316712"></a>APIG.3603</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p153411343076"><a name="p153411343076"></a><a name="p153411343076"></a>The Swagger file content is too long.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p153412436711"><a name="p153412436711"></a><a name="p153412436711"></a>swagger内容超过限制</p>
</td>
</tr>
<tr id="row765810162317"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p146581716153113"><a name="p146581716153113"></a><a name="p146581716153113"></a>APIG.9000</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p02521648183613"><a name="p02521648183613"></a><a name="p02521648183613"></a>Failed to delete the trigger.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p8658121610313"><a name="p8658121610313"></a><a name="p8658121610313"></a>删除函数计算触发器失败</p>
</td>
</tr>
<tr id="row14821161173315"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p128216120337"><a name="p128216120337"></a><a name="p128216120337"></a>APIG.9001</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p20821316337"><a name="p20821316337"></a><a name="p20821316337"></a>Failed to create or update the trigger.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p20848446123411"><a name="p20848446123411"></a><a name="p20848446123411"></a>创建或重建函数计算触发器失败</p>
</td>
</tr>
<tr id="row19324163173710"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p11324103115371"><a name="p11324103115371"></a><a name="p11324103115371"></a>APIG.9002</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p19161505377"><a name="p19161505377"></a><a name="p19161505377"></a>Invalid function URN.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p18918165718374"><a name="p18918165718374"></a><a name="p18918165718374"></a>函数URN校验失败</p>
</td>
</tr>
<tr id="row8297173194111"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p32971331174115"><a name="p32971331174115"></a><a name="p32971331174115"></a>APIG.9003</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p12956145773717"><a name="p12956145773717"></a><a name="p12956145773717"></a>Statistics Center request failed.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1829712310416"><a name="p1829712310416"></a><a name="p1829712310416"></a>请求统计中心失败</p>
</td>
</tr>
<tr id="row122151638191712"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p202156387179"><a name="p202156387179"></a><a name="p202156387179"></a>APIG.9004</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p4215133841711"><a name="p4215133841711"></a><a name="p4215133841711"></a>IAM request failed.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p152153383175"><a name="p152153383175"></a><a name="p152153383175"></a>请求IAM认证鉴权失败</p>
</td>
</tr>
<tr id="row143671715204218"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p13367151512425"><a name="p13367151512425"></a><a name="p13367151512425"></a>APIG.9005</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p336721524213"><a name="p336721524213"></a><a name="p336721524213"></a>VPC request failed.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p736718153425"><a name="p736718153425"></a><a name="p736718153425"></a>请求VPC服务失败</p>
</td>
</tr>
<tr id="row084545433713"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p284595419379"><a name="p284595419379"></a><a name="p284595419379"></a>APIG.9006</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p184585423716"><a name="p184585423716"></a><a name="p184585423716"></a>DNS request failed.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1845135473711"><a name="p1845135473711"></a><a name="p1845135473711"></a>请求dns服务失败</p>
</td>
</tr>
<tr id="row18471647127"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p154711245121"><a name="p154711245121"></a><a name="p154711245121"></a>APIG.9007</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p2047194101211"><a name="p2047194101211"></a><a name="p2047194101211"></a>ELB request failed.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p194714411129"><a name="p194714411129"></a><a name="p194714411129"></a>请求ELB服务失败</p>
</td>
</tr>
<tr id="row1821194124512"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p17211194164513"><a name="p17211194164513"></a><a name="p17211194164513"></a>APIG.9008</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p18211741114516"><a name="p18211741114516"></a><a name="p18211741114516"></a>Too many requests.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p6211341184515"><a name="p6211341184515"></a><a name="p6211341184515"></a>请求过于频繁，请稍后重试</p>
</td>
</tr>
<tr id="row3170105413615"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p151702541567"><a name="p151702541567"></a><a name="p151702541567"></a>APIG.9901</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p111709541368"><a name="p111709541368"></a><a name="p111709541368"></a>The system is unavailable because it is being upgraded.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p12170954662"><a name="p12170954662"></a><a name="p12170954662"></a>升级导致系统不可用</p>
</td>
</tr>
<tr id="row7503123025916"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p17503730115913"><a name="p17503730115913"></a><a name="p17503730115913"></a>APIG.9991</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p5443339135617"><a name="p5443339135617"></a><a name="p5443339135617"></a>Gateway timeout.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p16503113012591"><a name="p16503113012591"></a><a name="p16503113012591"></a>网关超时</p>
</td>
</tr>
<tr id="row19691123225914"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p10691183235917"><a name="p10691183235917"></a><a name="p10691183235917"></a>APIG.9992</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p21011057115613"><a name="p21011057115613"></a><a name="p21011057115613"></a>Service unavailable.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p439462217598"><a name="p439462217598"></a><a name="p439462217598"></a>服务不可用</p>
</td>
</tr>
<tr id="row1426910372592"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p226943717598"><a name="p226943717598"></a><a name="p226943717598"></a>APIG.9993</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p5874151313574"><a name="p5874151313574"></a><a name="p5874151313574"></a>Bad gateway.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p9269737195914"><a name="p9269737195914"></a><a name="p9269737195914"></a>不正确的网关</p>
</td>
</tr>
<tr id="row14160435185918"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p1016093513595"><a name="p1016093513595"></a><a name="p1016093513595"></a>APIG.9994</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p4728333155719"><a name="p4728333155719"></a><a name="p4728333155719"></a>The requested function is not available.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1216023585914"><a name="p1216023585914"></a><a name="p1216023585914"></a>请求的功能暂未实现</p>
</td>
</tr>
<tr id="row4738162715916"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p107381927155917"><a name="p107381927155917"></a><a name="p107381927155917"></a>APIG.9995</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p146931430123013"><a name="p146931430123013"></a><a name="p146931430123013"></a>No permissions to request this method.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p12738142775911"><a name="p12738142775911"></a><a name="p12738142775911"></a>不允许请求该方法</p>
</td>
</tr>
<tr id="row206604253599"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p266012516593"><a name="p266012516593"></a><a name="p266012516593"></a>APIG.9996</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1755714125814"><a name="p1755714125814"></a><a name="p1755714125814"></a>The request URL does not exist.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p179048161234"><a name="p179048161234"></a><a name="p179048161234"></a>请求的地址不存在</p>
</td>
</tr>
<tr id="row9394622105919"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p5394822175914"><a name="p5394822175914"></a><a name="p5394822175914"></a>APIG.9997</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p424615945816"><a name="p424615945816"></a><a name="p424615945816"></a>Request forbidden.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p437154284014"><a name="p437154284014"></a><a name="p437154284014"></a>请求被禁止</p>
</td>
</tr>
<tr id="row12173682013"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p5173885013"><a name="p5173885013"></a><a name="p5173885013"></a>APIG.9998</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p106141217115819"><a name="p106141217115819"></a><a name="p106141217115819"></a>Unauthorized request.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p1217358503"><a name="p1217358503"></a><a name="p1217358503"></a>请求未授权</p>
</td>
</tr>
<tr id="row29277991"><td class="cellrowborder" valign="top" width="14.93%" headers="mcps1.2.4.1.1 "><p id="p22707034"><a name="p22707034"></a><a name="p22707034"></a>APIG.9999</p>
</td>
<td class="cellrowborder" valign="top" width="46.07%" headers="mcps1.2.4.1.2 "><p id="p1583742585816"><a name="p1583742585816"></a><a name="p1583742585816"></a>System error.</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p66287124"><a name="p66287124"></a><a name="p66287124"></a>系统错误，请联系管理员</p>
</td>
</tr>
</tbody>
</table>

