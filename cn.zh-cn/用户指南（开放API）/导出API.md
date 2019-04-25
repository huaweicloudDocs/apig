# 导出API<a name="apig-zh-ug-181204105"></a>

## 操作场景<a name="section25971517509"></a>

导出JSON或YAML格式的API。API网关支持单个API导出和批量API导出。

>![](public_sys-resources/icon-note.gif) **说明：**   
>云市场购买的API不支持导出。  

## 前提条件<a name="section1678010231609"></a>

已创建API分组和API。

## 操作步骤<a name="section1539513818214"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域。
3.  在服务列表中，单击“应用服务 \> API网关”，进入API网关服务管理页面。
4.  单击“导出API”，进入“导出API”界面。
5.  设置如[表1](#table11284181112369)所示参数。

    **图 1**  导出API<a name="fig699762214"></a>  
    ![](figures/导出API.png "导出API")

    **表 1**  导出API

    <a name="table11284181112369"></a>
    <table><thead align="left"><tr id="row6284151113368"><th class="cellrowborder" valign="top" width="27.35%" id="mcps1.2.3.1.1"><p id="p15990164813454"><a name="p15990164813454"></a><a name="p15990164813454"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="72.65%" id="mcps1.2.3.1.2"><p id="p99907481453"><a name="p99907481453"></a><a name="p99907481453"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3286101118369"><td class="cellrowborder" valign="top" width="27.35%" headers="mcps1.2.3.1.1 "><p id="p32861711183614"><a name="p32861711183614"></a><a name="p32861711183614"></a><span>API分组</span></p>
    </td>
    <td class="cellrowborder" valign="top" width="72.65%" headers="mcps1.2.3.1.2 "><p id="p92867112366"><a name="p92867112366"></a><a name="p92867112366"></a>选择待导出API所在的API分组。</p>
    </td>
    </tr>
    <tr id="row194915509914"><td class="cellrowborder" valign="top" width="27.35%" headers="mcps1.2.3.1.1 "><p id="p13492350591"><a name="p13492350591"></a><a name="p13492350591"></a><span>运行环境</span></p>
    </td>
    <td class="cellrowborder" valign="top" width="72.65%" headers="mcps1.2.3.1.2 "><p id="p14492105011915"><a name="p14492105011915"></a><a name="p14492105011915"></a>选择待导出API所在的环境。</p>
    </td>
    </tr>
    <tr id="row185485314913"><td class="cellrowborder" valign="top" width="27.35%" headers="mcps1.2.3.1.1 "><p id="p1211151841013"><a name="p1211151841013"></a><a name="p1211151841013"></a><span>API</span></p>
    </td>
    <td class="cellrowborder" valign="top" width="72.65%" headers="mcps1.2.3.1.2 "><p id="p954653293"><a name="p954653293"></a><a name="p954653293"></a>默认导出API分组所在环境的所有的API，如果需要导出个别API，单击“自定义导出API”，勾选需要导出的API名称。</p>
    </td>
    </tr>
    <tr id="row16234355692"><td class="cellrowborder" valign="top" width="27.35%" headers="mcps1.2.3.1.1 "><p id="p152343551892"><a name="p152343551892"></a><a name="p152343551892"></a><span>API定义范围</span></p>
    </td>
    <td class="cellrowborder" valign="top" width="72.65%" headers="mcps1.2.3.1.2 "><a name="ul51051155111915"></a><a name="ul51051155111915"></a><ul id="ul51051155111915"><li>基础定义：包括API前端请求定义和响应定义，不包括后端服务定义。其中API前端请求定义除了Swagger规范定义项外，还包括API网关的一些Swagger扩展字段。</li><li>全量定义：包括API前端请求定义、后端服务定义和响应定义。</li><li>扩展定义：包括API前端请求定义、后端服务定义和响应定义，还包括API关联的流量控制、访问控制等策略对象的定义。</li></ul>
    </td>
    </tr>
    <tr id="row188814592914"><td class="cellrowborder" valign="top" width="27.35%" headers="mcps1.2.3.1.1 "><p id="p1388125917918"><a name="p1388125917918"></a><a name="p1388125917918"></a><span>导出格式</span></p>
    </td>
    <td class="cellrowborder" valign="top" width="72.65%" headers="mcps1.2.3.1.2 "><p id="p1888155917915"><a name="p1888155917915"></a><a name="p1888155917915"></a>选择JSON或YAML。</p>
    </td>
    </tr>
    <tr id="row5847204071012"><td class="cellrowborder" valign="top" width="27.35%" headers="mcps1.2.3.1.1 "><p id="p584714017109"><a name="p584714017109"></a><a name="p584714017109"></a><span>自定义版本</span></p>
    </td>
    <td class="cellrowborder" valign="top" width="72.65%" headers="mcps1.2.3.1.2 "><p id="p128473404109"><a name="p128473404109"></a><a name="p128473404109"></a>为导出的API自定义版本号，如果没有指定版本号，默认使用当前时间。</p>
    </td>
    </tr>
    </tbody>
    </table>

6.  单击“导出”，右侧显示导出结果。

