# 创建API分组<a name="ZH-CN_TOPIC_0000001188877313"></a>

## 操作场景<a name="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_section1731012541118"></a>

创建API前，需要先创建API分组。API分组相当于API的集合，API提供者以API分组为单位，管理分组内的所有API。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   一个API只能属于某一个API分组。
>-   每个用户最多创建50个API分组。

## 操作步骤<a name="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_section8731554122615"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域。
3.  单击管理控制台左上角![](figures/zh-cn_image_0000001145871968.png)，然后单击“API网关 APIG”。
4.  在左侧选择您的API版本，单击并进入到对应版本的API开发与调用管理页面。
    -   “共享版”指直接创建并管理API，如涉及到费用，以API调用次数计费。
    -   “专享版”指在API专享版实例中创建并管理API，如涉及到费用，按实例运行时间计费。

5.  单击“开放API \> API分组”，进入到API分组信息页面。
6.  单击“创建分组”，弹出“创建分组”对话框。填写如[表1](#zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_table195413315428)所示信息。

    **表 1**  分组信息表

    <a name="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_table195413315428"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_row45523384220"><th class="cellrowborder" valign="top" width="31.03%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p65563314423"><a name="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p65563314423"></a><a name="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p65563314423"></a>信息项</p>
    </th>
    <th class="cellrowborder" valign="top" width="68.97%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p356183311427"><a name="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p356183311427"></a><a name="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p356183311427"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_row1156183364219"><td class="cellrowborder" valign="top" width="31.03%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p105616333427"><a name="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p105616333427"></a><a name="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p105616333427"></a>分组名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.97%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p1656123374219"><a name="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p1656123374219"></a><a name="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p1656123374219"></a>API分组名称，用于将API接口进行分组管理。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_row14879114316433"><td class="cellrowborder" valign="top" width="31.03%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p12880154304320"><a name="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p12880154304320"></a><a name="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p12880154304320"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="68.97%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p48801043134312"><a name="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p48801043134312"></a><a name="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_p48801043134312"></a>对分组的介绍。</p>
    </td>
    </tr>
    </tbody>
    </table>

7.  完成分组信息填写后，单击“确定”，创建API分组。

    创建分组成功后，在“API分组”页面的列表中显示新创建的API分组。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >-   API分组创建后，系统为分组自动分配一个内部测试用的子域名，此子域名每天最多可以访问1000次。
    >-   专享版实例创建后，有一个默认分组，可直接通过虚拟私有云地址调用默认分组中的API。
    >-   共享版中的API，分组子域名可公网访问。专享版中的API，分组子域名默认只能在与实例相同VPC内的服务器上解析和访问，如要子域名要支持公网解析与访问，请在专享版实例上绑定公网入口弹性IP。
    >-   对外开放API时，您需要为API分组绑定您自己的独立域名。


## 使用API方式创建API分组<a name="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_section7546754133419"></a>

您还可以使用API的方式创建API分组，具体操作请查看以下链接。

[创建API分组](https://support.huaweicloud.com/api-apig/CreateApiGroupV2.html)

## 后续操作<a name="zh-cn_topic_0000001128537176_zh-cn_topic_0089184725_zh-cn_topic_0080101677_section12967127112416"></a>

API分组创建成功后，您可以为此分组[绑定域名](绑定域名.md#ZH-CN_TOPIC_0000001142797438)，API调用者通过访问独立域名来调用您开放的API。

