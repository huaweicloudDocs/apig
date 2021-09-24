# 对象模型<a name="ZH-CN_TOPIC_0000001081837371"></a>

API需要绑定ACL策略，ACL策略才能够对API起到保护作用。本节介绍ACL策略与API的绑定关系的对象模型，如[表1](#zh-cn_topic_0225568892_d0e23824)所示。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   “操作类型”用于描述字段的属性，表示对应字段的值可进行的操作：
>    C：创建；U：更新；R：读取。
>-   “是否必选”列表示对于“操作类型”为“C”的创建操作，对应字段是否为必选字段。

**表 1**  api绑定acl的应用参数列表

<a name="zh-cn_topic_0225568892_d0e23824"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568892_row50624723"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0225568892_p6961916"><a name="zh-cn_topic_0225568892_p6961916"></a><a name="zh-cn_topic_0225568892_p6961916"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0225568892_p27044293"><a name="zh-cn_topic_0225568892_p27044293"></a><a name="zh-cn_topic_0225568892_p27044293"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0225568892_p43104086"><a name="zh-cn_topic_0225568892_p43104086"></a><a name="zh-cn_topic_0225568892_p43104086"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0225568892_p1770072"><a name="zh-cn_topic_0225568892_p1770072"></a><a name="zh-cn_topic_0225568892_p1770072"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0225568892_p9158130"><a name="zh-cn_topic_0225568892_p9158130"></a><a name="zh-cn_topic_0225568892_p9158130"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568892_row3611085"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568892_p24062481"><a name="zh-cn_topic_0225568892_p24062481"></a><a name="zh-cn_topic_0225568892_p24062481"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568892_p2903908"><a name="zh-cn_topic_0225568892_p2903908"></a><a name="zh-cn_topic_0225568892_p2903908"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568892_p33890033"><a name="zh-cn_topic_0225568892_p33890033"></a><a name="zh-cn_topic_0225568892_p33890033"></a>绑定关系编号</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568892_p60738142"><a name="zh-cn_topic_0225568892_p60738142"></a><a name="zh-cn_topic_0225568892_p60738142"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568892_p20842451"><a name="zh-cn_topic_0225568892_p20842451"></a><a name="zh-cn_topic_0225568892_p20842451"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568892_row53364337"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568892_p27544006"><a name="zh-cn_topic_0225568892_p27544006"></a><a name="zh-cn_topic_0225568892_p27544006"></a>front_api_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568892_p16471991"><a name="zh-cn_topic_0225568892_p16471991"></a><a name="zh-cn_topic_0225568892_p16471991"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568892_p59162926"><a name="zh-cn_topic_0225568892_p59162926"></a><a name="zh-cn_topic_0225568892_p59162926"></a>API编号</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568892_p27467664"><a name="zh-cn_topic_0225568892_p27467664"></a><a name="zh-cn_topic_0225568892_p27467664"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568892_p10288327"><a name="zh-cn_topic_0225568892_p10288327"></a><a name="zh-cn_topic_0225568892_p10288327"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568892_row25486086"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568892_p51107095"><a name="zh-cn_topic_0225568892_p51107095"></a><a name="zh-cn_topic_0225568892_p51107095"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568892_p46034032"><a name="zh-cn_topic_0225568892_p46034032"></a><a name="zh-cn_topic_0225568892_p46034032"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568892_p37769146"><a name="zh-cn_topic_0225568892_p37769146"></a><a name="zh-cn_topic_0225568892_p37769146"></a>环境的编号</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568892_p39402013"><a name="zh-cn_topic_0225568892_p39402013"></a><a name="zh-cn_topic_0225568892_p39402013"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568892_p37446464"><a name="zh-cn_topic_0225568892_p37446464"></a><a name="zh-cn_topic_0225568892_p37446464"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568892_row1473857"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568892_p52273575"><a name="zh-cn_topic_0225568892_p52273575"></a><a name="zh-cn_topic_0225568892_p52273575"></a>acl_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568892_p6301219"><a name="zh-cn_topic_0225568892_p6301219"></a><a name="zh-cn_topic_0225568892_p6301219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568892_p40636698"><a name="zh-cn_topic_0225568892_p40636698"></a><a name="zh-cn_topic_0225568892_p40636698"></a>ACL策略编号</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568892_p3238262"><a name="zh-cn_topic_0225568892_p3238262"></a><a name="zh-cn_topic_0225568892_p3238262"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568892_p60972703"><a name="zh-cn_topic_0225568892_p60972703"></a><a name="zh-cn_topic_0225568892_p60972703"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568892_row11883420"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568892_p23032930"><a name="zh-cn_topic_0225568892_p23032930"></a><a name="zh-cn_topic_0225568892_p23032930"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568892_p53728041"><a name="zh-cn_topic_0225568892_p53728041"></a><a name="zh-cn_topic_0225568892_p53728041"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568892_p57004056"><a name="zh-cn_topic_0225568892_p57004056"></a><a name="zh-cn_topic_0225568892_p57004056"></a>绑定的时间</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568892_p53925848"><a name="zh-cn_topic_0225568892_p53925848"></a><a name="zh-cn_topic_0225568892_p53925848"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568892_p5917585"><a name="zh-cn_topic_0225568892_p5917585"></a><a name="zh-cn_topic_0225568892_p5917585"></a>否</p>
</td>
</tr>
</tbody>
</table>

