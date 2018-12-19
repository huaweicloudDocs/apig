# REST API介绍<a name="apig-zh-api-180713011"></a>

API网关服务接口符合RESTful API的设计风格。

REST从资源的角度来观察整个网络，分布在各处的资源由URI（Uniform Resource Identifier）确定，而客户端的应用通过URL（Unified Resource Locator）来获取资源。

URL的一般格式为（带方括号的为可选项）：

protocol://hostname\[:port\] \[/uri\]

URL中的参数说明如[表1](#table12812809)所示。

**表 1**  URL中的参数说明

<a name="table12812809"></a>
<table><thead align="left"><tr id="row16762932"><th class="cellrowborder" valign="top" width="22.220000000000002%" id="mcps1.2.4.1.1"><p id="p15620237"><a name="p15620237"></a><a name="p15620237"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="54.55%" id="mcps1.2.4.1.2"><p id="p57279683"><a name="p57279683"></a><a name="p57279683"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="23.23%" id="mcps1.2.4.1.3"><p id="p9142717"><a name="p9142717"></a><a name="p9142717"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="row2362595"><td class="cellrowborder" valign="top" width="22.220000000000002%" headers="mcps1.2.4.1.1 "><p id="p57152543"><a name="p57152543"></a><a name="p57152543"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="54.55%" headers="mcps1.2.4.1.2 "><p id="p65953238"><a name="p65953238"></a><a name="p65953238"></a>请求使用的协议类型，如HTTPS。</p>
<p id="p56708236"><a name="p56708236"></a><a name="p56708236"></a>HTTPS表示通过安全的SSL加密的HTTP协议访问该资源。</p>
</td>
<td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.3 "><p id="p29964426"><a name="p29964426"></a><a name="p29964426"></a>是</p>
</td>
</tr>
<tr id="row1244379"><td class="cellrowborder" valign="top" width="22.220000000000002%" headers="mcps1.2.4.1.1 "><p id="p33685880"><a name="p33685880"></a><a name="p33685880"></a>hostname</p>
</td>
<td class="cellrowborder" valign="top" width="54.55%" headers="mcps1.2.4.1.2 "><p id="p44201778"><a name="p44201778"></a><a name="p44201778"></a>请求使用的服务器名。是指存放资源的服务器的域名或IP地址。</p>
</td>
<td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.3 "><p id="p23574256"><a name="p23574256"></a><a name="p23574256"></a>是</p>
</td>
</tr>
<tr id="row10841716"><td class="cellrowborder" valign="top" width="22.220000000000002%" headers="mcps1.2.4.1.1 "><p id="p5763828"><a name="p5763828"></a><a name="p5763828"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="54.55%" headers="mcps1.2.4.1.2 "><p id="p64216941"><a name="p64216941"></a><a name="p64216941"></a>请求使用的端口号。根据软件服务器的部署不同而不同。缺省时使用默认端口，各种传输协议都有默认的端口号，如HTTPS的默认端口为443。</p>
</td>
<td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.3 "><p id="p34189702"><a name="p34189702"></a><a name="p34189702"></a>否</p>
</td>
</tr>
<tr id="row39271862"><td class="cellrowborder" valign="top" width="22.220000000000002%" headers="mcps1.2.4.1.1 "><p id="p26904226"><a name="p26904226"></a><a name="p26904226"></a>uri</p>
</td>
<td class="cellrowborder" valign="top" width="54.55%" headers="mcps1.2.4.1.2 "><p id="p31758723"><a name="p31758723"></a><a name="p31758723"></a>资源路径，也即API访问路径。</p>
</td>
<td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.3 "><p id="p22319809"><a name="p22319809"></a><a name="p22319809"></a>否</p>
</td>
</tr>
</tbody>
</table>

## 请求URI<a name="section1849899574"></a>

请求URI由如下部分组成。

**\{URI-scheme\} :// \{**Endpoint**\} / \{resource-path\} ? \{query-string\}**

尽管请求URI包含在请求消息头中，但大多数语言或框架都要求您从请求消息中单独传递它，所有在此单独拿出来强调。URI中的参数说明如[表2](#t1797260c744a4e1a85d354f259cae55a)所示。

**表 2**  URI中的参数说明

<a name="t1797260c744a4e1a85d354f259cae55a"></a>
<table><thead align="left"><tr id="r6dceed05bcc649d2b032accbb2980a31"><th class="cellrowborder" valign="top" width="24.529999999999998%" id="mcps1.2.3.1.1"><p id="a3446b6b785cb432bae9f45aef9177041"><a name="a3446b6b785cb432bae9f45aef9177041"></a><a name="a3446b6b785cb432bae9f45aef9177041"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="75.47%" id="mcps1.2.3.1.2"><p id="abe71244a12ac45308e99d4bbf975a9f8"><a name="abe71244a12ac45308e99d4bbf975a9f8"></a><a name="abe71244a12ac45308e99d4bbf975a9f8"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row106982018513"><td class="cellrowborder" valign="top" width="24.529999999999998%" headers="mcps1.2.3.1.1 "><p id="p136991001517"><a name="p136991001517"></a><a name="p136991001517"></a>URI-scheme</p>
</td>
<td class="cellrowborder" valign="top" width="75.47%" headers="mcps1.2.3.1.2 "><p id="p56992017520"><a name="p56992017520"></a><a name="p56992017520"></a>表示用于传输请求的协议。</p>
</td>
</tr>
<tr id="rb217758afff146a1b40b0dcbb28a4ae1"><td class="cellrowborder" valign="top" width="24.529999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0035614179_p480227019422"><a name="zh-cn_topic_0035614179_p480227019422"></a><a name="zh-cn_topic_0035614179_p480227019422"></a>Endpoint</p>
</td>
<td class="cellrowborder" valign="top" width="75.47%" headers="mcps1.2.3.1.2 "><p id="p1780595345416"><a name="p1780595345416"></a><a name="p1780595345416"></a>指定承载REST服务端点的服务器域名或IP，从<a href="http://developer.huaweicloud.com/endpoint.html" target="_blank" rel="noopener noreferrer">地区和终端节点</a>获取。</p>
</td>
</tr>
<tr id="refeed61892004ea682639be281a1a707"><td class="cellrowborder" valign="top" width="24.529999999999998%" headers="mcps1.2.3.1.1 "><p id="p1797614317513"><a name="p1797614317513"></a><a name="p1797614317513"></a>resource-path</p>
</td>
<td class="cellrowborder" valign="top" width="75.47%" headers="mcps1.2.3.1.2 "><p id="a90409cbb8b1c49c4ad4d3cfee16f475e"><a name="a90409cbb8b1c49c4ad4d3cfee16f475e"></a><a name="a90409cbb8b1c49c4ad4d3cfee16f475e"></a>资源路径，也即API访问路径。从具体接口的URI模块获取，例如“v3/auth/tokens”。</p>
</td>
</tr>
<tr id="row19939365518"><td class="cellrowborder" valign="top" width="24.529999999999998%" headers="mcps1.2.3.1.1 "><p id="p393966455"><a name="p393966455"></a><a name="p393966455"></a>Query string</p>
</td>
<td class="cellrowborder" valign="top" width="75.47%" headers="mcps1.2.3.1.2 "><p id="p159401867517"><a name="p159401867517"></a><a name="p159401867517"></a>可选参数，例如API版本或资源选择标准。</p>
</td>
</tr>
</tbody>
</table>

## 请求方法<a name="section1580010308490"></a>

在HTTP协议中，请求可以使用多种请求方法，例如GET、PUT、POST、DELETE等，用于指明以何种方式来访问指定的资源，目前提供的REST接口支持的请求方法如[表3](#table48206417)所示。

**表 3**  请求方法一览表

<a name="table48206417"></a>
<table><thead align="left"><tr id="row55728610"><th class="cellrowborder" valign="top" width="30%" id="mcps1.2.3.1.1"><p id="p17723551"><a name="p17723551"></a><a name="p17723551"></a>方法</p>
</th>
<th class="cellrowborder" valign="top" width="70%" id="mcps1.2.3.1.2"><p id="p26321508"><a name="p26321508"></a><a name="p26321508"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row51667418"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.3.1.1 "><p id="p24311336"><a name="p24311336"></a><a name="p24311336"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.2.3.1.2 "><p id="p23061239"><a name="p23061239"></a><a name="p23061239"></a>请求服务器返回指定资源。</p>
</td>
</tr>
<tr id="row6224567"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.3.1.1 "><p id="p34427881"><a name="p34427881"></a><a name="p34427881"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.2.3.1.2 "><p id="p37194992"><a name="p37194992"></a><a name="p37194992"></a>请求服务器更新指定资源。</p>
</td>
</tr>
<tr id="row66319479"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.3.1.1 "><p id="p3168728"><a name="p3168728"></a><a name="p3168728"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.2.3.1.2 "><p id="p55340417"><a name="p55340417"></a><a name="p55340417"></a>请求服务器新增资源或执行特殊操作。</p>
</td>
</tr>
<tr id="row28301713"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.3.1.1 "><p id="p10737402"><a name="p10737402"></a><a name="p10737402"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.2.3.1.2 "><p id="p64423232"><a name="p64423232"></a><a name="p64423232"></a>请求服务器删除指定资源，如删除API等。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息头<a name="section37818817"></a>

请求消息头由若干头域构成，每个头域由一个域名，冒号\(: \)和域值组成。

公共请求报头如[表4](#d0e750)所示。

**表 4**  公共请求消息头

<a name="d0e750"></a>
<table><thead align="left"><tr id="row48068532"><th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.2.5.1.1"><p id="p1237054"><a name="p1237054"></a><a name="p1237054"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="32.65%" id="mcps1.2.5.1.2"><p id="p33092577"><a name="p33092577"></a><a name="p33092577"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="20.41%" id="mcps1.2.5.1.3"><p id="p63253060"><a name="p63253060"></a><a name="p63253060"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="29.59%" id="mcps1.2.5.1.4"><p id="p23224207"><a name="p23224207"></a><a name="p23224207"></a>示例</p>
</th>
</tr>
</thead>
<tbody><tr id="row2112619"><td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.1 "><p id="p86023305127"><a name="p86023305127"></a><a name="p86023305127"></a>x-sdk-date</p>
</td>
<td class="cellrowborder" valign="top" width="32.65%" headers="mcps1.2.5.1.2 "><p id="p86021630121217"><a name="p86021630121217"></a><a name="p86021630121217"></a>请求的发生时间，格式为(YYYYMMDD'T'HHMMSS'Z')。</p>
<p id="p560213301124"><a name="p560213301124"></a><a name="p560213301124"></a>取值为当前系统的GMT时间。</p>
</td>
<td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.5.1.3 "><p id="p16602133011218"><a name="p16602133011218"></a><a name="p16602133011218"></a>否</p>
<p id="p360283091210"><a name="p360283091210"></a><a name="p360283091210"></a>使用AK/SK认证时必选</p>
</td>
<td class="cellrowborder" valign="top" width="29.59%" headers="mcps1.2.5.1.4 "><p id="p1160293041212"><a name="p1160293041212"></a><a name="p1160293041212"></a>20150907T101459Z</p>
</td>
</tr>
<tr id="row1827941711129"><td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.1 "><p id="p1160213041210"><a name="p1160213041210"></a><a name="p1160213041210"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="32.65%" headers="mcps1.2.5.1.2 "><p id="p7602130121212"><a name="p7602130121212"></a><a name="p7602130121212"></a>签名认证信息</p>
<p id="p15602830121216"><a name="p15602830121216"></a><a name="p15602830121216"></a>该值来源于请求签名结果。</p>
</td>
<td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.5.1.3 "><p id="p5602930131217"><a name="p5602930131217"></a><a name="p5602930131217"></a>否</p>
<p id="p960223081216"><a name="p960223081216"></a><a name="p960223081216"></a>使用Token认证时必选</p>
</td>
<td class="cellrowborder" valign="top" width="29.59%" headers="mcps1.2.5.1.4 "><p id="p1160373013128"><a name="p1160373013128"></a><a name="p1160373013128"></a>-</p>
</td>
</tr>
<tr id="row13731878"><td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.1 "><p id="p060311300123"><a name="p060311300123"></a><a name="p060311300123"></a>Authorization</p>
</td>
<td class="cellrowborder" valign="top" width="32.65%" headers="mcps1.2.5.1.2 "><p id="p1360323031211"><a name="p1360323031211"></a><a name="p1360323031211"></a>签名认证信息。</p>
<p id="p156031730161213"><a name="p156031730161213"></a><a name="p156031730161213"></a>该值来源于请求签名结果。</p>
</td>
<td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.5.1.3 "><p id="p1760313302124"><a name="p1760313302124"></a><a name="p1760313302124"></a>否</p>
<p id="p1260319308126"><a name="p1260319308126"></a><a name="p1260319308126"></a>使用AK/SK认证时必选</p>
</td>
<td class="cellrowborder" valign="top" width="29.59%" headers="mcps1.2.5.1.4 "><p id="p196031730111214"><a name="p196031730111214"></a><a name="p196031730111214"></a>SDK-HMAC-SHA256 Credential=ZIRRKMTWPTQFQI1WKNKB/20150907//ec2/sdk_request, SignedHeaders=content-type;host;x-sdk-date, Signature=55741b610f3c9fa3ae40b5a8021ebf7ebc2a28a603fc62d25cb3bfe6608e1994</p>
</td>
</tr>
<tr id="row43304686"><td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.1 "><p id="p18018639"><a name="p18018639"></a><a name="p18018639"></a>Host</p>
</td>
<td class="cellrowborder" valign="top" width="32.65%" headers="mcps1.2.5.1.2 "><p id="p50223649"><a name="p50223649"></a><a name="p50223649"></a>请求的服务器信息，从服务API的URL中获取。值为hostname[:port]。端口缺省时使用默认的端口，https的默认端口为443。</p>
</td>
<td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.5.1.3 "><p id="p41583755"><a name="p41583755"></a><a name="p41583755"></a>是。</p>
</td>
<td class="cellrowborder" valign="top" width="29.59%" headers="mcps1.2.5.1.4 "><p id="p12841014"><a name="p12841014"></a><a name="p12841014"></a>code.test.com</p>
<p id="p48460267"><a name="p48460267"></a><a name="p48460267"></a>or</p>
<p id="p33489226"><a name="p33489226"></a><a name="p33489226"></a>code.test.com:443</p>
</td>
</tr>
<tr id="row32967578"><td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.1 "><p id="p53128157"><a name="p53128157"></a><a name="p53128157"></a>Content-type</p>
</td>
<td class="cellrowborder" valign="top" width="32.65%" headers="mcps1.2.5.1.2 "><p id="p8413469"><a name="p8413469"></a><a name="p8413469"></a>发送的实体的MIME类型。</p>
</td>
<td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.5.1.3 "><p id="p10402369"><a name="p10402369"></a><a name="p10402369"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="29.59%" headers="mcps1.2.5.1.4 "><p id="p37285554"><a name="p37285554"></a><a name="p37285554"></a>application/json</p>
</td>
</tr>
<tr id="row25666"><td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.1 "><p id="p2078992"><a name="p2078992"></a><a name="p2078992"></a>Content-Length</p>
</td>
<td class="cellrowborder" valign="top" width="32.65%" headers="mcps1.2.5.1.2 "><p id="p34180703"><a name="p34180703"></a><a name="p34180703"></a>请求body长度，单位为Byte。</p>
</td>
<td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.5.1.3 "><p id="p17173591"><a name="p17173591"></a><a name="p17173591"></a>POST/PUT请求必填。 GET/DELETE不需要设置该参数。</p>
</td>
<td class="cellrowborder" valign="top" width="29.59%" headers="mcps1.2.5.1.4 "><p id="p48883615"><a name="p48883615"></a><a name="p48883615"></a>3495</p>
</td>
</tr>
<tr id="row3436217134611"><td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.1 "><p id="p125792269463"><a name="p125792269463"></a><a name="p125792269463"></a>x-project-id</p>
</td>
<td class="cellrowborder" valign="top" width="32.65%" headers="mcps1.2.5.1.2 "><p id="p657942654614"><a name="p657942654614"></a><a name="p657942654614"></a>用户当前使用的Project ID。</p>
</td>
<td class="cellrowborder" valign="top" width="20.41%" headers="mcps1.2.5.1.3 "><p id="p105794268464"><a name="p105794268464"></a><a name="p105794268464"></a>否</p>
<p id="p45792263462"><a name="p45792263462"></a><a name="p45792263462"></a>使用AK/SK认证时必选</p>
</td>
<td class="cellrowborder" valign="top" width="29.59%" headers="mcps1.2.5.1.4 "><p id="p11579142624610"><a name="p11579142624610"></a><a name="p11579142624610"></a>d025c1ff85a24e1d86e15de3bd308a27</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-notice.gif) **注意：**   
>如果使用多项目（多Project）时，http头部消息中必须含有x-project-id字段，此字段需要自行添加。以AK/SK认证为例，添加方法如下：  
>1.  参考[获取项目编号](获取项目编号.md)查询到多项目的ID。  
>2.  在AccessServiceImpl.java中的调用signer.sign\(\)方法后面添加一行代码，参数值请填写实际的project id，具体位置参考[3.b](请求签名流程.md#li22657210162236)：  
>    request.addHeader\("x-project-id", "20cf5fb8035543049a80906a6652fed2"\);  
>如上，即可完成多项目下的AK/SK认证，否则可能报错。  

## 请求消息体<a name="section4825033"></a>

以JSON格式封装，基本语法是嵌套式的key:value形式。HTTP请求的正文针对不同的URI对象有不同的必须字段和可选字段。

## 响应消息头<a name="section10185684"></a>

响应的消息报头在大多数情况下含有下面报头：

-   Date:  _Mon, 12 Nov 2007 15:55:01 GMT_

    HTTP协议标准报头。表示消息发送的时间，时间的描述格式由rfc822定义。

-   Content-Length:  **_xxx_**

    HTTP协议标准报头。用于指明实体正文的长度，以字节方式存储的十进制数字来表示

-   Content-Type:  _application/json; charset=UTF-8_

    HTTP协议标准报头。用于指明发送给接收者的实体正文的媒体类型。


调用API时，API网关自动增加如下响应消息头。

X-Apig-Mode: debug表示响应消息头增加API网关调试信息。

<a name="table117316235592"></a>
<table><thead align="left"><tr id="row7731192385919"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.1.4.1.1"><p id="p11731172319598"><a name="p11731172319598"></a><a name="p11731172319598"></a>响应消息头</p>
</th>
<th class="cellrowborder" valign="top" width="35.35353535353536%" id="mcps1.1.4.1.2"><p id="p15731102315910"><a name="p15731102315910"></a><a name="p15731102315910"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="44.44444444444445%" id="mcps1.1.4.1.3"><p id="p773162375918"><a name="p773162375918"></a><a name="p773162375918"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row177311623155919"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.1.4.1.1 "><p id="p47312236593"><a name="p47312236593"></a><a name="p47312236593"></a>X-Request-Id</p>
</td>
<td class="cellrowborder" valign="top" width="35.35353535353536%" headers="mcps1.1.4.1.2 "><p id="p873111236591"><a name="p873111236591"></a><a name="p873111236591"></a>请求ID</p>
</td>
<td class="cellrowborder" valign="top" width="44.44444444444445%" headers="mcps1.1.4.1.3 "><p id="p8731162335913"><a name="p8731162335913"></a><a name="p8731162335913"></a>所有合法请求，都会返回此参数</p>
</td>
</tr>
<tr id="row1073111238597"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.1.4.1.1 "><p id="p1773132365914"><a name="p1773132365914"></a><a name="p1773132365914"></a>X-Apig-Latency</p>
</td>
<td class="cellrowborder" valign="top" width="35.35353535353536%" headers="mcps1.1.4.1.2 "><p id="p9731823195920"><a name="p9731823195920"></a><a name="p9731823195920"></a>从API网关接收请求到后端返回消息头的用时</p>
</td>
<td class="cellrowborder" valign="top" width="44.44444444444445%" headers="mcps1.1.4.1.3 "><p id="p9731132319591"><a name="p9731132319591"></a><a name="p9731132319591"></a>仅在请求消息头包含X-Apig-Mode: debug时，返回此参数</p>
</td>
</tr>
<tr id="row67311223115912"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.1.4.1.1 "><p id="p2073162335913"><a name="p2073162335913"></a><a name="p2073162335913"></a>X-Apig-Upstream-Latency</p>
</td>
<td class="cellrowborder" valign="top" width="35.35353535353536%" headers="mcps1.1.4.1.2 "><p id="p1115131612616"><a name="p1115131612616"></a><a name="p1115131612616"></a>从API网关请求后端到后端返回消息头的用时</p>
</td>
<td class="cellrowborder" valign="top" width="44.44444444444445%" headers="mcps1.1.4.1.3 "><p id="p773102318597"><a name="p773102318597"></a><a name="p773102318597"></a>仅在请求消息头包含X-Apig-Mode: debug，且后端服务类型不为Mock时，返回此参数</p>
</td>
</tr>
<tr id="row8731152316597"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.1.4.1.1 "><p id="p131483259118"><a name="p131483259118"></a><a name="p131483259118"></a>X-Apig-RateLimit-api</p>
</td>
<td class="cellrowborder" valign="top" width="35.35353535353536%" headers="mcps1.1.4.1.2 "><p id="p1384223313019"><a name="p1384223313019"></a><a name="p1384223313019"></a>API流量控制信息</p>
<p id="p1073172316595"><a name="p1073172316595"></a><a name="p1073172316595"></a>示例：remain:9,limit:10,time:10 second</p>
</td>
<td class="cellrowborder" valign="top" width="44.44444444444445%" headers="mcps1.1.4.1.3 "><p id="p92691839101212"><a name="p92691839101212"></a><a name="p92691839101212"></a>仅在请求消息头包含X-Apig-Mode: debug，且API配置了API流量控制时，返回此参数</p>
</td>
</tr>
<tr id="row2520195919126"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.1.4.1.1 "><p id="p8895889134"><a name="p8895889134"></a><a name="p8895889134"></a>X-Apig-RateLimit-user</p>
</td>
<td class="cellrowborder" valign="top" width="35.35353535353536%" headers="mcps1.1.4.1.2 "><p id="p112070387020"><a name="p112070387020"></a><a name="p112070387020"></a>用户流量限制信息</p>
<p id="p352095941211"><a name="p352095941211"></a><a name="p352095941211"></a>示例：remain:9,limit:10,time:10 second</p>
</td>
<td class="cellrowborder" valign="top" width="44.44444444444445%" headers="mcps1.1.4.1.3 "><p id="p1652085920120"><a name="p1652085920120"></a><a name="p1652085920120"></a>仅在请求消息头包含X-Apig-Mode: debug，且API配置了用户流量限制时，返回此参数</p>
</td>
</tr>
<tr id="row184819451319"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.1.4.1.1 "><p id="p195820971314"><a name="p195820971314"></a><a name="p195820971314"></a>X-Apig-RateLimit-app</p>
</td>
<td class="cellrowborder" valign="top" width="35.35353535353536%" headers="mcps1.1.4.1.2 "><p id="p193517417012"><a name="p193517417012"></a><a name="p193517417012"></a>应用流量限制信息</p>
<p id="p198481443135"><a name="p198481443135"></a><a name="p198481443135"></a>示例：remain:9,limit:10,time:10 second</p>
</td>
<td class="cellrowborder" valign="top" width="44.44444444444445%" headers="mcps1.1.4.1.3 "><p id="p178487431310"><a name="p178487431310"></a><a name="p178487431310"></a>仅在请求消息头包含X-Apig-Mode: debug，且API配置了应用流量限制时，返回此参数</p>
</td>
</tr>
<tr id="row5817527135"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.1.4.1.1 "><p id="p936361051317"><a name="p936361051317"></a><a name="p936361051317"></a>X-Apig-RateLimit-api-allenv</p>
</td>
<td class="cellrowborder" valign="top" width="35.35353535353536%" headers="mcps1.1.4.1.2 "><p id="p133314450013"><a name="p133314450013"></a><a name="p133314450013"></a>API默认流控信息</p>
<p id="p38171823137"><a name="p38171823137"></a><a name="p38171823137"></a>示例：remain:199,limit:200,time:1 second</p>
</td>
<td class="cellrowborder" valign="top" width="44.44444444444445%" headers="mcps1.1.4.1.3 "><p id="p9817721139"><a name="p9817721139"></a><a name="p9817721139"></a>仅在请求消息头包含X-Apig-Mode: debug时，返回此参数</p>
</td>
</tr>
</tbody>
</table>

## 响应消息体<a name="section24562296"></a>

响应正文为JSON格式的文本。

## 发起请求<a name="section3165192822915"></a>

共有三种方式可以基于已构建好的请求消息发起请求，分别为：

-   cURL

    cURL是一个命令行工具，用来执行各种URL操作和信息传输。cURL充当的是HTTP客户端，可以发送HTTP请求给服务端，并接收响应消息。cURL适用于接口调试。关于cURL详细信息请参见[https://curl.haxx.se/](https://curl.haxx.se/)。

-   编码

    通过编码调用接口，组装请求消息，并发送处理请求消息。

-   REST客户端

    Mozilla、Google都为REST提供了图形化的浏览器插件，发送处理请求消息。针对Firefox，请参见[Firefox REST Client](https://addons.mozilla.org/en-US/firefox/addon/restclient/)。针对Chrome，请参见[Chrome REST Client](https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop)。


