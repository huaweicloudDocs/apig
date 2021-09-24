# 调用API<a name="ZH-CN_TOPIC_0000001188920189"></a>

## 获取API及文档<a name="zh-cn_topic_0000001129305640_section15668112016810"></a>

在调用API前，您需要向API提供者获取API的请求信息，包括访问域名、请求协议、请求方法、请求路径以及请求参数。

**获取API**：

-   从云市场购买。
-   通过线下传递（如企业内部或者企业间合作）。

**获取文档**：

-   已发布到应用市场的API，通过云市场可以获取参考文档。
-   未发布到应用市场的API，需要线下联系API提供方获取参考文档。
-   如果API为云服务官方提供的服务，还可以在[华为云帮助中心](https://support.huaweicloud.com/index.html)获取参考文档。

根据API使用的安全认证方式，还要获取相关的请求认证信息：

-   **APP认证**：
    -   签名认证：向API提供者获取该API所授权应用的Key和Secret（或客户端的AppKey和AppSecret），以及用于调用API的SDK。
    -   简易认证：向API提供者获取该API所在应用的AppCode。
    -   其他认证：向API提供者获取该API所授权应用的Key和Secret（或客户端的AppKey和AppSecret）。

-   **华为IAM认证**：通过云服务平台的帐号凭证（帐号和密码获取Token或者AK/SK）进行认证。如果使用AK/SK进行认证，还需要向API提供者获取用于调用API的SDK。
-   **自定义认证**：向API提供者获取请求参数中要携带的自定义认证信息。
-   **无认证**：无需认证信息。

## 调用API<a name="zh-cn_topic_0000001129305640_section14411121782210"></a>

1.  配置请求地址相关参数。

    <a name="zh-cn_topic_0000001129305640_table34781521204310"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0000001129305640_row104795211436"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="zh-cn_topic_0000001129305640_p1024865514435"><a name="zh-cn_topic_0000001129305640_p1024865514435"></a><a name="zh-cn_topic_0000001129305640_p1024865514435"></a>API调用场景</p>
    </th>
    <th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="zh-cn_topic_0000001129305640_p1024735514432"><a name="zh-cn_topic_0000001129305640_p1024735514432"></a><a name="zh-cn_topic_0000001129305640_p1024735514432"></a>API请求参数配置</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0000001129305640_row1161116509438"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0000001129305640_p745119295438"><a name="zh-cn_topic_0000001129305640_p745119295438"></a><a name="zh-cn_topic_0000001129305640_p745119295438"></a>使用域名调用API</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0000001129305640_p1451132919432"><a name="zh-cn_topic_0000001129305640_p1451132919432"></a><a name="zh-cn_topic_0000001129305640_p1451132919432"></a>使用服务分配的子域名或服务绑定的域名调用API，无需另外配置。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001129305640_row411301313617"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0000001129305640_p785858979"><a name="zh-cn_topic_0000001129305640_p785858979"></a><a name="zh-cn_topic_0000001129305640_p785858979"></a>使用IP调用DEFAULT分组的API</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0000001129305640_p108581585713"><a name="zh-cn_topic_0000001129305640_p108581585713"></a><a name="zh-cn_topic_0000001129305640_p108581585713"></a>专享版API允许使用IP地址调用DEFAULT分组下的API，无需另外配置。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001129305640_row3232376712"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0000001129305640_p4858138272"><a name="zh-cn_topic_0000001129305640_p4858138272"></a><a name="zh-cn_topic_0000001129305640_p4858138272"></a>使用IP调用非DEFAULT分组的API</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><a name="zh-cn_topic_0000001129305640_ul1985813814711"></a><a name="zh-cn_topic_0000001129305640_ul1985813814711"></a><ul id="zh-cn_topic_0000001129305640_ul1985813814711"><li>专享版实例<a href="修改专享版实例.md#zh-cn_topic_0000001128537174_zh-cn_topic_0272531149_section12828154014100">配置参数</a>“app_route”已设置为“on”，允许通过IP访问API。</li><li>不允许使用IP地址直接调用非DEFAULT分组下的API，需要在请求消息中添加Header参数“X-HW-ID”，参数值为API所授权的Key或客户端的AppKey。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

2.  配置认证参数。

    <a name="zh-cn_topic_0000001129305640_table51311449166"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0000001129305640_row141414445165"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="zh-cn_topic_0000001129305640_p4143444163"><a name="zh-cn_topic_0000001129305640_p4143444163"></a><a name="zh-cn_topic_0000001129305640_p4143444163"></a>API认证方式</p>
    </th>
    <th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="zh-cn_topic_0000001129305640_p1914134431617"><a name="zh-cn_topic_0000001129305640_p1914134431617"></a><a name="zh-cn_topic_0000001129305640_p1914134431617"></a>API请求参数配置</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0000001129305640_row414184461610"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0000001129305640_p184213254178"><a name="zh-cn_topic_0000001129305640_p184213254178"></a><a name="zh-cn_topic_0000001129305640_p184213254178"></a>APP认证（签名认证）</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0000001129305640_p1942192551712"><a name="zh-cn_topic_0000001129305640_p1942192551712"></a><a name="zh-cn_topic_0000001129305640_p1942192551712"></a>使用获取的SDK对API请求进行签名，具体请参考<a href="https://support.huaweicloud.com/devg-apig/apig-dev-180907066.html" target="_blank" rel="noopener noreferrer">使用APP认证调用API</a></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001129305640_row1314104441614"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0000001129305640_p11965104095410"><a name="zh-cn_topic_0000001129305640_p11965104095410"></a><a name="zh-cn_topic_0000001129305640_p11965104095410"></a>APP认证（简易认证）</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0000001129305640_p642192516170"><a name="zh-cn_topic_0000001129305640_p642192516170"></a><a name="zh-cn_topic_0000001129305640_p642192516170"></a>在API请求中添加Header参数“X-Apig-AppCode”，参数值为<a href="#zh-cn_topic_0000001129305640_section15668112016810">获取API及文档</a>中获取到的AppCode。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001129305640_row161464431612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0000001129305640_p78591053125218"><a name="zh-cn_topic_0000001129305640_p78591053125218"></a><a name="zh-cn_topic_0000001129305640_p78591053125218"></a>APP认证（app_api_key认证）</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><a name="zh-cn_topic_0000001129305640_ul1142162520174"></a><a name="zh-cn_topic_0000001129305640_ul1142162520174"></a><ul id="zh-cn_topic_0000001129305640_ul1142162520174"><li>专享版的实例<a href="修改专享版实例.md#zh-cn_topic_0000001128537174_zh-cn_topic_0272531149_section12828154014100">配置参数</a>“app_api_key”已设置为“on”，开启app_api_key认证。</li><li>在API请求中添加Header或Query参数“apikey”，参数值为<a href="#zh-cn_topic_0000001129305640_section15668112016810">获取API及文档</a>中获取到的Key或AppKey。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001129305640_row914344101610"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0000001129305640_p170951025517"><a name="zh-cn_topic_0000001129305640_p170951025517"></a><a name="zh-cn_topic_0000001129305640_p170951025517"></a>APP认证（app_secret认证）</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><a name="zh-cn_topic_0000001129305640_ul14422122531720"></a><a name="zh-cn_topic_0000001129305640_ul14422122531720"></a><ul id="zh-cn_topic_0000001129305640_ul14422122531720"><li>专享版的实例<a href="修改专享版实例.md#zh-cn_topic_0000001128537174_zh-cn_topic_0272531149_section12828154014100">配置参数</a>“app_secret”已设置为“on”，开启app_secret认证，且“app_api_key”已设置为“off”，关闭app_api_key认证。</li><li>在API请求中添加Header参数“X-HW-ID”，参数值为API所授权的Key或客户端的AppKey。</li><li>在API请求中添加Header参数“X-HW-AppKey”，参数值为<a href="#zh-cn_topic_0000001129305640_section15668112016810">获取API及文档</a>中获取到的Secret或AppSecret。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001129305640_row151474418164"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0000001129305640_p19859125335212"><a name="zh-cn_topic_0000001129305640_p19859125335212"></a><a name="zh-cn_topic_0000001129305640_p19859125335212"></a>APP认证（app_basic认证）</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><a name="zh-cn_topic_0000001129305640_ul1442515250177"></a><a name="zh-cn_topic_0000001129305640_ul1442515250177"></a><ul id="zh-cn_topic_0000001129305640_ul1442515250177"><li>专享版的实例<a href="修改专享版实例.md#zh-cn_topic_0000001128537174_zh-cn_topic_0272531149_section12828154014100">配置参数</a>“app_basic”已设置为“on”，开启app_basic认证。</li><li>在API请求中添加Header参数“Authorization”，参数值为"Basic "+base64(appkey+":"+appsecret)，其中appkey和appsecret分别为<a href="#zh-cn_topic_0000001129305640_section15668112016810">获取API及文档</a>中获取到的Key和Secret（或AppKey和AppSecret）。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001129305640_row1614204412166"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0000001129305640_p58594537528"><a name="zh-cn_topic_0000001129305640_p58594537528"></a><a name="zh-cn_topic_0000001129305640_p58594537528"></a>APP认证（app_jwt认证）</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><a name="zh-cn_topic_0000001129305640_ul54251925181711"></a><a name="zh-cn_topic_0000001129305640_ul54251925181711"></a><ul id="zh-cn_topic_0000001129305640_ul54251925181711"><li>专享版的实例<a href="修改专享版实例.md#zh-cn_topic_0000001128537174_zh-cn_topic_0272531149_section12828154014100">配置参数</a>“app_jwt”已设置为“on”，开启app_jwt认证。</li><li>在API请求中添加Header参数“Timestamp”，参数值为当前时间的Unix时间戳。</li><li>在API请求中添加Header参数“Authorization”，参数值为sha256(appkey+appsecret+timestamp)，其中appkey和appsecret分别为<a href="#zh-cn_topic_0000001129305640_section15668112016810">获取API及文档</a>中获取到的Key和Secret（或AppKey和AppSecret），timestamp为当前时间的Unix时间戳。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001129305640_row1714644141611"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0000001129305640_p54259252175"><a name="zh-cn_topic_0000001129305640_p54259252175"></a><a name="zh-cn_topic_0000001129305640_p54259252175"></a>华为IAM认证（Token认证）</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0000001129305640_p5425122561715"><a name="zh-cn_topic_0000001129305640_p5425122561715"></a><a name="zh-cn_topic_0000001129305640_p5425122561715"></a>先获取云服务平台的认证Token，然后在API请求中携带Token进行认证，具体请参考<a href="https://support.huaweicloud.com/devg-apig/apig-dev-180307020.html" target="_blank" rel="noopener noreferrer">Token认证</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001129305640_row131510445161"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0000001129305640_p127721215617"><a name="zh-cn_topic_0000001129305640_p127721215617"></a><a name="zh-cn_topic_0000001129305640_p127721215617"></a>华为IAM认证（AK/SK认证）</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0000001129305640_p642542531719"><a name="zh-cn_topic_0000001129305640_p642542531719"></a><a name="zh-cn_topic_0000001129305640_p642542531719"></a>调用API时，使用获取的SDK对API请求进行签名，具体请参考<a href="https://support.huaweicloud.com/devg-apig/apig-dev-180307021.html" target="_blank" rel="noopener noreferrer">AK/SK认证</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001129305640_row171584416166"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0000001129305640_p12425102591715"><a name="zh-cn_topic_0000001129305640_p12425102591715"></a><a name="zh-cn_topic_0000001129305640_p12425102591715"></a>自定义认证</p>
    <p id="zh-cn_topic_0000001129305640_p184391225171719"><a name="zh-cn_topic_0000001129305640_p184391225171719"></a><a name="zh-cn_topic_0000001129305640_p184391225171719"></a></p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0000001129305640_p114261625191712"><a name="zh-cn_topic_0000001129305640_p114261625191712"></a><a name="zh-cn_topic_0000001129305640_p114261625191712"></a>在API请求参数中携带认证信息进行认证。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001129305640_row736810221172"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="zh-cn_topic_0000001129305640_p15426102513175"><a name="zh-cn_topic_0000001129305640_p15426102513175"></a><a name="zh-cn_topic_0000001129305640_p15426102513175"></a>无认证</p>
    <p id="zh-cn_topic_0000001129305640_p543962510173"><a name="zh-cn_topic_0000001129305640_p543962510173"></a><a name="zh-cn_topic_0000001129305640_p543962510173"></a></p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="zh-cn_topic_0000001129305640_p194261325181719"><a name="zh-cn_topic_0000001129305640_p194261325181719"></a><a name="zh-cn_topic_0000001129305640_p194261325181719"></a>无需认证，可直接调用API。</p>
    </td>
    </tr>
    </tbody>
    </table>


