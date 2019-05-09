# 体验demo<a name="ZH-CN_TOPIC_0121051330"></a>

## 操作场景<a name="section2856020427"></a>

通过一键式操作，完成手机号码归属地查询API的创建、发布以及绑定流控，此demo主要用于演示API网关的使用。

此demo中，系统自动完成如下操作：

-   创建分组。
-   创建API。
-   API发布到Release环境。
-   创建流控策略。
-   API绑定流控策略。

手机号码归属地查询的业务概述：您通过HTTP GET方式调用手机号码归属地查询API，将手机号码作为入参参数传入到业务后端（业务后端为部署在华为云上的手机号码归属地查询服务），业务后端将查询到的手机号归属地信息通过response返回给您。

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   您如果需要再次体验demo，需要先将demo创建的API和API分组删除。  
>-   仅在第一体验时创建流控策略，如果再次体验前未删除，再次体验时不会再创建另一个流控策略。  

## 操作步骤<a name="section2076017329213"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域。
3.  在服务列表中，单击“应用服务 \> API网关”，进入API网关服务管理页面。
4.  单击“总览”，进入“总览”页面。
5.  单击“体验demo”，进入“体验demo”页面。
6.  单击“调用API”，进入“调试API”页面。
7.  在“Value”输入待查询的电话号码，单击“发送请求”，查看返回结果。

    -   调用成功时，返回HTTP状态码为“200”和手机号归属地信息。
    -   调试失败时，返回HTTP状态码为4_xx_或5_xx_，具体错误信息请参见[错误码](https://support.huaweicloud.com/ugcall-apig/apig-zh-ug-180530090.html)。

    **图 1**  调试API<a name="fig34366933812"></a>  
    ![](figures/调试API.png "调试API")

8.  调用API。
    1.  在“开放API \> API管理”中，单击“QueryPhoneNumber”，进入QueryPhoneNumber详情页面。
    2.  在“Dashboard”页签，在“API URL”所在行，单击![](figures/icon-copy.png)，复制URL。

        **图 2**  API详情<a name="fig185171534173819"></a>  
        ![](figures/API详情.png "API详情")

    3.  在浏览器中粘贴URL，并将\{phoneNumber\}改为待查询的电话号码，按“Enter”，查看此电话号码所在地。

        **图 3**  调用结果<a name="fig104292210399"></a>  
        ![](figures/调用结果.png "调用结果")



