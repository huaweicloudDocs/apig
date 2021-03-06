# 创建流控策略并绑定到API<a name="apig-zh-ug-180307029"></a>

## 操作场景<a name="section1731012541118"></a>

流量控制可限制单位时间内API的被调用次数，保护后端服务。

为了提供持续稳定的服务，您可以通过创建流控策略，针对部分API进行流量控制。

流控策略和API本身是相互独立的，只有将流控策略绑定API后，流控策略才对绑定的API生效。

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   每个用户最多创建30个流控策略。  
>-   同一个环境中，一个API只能被一个流控策略绑定，但一个流控策略可以绑定多个API。  

## 前提条件<a name="section83110548119"></a>

需要绑定的API已发布。

## 创建流控策略<a name="section8731554122615"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域。
3.  在服务列表中，选择“应用服务 \> API网关”，进入API网关服务管理页面。
4.  在左侧选择您的API版本，单击并进入到对应版本的API开发与调用管理页面。

    “共享版”指直接创建并管理API，如涉及到费用，以API调用次数计费。

    “专享版”指在API专享版实例中创建并管理API，如涉及到费用，按实例运行时间计费。

5.  单击“开放API \> 流量控制”，进入到流量控制信息页面。
6.  单击“创建流控策略”，弹出“创建流控策略”对话框。输入如[表1](#table195413315428)所示信息。

    **图 1**  创建流控策略<a name="fig04103333113"></a>  
    ![](figures/创建流控策略.png "创建流控策略")

    **表 1**  流控策略信息

    <a name="table195413315428"></a>
    <table><thead align="left"><tr id="row45523384220"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p65563314423"><a name="p65563314423"></a><a name="p65563314423"></a>信息项</p>
    </th>
    <th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p356183311427"><a name="p356183311427"></a><a name="p356183311427"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row175619332424"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p456103313429"><a name="p456103313429"></a><a name="p456103313429"></a>策略名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p16561833104213"><a name="p16561833104213"></a><a name="p16561833104213"></a>API流控策略名称。</p>
    </td>
    </tr>
    <tr id="row936312516340"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p6363325123413"><a name="p6363325123413"></a><a name="p6363325123413"></a>类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p3363192519341"><a name="p3363192519341"></a><a name="p3363192519341"></a>分“基础流控”和“共享流控”两类。</p>
    <p id="p9464135917347"><a name="p9464135917347"></a><a name="p9464135917347"></a>基础流控针对单个API进行流量统计和控制；共享流控的策略，针对绑定了该策略的所有API进行总流量统计和控制。</p>
    </td>
    </tr>
    <tr id="row1156183364219"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p105616333427"><a name="p105616333427"></a><a name="p105616333427"></a>时长</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1656123374219"><a name="p1656123374219"></a><a name="p1656123374219"></a>流量限制的时长。</p>
    <a name="ul580520385234"></a><a name="ul580520385234"></a><ul id="ul580520385234"><li>与“API流量限制”配合使用，表示单位时间内的单个API请求次数上限。</li><li>与“用户流量限制”配合使用，表示单位时间内的单个用户请求次数上限。</li><li>与“应用流量限制”配合使用，表示单位时间内的单个APP请求次数上限。</li></ul>
    </td>
    </tr>
    <tr id="row14879114316433"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p12880154304320"><a name="p12880154304320"></a><a name="p12880154304320"></a>API流量限制</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p48801043134312"><a name="p48801043134312"></a><a name="p48801043134312"></a>单个API被调用次数上限。</p>
    <p id="p3999181141211"><a name="p3999181141211"></a><a name="p3999181141211"></a>与“时长”配合使用，表示单位时间内的单个API请求次数上限。</p>
    </td>
    </tr>
    <tr id="row247519275166"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p14476127151620"><a name="p14476127151620"></a><a name="p14476127151620"></a>用户流量限制</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1347622781611"><a name="p1347622781611"></a><a name="p1347622781611"></a>单个用户调用API次数上限。</p>
    <a name="ul1091113535268"></a><a name="ul1091113535268"></a><ul id="ul1091113535268"><li>不超过“API流量限制”。</li><li>与“时长”配合使用，表示单位时间内的单个用户请求次数上限。</li><li>如果主账号下有多个子用户访问API，按主账号累计的调用次数进行限制。</li></ul>
    </td>
    </tr>
    <tr id="row8159123418166"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p015933461620"><a name="p015933461620"></a><a name="p015933461620"></a>应用流量限制</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p9107151417591"><a name="p9107151417591"></a><a name="p9107151417591"></a>单个应用调用API次数上限。</p>
    <a name="ul448161162718"></a><a name="ul448161162718"></a><ul id="ul448161162718"><li>不超过“用户流量限制”。</li><li>与“时长”配合使用，表示单位时间内的单个应用请求次数上限。</li></ul>
    </td>
    </tr>
    <tr id="row8202182105513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p6202142135511"><a name="p6202142135511"></a><a name="p6202142135511"></a>源IP流量限制</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p152026295512"><a name="p152026295512"></a><a name="p152026295512"></a>单个IP地址调用API次数上限。</p>
    <a name="ul15411858125518"></a><a name="ul15411858125518"></a><ul id="ul15411858125518"><li>不超过“API流量限制”。</li><li>与“时长”配合使用，表示单位时间内的单个IP地址请求次数上限。</li><li>如果调用方在华为云弹性云服务器，且通过弹性公网IP访问API，则不能使用此限制策略。</li></ul>
    </td>
    </tr>
    <tr id="row45611440141619"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p1156124041619"><a name="p1156124041619"></a><a name="p1156124041619"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p25611440141620"><a name="p25611440141620"></a><a name="p25611440141620"></a>关于控制策略的描述。</p>
    </td>
    </tr>
    </tbody>
    </table>

7.  单击“确定”，完成流量控制策略的创建。

    创建成功后，策略信息页面增加显示新创建的策略，您可以将相关API绑定到该策略，以实现流量控制。


## 绑定API<a name="section1853216101881"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域。
3.  在服务列表中，选择“应用服务 \> API网关”，进入API网关服务管理页面。
4.  单击“开放API \> 流量控制”，进入到流量控制信息页面。
5.  通过以下任意一种方法，进入“绑定API”页面。
    -   在待绑定的流量控制策略所在行，单击“绑定API”，进入已绑定API列表页面。单击“绑定API”。
    -   单击策略名称，进入策略详情页面。在“绑定的API列表”页签中单击“绑定API”。

6.  选择“API分组”、“环境”以及“API名称”，筛选所需的API。
7.  勾选API，单击“绑定”，完成API绑定策略。

    **图 2**  绑定API<a name="fig192531244154"></a>  
    ![](figures/绑定API.png "绑定API")

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >在流控策略绑定API后，如果API不需要调用此策略，单击“解除”，解除绑定。如果需要批量解绑API，则勾选待解绑的API，单击“解除”。最多同时解绑1000个API。  


## 使用API方式创建流控策略、绑定API和解除绑定<a name="zh-cn_topic_0080101678_section7546754133419"></a>

您还可以使用API的方式创建流控策略、绑定API和解除绑定，具体操作请查看以下链接。

[创建流控策略](https://support.huaweicloud.com/api-apig/apig-zh-api-180713064.html)

[绑定流控策略](https://support.huaweicloud.com/api-apig/apig-zh-api-180713072.html)

[解除绑定](https://support.huaweicloud.com/api-apig/apig-zh-api-180713075.html)

## 后续操作<a name="section186331115191812"></a>

如果某个应用希望受流量策略控制，可以通过对该策略增加特殊应用实现，具体参考[添加特殊应用或租户](添加特殊应用或租户.md)。增加特殊应用后，此应用的应用流量限制受增加特殊应用时设置的阈值限制，API流量限制和用户流量限制受策略限制。

如果某个租户希望受流量策略控制，可以通过对该策略增加特殊租户实现，具体参考[添加特殊应用或租户](添加特殊应用或租户.md)。增加特殊租户后，此租户的用户流量限制受增加特殊租户时设置的阈值限制，API流量限制和应用流量限制受策略限制。

