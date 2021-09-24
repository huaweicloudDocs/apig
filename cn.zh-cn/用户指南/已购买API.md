# 已购买API<a name="ZH-CN_TOPIC_0000001142957202"></a>

## 操作场景<a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_section1731012541118"></a>

API网关共享版支持查看已购买的API，明确已购买服务的详情。并通过调试API，验证服务是否正常。

已购买的API，需要通过APP认证方式调用。

## 前提条件<a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_section83110548119"></a>

已从云市场购买了API。

## 操作步骤<a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_section8731554122615"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域。
3.  单击管理控制台左上角![](figures/zh-cn_image_0000001145871970.png)，然后单击“API网关 APIG”。
4.  在左侧导航树中单击“共享版”。
5.  单击“调用API \> 已购买API”，进入到已购买API分组信息页面。

    **图 1**  已购买API分组示例<a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_fig173661455192013"></a>  
    ![](figures/已购买API分组示例.png "已购买API分组示例")

6.  单击待查看的API分组名称，进入此分组详情页面。

    查看此分组下已购买的API列表和此分组的详细信息。

    **图 2**  已购买API的分组详情示例<a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_fig18693205011226"></a>  
    ![](figures/已购买API的分组详情示例.png "已购买API的分组详情示例")

7.  在待调试API所在行，单击“调试API”，跳转到“调试API”页面。
8.  左侧为API请求参数配置区域，参数说明如[表1](#zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_table1699044810457)所示。右侧为API发送的请求信息和API请求调用后的返回结果回显。

    **表 1**  调试API

    <a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_table1699044810457"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_row1699084815458"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p15990164813454"><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p15990164813454"></a><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p15990164813454"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p99907481453"><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p99907481453"></a><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p99907481453"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_row699013480453"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p8441941705"><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p8441941705"></a><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p8441941705"></a>协议</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p444164702"><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p444164702"></a><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p444164702"></a>仅在“请求协议”为“HTTP&amp;HTTPS”时，支持修改。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_row1299115489454"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p9131133413812"><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p9131133413812"></a><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p9131133413812"></a>方法</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p12132434583"><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p12132434583"></a><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p12132434583"></a>仅在“Method”为“ANY”时，支持修改。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_row159914483458"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p1513211341184"><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p1513211341184"></a><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p1513211341184"></a>路径</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p16134203420812"><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p16134203420812"></a><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p16134203420812"></a>仅在“匹配模式”为“前缀模式”时，支持自定义路径。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_row13534132210817"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p113573412820"><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p113573412820"></a><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p113573412820"></a>路径参数</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p713613341089"><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p713613341089"></a><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p713613341089"></a>仅在“Path”中存在“{}”时，支持修改。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_row10991184818452"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p7136113420810"><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p7136113420810"></a><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p7136113420810"></a>请求头</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p81365341489"><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p81365341489"></a><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p81365341489"></a>HTTP Headers的参数与参数值。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_row14991164811452"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p1213919343817"><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p1213919343817"></a><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p1213919343817"></a>查询参数</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p121394342815"><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p121394342815"></a><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p121394342815"></a>Query的参数与参数值。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_row12855103617473"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p181415341480"><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p181415341480"></a><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p181415341480"></a>Body</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p514113346815"><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p514113346815"></a><a name="zh-cn_topic_0000001128537188_zh-cn_topic_0084753158_p514113346815"></a>仅在“Method”为“PATCH”/“POST”/“PUT”时，支持修改。</p>
    </td>
    </tr>
    </tbody>
    </table>

9.  添加请求参数后，单击“发送请求”。

    右侧返回结果回显区域打印API调用的Response信息。

    ![](figures/zh-cn_image_0000001188807567.png)

10. 开发者可以通过调整请求参数与参数值，发送不同的请求，验证API服务。

