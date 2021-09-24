# 对象模型<a name="ZH-CN_TOPIC_0000001082135195"></a>

API发布后，如果不想API被某些IP地址访问到，可以将这些IP地址加入黑名单，或者想API被某些特性的IP地址访问到，也可以将这些IP地址加入白名单。这样可以提高API的访问安全性，保护API免受攻击。本节介绍API的黑白名单（ACL策略）管理的对象模型，如[表1 ACL策略对象模型](AccessControlPolicyManagement-ObjectModel-9.md#ZH-CN_TOPIC_0000001082135119)所示。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   “操作类型”用于描述字段的属性，表示对应字段的值可进行的操作：
>    C：创建；U：更新；R：读取
>-   “是否必选”列表示对于“操作类型”为“C”的创建操作，对应字段是否为必选字段。

**表 1**  ACL策略对象模型

<a name="zh-cn_topic_0225568882_d0e21846"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568882_row63071936"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0225568882_p8553193"><a name="zh-cn_topic_0225568882_p8553193"></a><a name="zh-cn_topic_0225568882_p8553193"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0225568882_p21720067"><a name="zh-cn_topic_0225568882_p21720067"></a><a name="zh-cn_topic_0225568882_p21720067"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0225568882_p14495030"><a name="zh-cn_topic_0225568882_p14495030"></a><a name="zh-cn_topic_0225568882_p14495030"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0225568882_p33246761"><a name="zh-cn_topic_0225568882_p33246761"></a><a name="zh-cn_topic_0225568882_p33246761"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0225568882_p8633092"><a name="zh-cn_topic_0225568882_p8633092"></a><a name="zh-cn_topic_0225568882_p8633092"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568882_row28191856"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568882_p1838996"><a name="zh-cn_topic_0225568882_p1838996"></a><a name="zh-cn_topic_0225568882_p1838996"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568882_p14741017"><a name="zh-cn_topic_0225568882_p14741017"></a><a name="zh-cn_topic_0225568882_p14741017"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568882_p53171751"><a name="zh-cn_topic_0225568882_p53171751"></a><a name="zh-cn_topic_0225568882_p53171751"></a>黑白名单的编号</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568882_p11944549"><a name="zh-cn_topic_0225568882_p11944549"></a><a name="zh-cn_topic_0225568882_p11944549"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568882_p27984379"><a name="zh-cn_topic_0225568882_p27984379"></a><a name="zh-cn_topic_0225568882_p27984379"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568882_row50532823"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568882_p66626853"><a name="zh-cn_topic_0225568882_p66626853"></a><a name="zh-cn_topic_0225568882_p66626853"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568882_p28066016"><a name="zh-cn_topic_0225568882_p28066016"></a><a name="zh-cn_topic_0225568882_p28066016"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568882_p58754799"><a name="zh-cn_topic_0225568882_p58754799"></a><a name="zh-cn_topic_0225568882_p58754799"></a>黑白名单的名称</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568882_p61518267"><a name="zh-cn_topic_0225568882_p61518267"></a><a name="zh-cn_topic_0225568882_p61518267"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568882_p16923691"><a name="zh-cn_topic_0225568882_p16923691"></a><a name="zh-cn_topic_0225568882_p16923691"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568882_row18095492"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568882_p56448742"><a name="zh-cn_topic_0225568882_p56448742"></a><a name="zh-cn_topic_0225568882_p56448742"></a>entity_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568882_p8945376"><a name="zh-cn_topic_0225568882_p8945376"></a><a name="zh-cn_topic_0225568882_p8945376"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568882_p53486875"><a name="zh-cn_topic_0225568882_p53486875"></a><a name="zh-cn_topic_0225568882_p53486875"></a>对象类型</p>
<a name="zh-cn_topic_0225568882_ul931411563148"></a><a name="zh-cn_topic_0225568882_ul931411563148"></a><ul id="zh-cn_topic_0225568882_ul931411563148"><li>IP</li><li>DOMAIN （租户名称）</li></ul>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568882_p15141234"><a name="zh-cn_topic_0225568882_p15141234"></a><a name="zh-cn_topic_0225568882_p15141234"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568882_p18480479"><a name="zh-cn_topic_0225568882_p18480479"></a><a name="zh-cn_topic_0225568882_p18480479"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568882_row32106586"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568882_p50496654"><a name="zh-cn_topic_0225568882_p50496654"></a><a name="zh-cn_topic_0225568882_p50496654"></a>acl_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568882_p63697167"><a name="zh-cn_topic_0225568882_p63697167"></a><a name="zh-cn_topic_0225568882_p63697167"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568882_p59196868"><a name="zh-cn_topic_0225568882_p59196868"></a><a name="zh-cn_topic_0225568882_p59196868"></a>黑白名单的类型</p>
<a name="zh-cn_topic_0225568882_ul830420276155"></a><a name="zh-cn_topic_0225568882_ul830420276155"></a><ul id="zh-cn_topic_0225568882_ul830420276155"><li>PERMIT  (白名单)</li><li>DENY     (黑名单)</li></ul>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568882_p31656428"><a name="zh-cn_topic_0225568882_p31656428"></a><a name="zh-cn_topic_0225568882_p31656428"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568882_p14033838"><a name="zh-cn_topic_0225568882_p14033838"></a><a name="zh-cn_topic_0225568882_p14033838"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568882_row59195684"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568882_p30121076"><a name="zh-cn_topic_0225568882_p30121076"></a><a name="zh-cn_topic_0225568882_p30121076"></a>acl_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568882_p23888101"><a name="zh-cn_topic_0225568882_p23888101"></a><a name="zh-cn_topic_0225568882_p23888101"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568882_p55888030"><a name="zh-cn_topic_0225568882_p55888030"></a><a name="zh-cn_topic_0225568882_p55888030"></a>ip或者域名ID的值</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568882_p30636616"><a name="zh-cn_topic_0225568882_p30636616"></a><a name="zh-cn_topic_0225568882_p30636616"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568882_p65646859"><a name="zh-cn_topic_0225568882_p65646859"></a><a name="zh-cn_topic_0225568882_p65646859"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568882_row10774244162511"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568882_p477454462515"><a name="zh-cn_topic_0225568882_p477454462515"></a><a name="zh-cn_topic_0225568882_p477454462515"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568882_p1677416449253"><a name="zh-cn_topic_0225568882_p1677416449253"></a><a name="zh-cn_topic_0225568882_p1677416449253"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568882_p480522202612"><a name="zh-cn_topic_0225568882_p480522202612"></a><a name="zh-cn_topic_0225568882_p480522202612"></a>创建该ACL策略的租户编号</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568882_p86951221132617"><a name="zh-cn_topic_0225568882_p86951221132617"></a><a name="zh-cn_topic_0225568882_p86951221132617"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568882_p97741144132511"><a name="zh-cn_topic_0225568882_p97741144132511"></a><a name="zh-cn_topic_0225568882_p97741144132511"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568882_row2086724202615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568882_p186162452614"><a name="zh-cn_topic_0225568882_p186162452614"></a><a name="zh-cn_topic_0225568882_p186162452614"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568882_p1986152482614"><a name="zh-cn_topic_0225568882_p1986152482614"></a><a name="zh-cn_topic_0225568882_p1986152482614"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568882_p178614243268"><a name="zh-cn_topic_0225568882_p178614243268"></a><a name="zh-cn_topic_0225568882_p178614243268"></a>最近一次更新时间</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 ">&nbsp;&nbsp;</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 ">&nbsp;&nbsp;</td>
</tr>
</tbody>
</table>

