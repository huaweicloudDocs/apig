# 创建API分组<a name="apig-zh-ug-180307003"></a>

## 操作场景<a name="section1731012541118"></a>

API分组相当于API的集合，API提供方以API分组为单位，管理分组内的所有API。

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   一个API只能属于某一个API分组。  
>-   每个用户最多创建50个API分组。  

## 操作步骤<a name="section8731554122615"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域。
3.  在服务列表中，单击“应用服务 \> API网关”，进入API网关服务管理页面。
4.  单击“开放API \> API分组”，进入到API分组信息页面。
5.  单击“创建分组”，弹出“创建分组”对话框。填写如[表1](#table195413315428)所示信息。

    **表 1**  分组信息表

    <a name="table195413315428"></a>
    <table><thead align="left"><tr id="row45523384220"><th class="cellrowborder" valign="top" width="18%" id="mcps1.2.4.1.1"><p id="p65563314423"><a name="p65563314423"></a><a name="p65563314423"></a>信息项</p>
    </th>
    <th class="cellrowborder" valign="top" width="40%" id="mcps1.2.4.1.2"><p id="p356183311427"><a name="p356183311427"></a><a name="p356183311427"></a>描述</p>
    </th>
    <th class="cellrowborder" valign="top" width="42%" id="mcps1.2.4.1.3"><p id="p756163324216"><a name="p756163324216"></a><a name="p756163324216"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1156183364219"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="p105616333427"><a name="p105616333427"></a><a name="p105616333427"></a>分组名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.2 "><p id="p1656123374219"><a name="p1656123374219"></a><a name="p1656123374219"></a>API分组名称，用于将API接口进行分组管理。</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.4.1.3 "><a name="ul1534415125011"></a><a name="ul1534415125011"></a><ul id="ul1534415125011"><li>必须以英文或汉字开头。</li><li>支持汉字、英文、数字和下划线。</li><li>长度为3 ~ 64个字符。</li></ul>
    </td>
    </tr>
    <tr id="row14879114316433"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="p12880154304320"><a name="p12880154304320"></a><a name="p12880154304320"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.2 "><p id="p48801043134312"><a name="p48801043134312"></a><a name="p48801043134312"></a>对分组的介绍</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.4.1.3 "><p id="p8880154374314"><a name="p8880154374314"></a><a name="p8880154374314"></a>长度不超过255个字符。</p>
    </td>
    </tr>
    </tbody>
    </table>

6.  完成分组信息填写后，单击“确定”，创建API分组。

    创建分组成功后，在“API分组”页面的列表中显示新创建的API分组。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >-   API分组创建后，系统为分组自动分配一个内部测试用的子域名，此子域名每天最多可以访问1000次。  
    >-   对外开放API时，您需要为API分组绑定您自己的独立域名。  


