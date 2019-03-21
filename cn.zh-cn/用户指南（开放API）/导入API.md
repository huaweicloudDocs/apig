# 导入API<a name="apig-zh-ug-181025104"></a>

## 操作场景<a name="section25971517509"></a>

将以Swagger 2.0定义的API导入到已有的API分组或新的API分组。

## 前提条件<a name="section1678010231609"></a>

-   已获取待导入API的Swagger文件，导入前您需要在API定义中补全API网关的[Swagger扩展定义](https://support.huaweicloud.com/devg-apig/apig-zh-dev-181109073.html)。
-   API分组和API的配额满足需求。

## 操作步骤<a name="section1539513818214"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域。
3.  在服务列表中，单击“应用服务 \> API网关”，进入API网关服务管理页面。
4.  单击“开放API \> API管理”，进入到API管理信息页面。
5.  单击“导入API”，进入“导入API”界面。
6.  选择如[表1](#table11284181112369)所示参数。

    **表 1**  导入API

    <a name="table11284181112369"></a>
    <table><thead align="left"><tr id="row6284151113368"><th class="cellrowborder" valign="top" width="27.35%" id="mcps1.2.3.1.1"><p id="p15990164813454"><a name="p15990164813454"></a><a name="p15990164813454"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="72.65%" id="mcps1.2.3.1.2"><p id="p99907481453"><a name="p99907481453"></a><a name="p99907481453"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row14286311173619"><td class="cellrowborder" valign="top" width="27.35%" headers="mcps1.2.3.1.1 "><p id="p52861411103620"><a name="p52861411103620"></a><a name="p52861411103620"></a><span>导入方式</span></p>
    </td>
    <td class="cellrowborder" valign="top" width="72.65%" headers="mcps1.2.3.1.2 "><p id="p17286171143616"><a name="p17286171143616"></a><a name="p17286171143616"></a>导入方式包含以下2种：</p>
    <a name="ul17716192483810"></a><a name="ul17716192483810"></a><ul id="ul17716192483810"><li>导入到新的分组：将API定义导入到一个新的分组，导入过程中系统会自动创建一个新的API分组，并将导入的API归属到该分组。</li><li>导入到已有分组：将API定义导入到一个已有的分组，导入过程中不会删除分组中已有的API，只是将新增的API导入分组。</li></ul>
    </td>
    </tr>
    <tr id="row3286101118369"><td class="cellrowborder" valign="top" width="27.35%" headers="mcps1.2.3.1.1 "><p id="p32861711183614"><a name="p32861711183614"></a><a name="p32861711183614"></a><span>API分组</span></p>
    </td>
    <td class="cellrowborder" valign="top" width="72.65%" headers="mcps1.2.3.1.2 "><p id="p92867112366"><a name="p92867112366"></a><a name="p92867112366"></a>仅在选择“导入到已有分组”时，需要选择API分组。</p>
    </td>
    </tr>
    <tr id="row7286711183611"><td class="cellrowborder" valign="top" width="27.35%" headers="mcps1.2.3.1.1 "><p id="p12286191116360"><a name="p12286191116360"></a><a name="p12286191116360"></a><span>是否覆盖</span></p>
    </td>
    <td class="cellrowborder" valign="top" width="72.65%" headers="mcps1.2.3.1.2 "><p id="p20286181118363"><a name="p20286181118363"></a><a name="p20286181118363"></a>仅在选择“导入到已有分组”时，需要选择是否覆盖。</p>
    <p id="p72021538134113"><a name="p72021538134113"></a><a name="p72021538134113"></a>勾选“是否覆盖”后，当导入的API定义与已有的API定义冲突时，导入的API定义会覆盖已有的API定义。</p>
    </td>
    </tr>
    <tr id="row32862011133615"><td class="cellrowborder" valign="top" width="27.35%" headers="mcps1.2.3.1.1 "><p id="p132861115369"><a name="p132861115369"></a><a name="p132861115369"></a><span>Swagger</span></p>
    </td>
    <td class="cellrowborder" valign="top" width="72.65%" headers="mcps1.2.3.1.2 "><p id="p14286151113620"><a name="p14286151113620"></a><a name="p14286151113620"></a>选择<span>Swagger</span>文件</p>
    </td>
    </tr>
    </tbody>
    </table>

7.  单击“导入”，导入成功后在API分组中查看已导入的API。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >导入的API不会自动发布到环境，需要您手动发布。  


