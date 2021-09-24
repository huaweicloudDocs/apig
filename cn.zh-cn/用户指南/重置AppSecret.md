# 重置AppSecret<a name="ZH-CN_TOPIC_0000001142797422"></a>

## 操作场景<a name="zh-cn_topic_0000001174497005_zh-cn_topic_0084768156_section1731012541118"></a>

重置AppSecret，将AppSecret的值重新改变。重置完成后，原先的AppSecret将失效，绑定此应用的API将无法调用，请更新AppSecret，并重新调用API。

## 前提条件<a name="zh-cn_topic_0000001174497005_zh-cn_topic_0084768156_section83110548119"></a>

已创建应用。

## 操作步骤<a name="zh-cn_topic_0000001174497005_zh-cn_topic_0084768156_section8731554122615"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域。
3.  单击管理控制台左上角![](figures/zh-cn_image_0000001145871972.png)，然后单击“API网关 APIG”。
4.  在左侧选择您的API版本，单击并进入到对应版本的API开发与调用管理页面。
    -   “共享版”指直接创建并管理API，如涉及到费用，以API调用次数计费。
    -   “专享版”指在API专享版实例中创建并管理API，如涉及到费用，按实例运行时间计费。

5.  单击“调用API \> 应用管理”，进入到应用管理信息页面。
6.  单击待重置AppSecret的应用名称，进入应用详情页面。
7.  在右上角单击“重置AppSecret”，弹出“重置AppSecret”对话框。
8.  单击“确定”，完成AppSecret的重置。

## 使用API方式重置AppSecret<a name="zh-cn_topic_0000001174497005_zh-cn_topic_0084768156_section321091893419"></a>

您还可以使用API的方式重置AppSecret，具体操作请查看以下链接。

[重置密钥](https://support.huaweicloud.com/api-apig/ResettingAppSecretV2.html)

