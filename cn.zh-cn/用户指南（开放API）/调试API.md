# 调试API<a name="apig-zh-ug-180307025"></a>

## 操作场景<a name="section25971517509"></a>

API创建后需要验证服务是否正常，管理控制台提供调试功能，开发者可以添加HTTP头部参数与body体参数，调试API接口。

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   后端路径中含有环境变量的API，不支持调试。  
>-   如果API已绑定流控策略，在调试API时，流控策略无效。  

## 前提条件<a name="section1678010231609"></a>

-   已创建API分组和分组内的API。
-   已搭建完成后端服务。

## 操作步骤<a name="section1929412566340"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择地域。
3.  在服务列表中，单击“应用服务 \> API网关”，进入API网关服务管理页面。
4.  单击“开放API \> API管理”，进入到API管理信息页面。
5.  通过以下任意一种方法，进入API调试页面。

    -   在待调试的API所在行，单击“更多 \> 调试”。
    -   单击“_API名称_”，进入API详情页面。在右上角单击“调试”。

    左侧为API请求参数配置区域，参数说明如[表1](#table1699044810457)所示。右侧为API发送的请求信息和API请求调用后的返回结果回显。

    **表 1**  调试API

    <a name="table1699044810457"></a>
    <table><thead align="left"><tr id="row1699084815458"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p15990164813454"><a name="p15990164813454"></a><a name="p15990164813454"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p99907481453"><a name="p99907481453"></a><a name="p99907481453"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2431345016"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p8441941705"><a name="p8441941705"></a><a name="p8441941705"></a>Protocol</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p444164702"><a name="p444164702"></a><a name="p444164702"></a>仅在“请求协议”为“HTTP&amp;HTTPS”时，支持修改。</p>
    </td>
    </tr>
    <tr id="row699013480453"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p599054811454"><a name="p599054811454"></a><a name="p599054811454"></a>Method</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1990104816453"><a name="p1990104816453"></a><a name="p1990104816453"></a>仅在“Method”为“ANY”时，支持修改。</p>
    </td>
    </tr>
    <tr id="row1299115489454"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p699184812454"><a name="p699184812454"></a><a name="p699184812454"></a>Suffix</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p49911348204512"><a name="p49911348204512"></a><a name="p49911348204512"></a>仅在“匹配模式”为“前缀模式”时，支持自定义路径。</p>
    </td>
    </tr>
    <tr id="row159914483458"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p59911248174520"><a name="p59911248174520"></a><a name="p59911248174520"></a>Path Parameters</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p139911748164513"><a name="p139911748164513"></a><a name="p139911748164513"></a>仅在“Path”中存在“{}”时，支持修改。</p>
    </td>
    </tr>
    <tr id="row10991184818452"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p1899144854513"><a name="p1899144854513"></a><a name="p1899144854513"></a>Headers</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1991134811453"><a name="p1991134811453"></a><a name="p1991134811453"></a>HTTP Headers的参数与参数值。</p>
    </td>
    </tr>
    <tr id="row14991164811452"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p2991248184511"><a name="p2991248184511"></a><a name="p2991248184511"></a>Query Parameters</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p8991748114514"><a name="p8991748114514"></a><a name="p8991748114514"></a>Query的参数与参数值。</p>
    </td>
    </tr>
    <tr id="row12855103617473"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p1685653611470"><a name="p1685653611470"></a><a name="p1685653611470"></a>Body</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p3856163615475"><a name="p3856163615475"></a><a name="p3856163615475"></a>仅在“Method”为“ANY”/“PATCH”/“POST”/“PUT”时，支持修改。</p>
    </td>
    </tr>
    </tbody>
    </table>

6.  添加请求参数后，单击“发送请求”。

    右侧返回结果回显区域打印API调用的Response信息。

7.  开发者可以通过调整请求参数与参数值，发送不同的请求，验证API服务。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >如果需要修改API参数，请在右上角单击“编辑”，进入API编辑页面。  


