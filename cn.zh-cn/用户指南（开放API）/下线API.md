# 下线API<a name="apig-zh-ug-180307024"></a>

## 操作场景<a name="section25971517509"></a>

已发布的API因为其他原因需要暂停对外提供服务，可以暂时将API从相关环境中下线。

>![](public_sys-resources/icon-notice.gif) **须知：**   
>该操作将导致此API在指定的环境无法被访问，请确保已经告知使用此API的用户。  

## 前提条件<a name="section1678010231609"></a>

-   已创建API分组和分组内的API。
-   API已发布到该环境。

## 操作步骤<a name="section1929412566340"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域。
3.  在服务列表中，选择“应用服务 \> API网关”，进入API网关服务管理页面。
4.  在左侧选择您的API版本，单击并进入到对应版本的API开发与调用管理页面。

    “共享版”指直接创建并管理API，如涉及到费用，以API调用次数计费。

    “专享版”指在API专享版实例中创建并管理API，如涉及到费用，按实例运行时间计费。

5.  单击“开放API \> API管理”，进入到API管理信息页面。
6.  通过以下任意一种方法，下线API。

    -   在待下线的API所在行，单击“更多 \> 下线”，弹出“下线API”对话框。
    -   单击“_API名称_”，进入API详情页面。在右上角单击“下线”，弹出“下线API”对话框。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >如果需要批量下线API，则勾选待下线的API，单击“下线”。最多同时下线1000个API。  

7.  选择API需要下线的环境，单击“确定”，完成API下线。

## 使用API方式下线API<a name="zh-cn_topic_0080101678_section7546754133419"></a>

您还可以使用API的方式下线API，具体操作请查看以下链接。

[下线API](https://support.huaweicloud.com/api-apig/apig-zh-api-180713029.html)

## 后续操作<a name="zh-cn_topic_0080101678_section1679143819506"></a>

您将API下线后，可以通过[删除API](删除API.md)，释放此API所占用的资源。

