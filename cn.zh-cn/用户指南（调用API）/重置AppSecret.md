# 重置AppSecret<a name="apig-zh-ug-180307053"></a>

## 操作场景<a name="section1731012541118"></a>

重置AppSecret，将AppSecret的值重新改变。重置完成后，原先的AppSecret将失效，绑定此应用的API将无法调用，请更新AppSecret，并重新调用API。

## 前提条件<a name="section83110548119"></a>

已创建应用。

## 操作步骤<a name="section8731554122615"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域。
3.  在服务列表中，选择“应用服务 \> API网关”，进入API网关服务管理页面。
4.  在左侧选择您的API版本，单击并进入到对应版本的API开发与调用管理页面。

    “共享版”指直接创建并管理API，如涉及到费用，以API调用次数计费。

    “专享版”指在API专享版实例中创建并管理API，如涉及到费用，按实例运行时间计费。

5.  单击“调用API \> 应用管理”，进入到应用管理信息页面。
6.  单击待重置AppSecret的应用名称，进入应用详情页面。
7.  在右上角单击“重置AppSecret”，弹出“重置AppSecret”对话框。
8.  单击“确定”，完成AppSecret的重置。

## 使用API方式重置AppSecret<a name="section321091893419"></a>

您还可以使用API的方式重置AppSecret，具体操作请查看以下链接。

[重置密钥](https://support.huaweicloud.com/api-apig/apig-zh-api-180713038.html)

