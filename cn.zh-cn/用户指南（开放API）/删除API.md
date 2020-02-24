# 删除API<a name="apig-zh-ug-180307027"></a>

## 操作场景<a name="section25971517509"></a>

已发布的API不再提供服务，可以将API删除。

>![](public_sys-resources/icon-notice.gif) **须知：**   
>-   该操作将导致此API无法被访问，可能会影响正在使用此API的应用或者用户，请确保已经告知用户。  
>-   已上架云市场的API，无法被删除。  
>-   已发布的API，需要先下线API，再删除。  

## 前提条件<a name="section1678010231609"></a>

-   已创建API分组和分组内的API。
-   该API不再需要提供服务。

## 操作步骤<a name="section1929412566340"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域。
3.  在服务列表中，选择“应用服务 \> API网关”，进入API网关服务管理页面。
4.  在左侧选择您的API版本，单击并进入到对应版本的API开发与调用管理页面。

    “共享版”指直接创建并管理API，如涉及到费用，以API调用次数计费。

    “专享版”指在API专享版实例中创建并管理API，如涉及到费用，按实例运行时间计费。

5.  单击“开放API \> API管理”，进入到API管理信息页面。
6.  通过以下任意一种方法，弹出“删除API”对话框。

    -   在待删除的API所在行，单击“更多 \> 删除”。
    -   单击“_API名称_”，进入API详情页面。在右上角单击“删除”。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >如果需要批量删除API，则勾选待删除的API，单击“删除”。最多同时删除1000个API。  

7.  按照提示，在输入框中输入“DELETE”，单击“确定”，完成API删除。

## 使用API方式删除API<a name="zh-cn_topic_0080101678_section7546754133419"></a>

您还可以使用API的方式删除API，具体操作请查看以下链接。

[删除API](https://support.huaweicloud.com/api-apig/apig-zh-api-180713027.html)

