# HTTP响应头管理插件<a name="ZH-CN_TOPIC_0000001142797430"></a>

API响应是指API网关返回客户端的响应，HTTP响应头是API响应中的一部分。您可以自定义HTTP响应头，在返回的API响应中指定您配置的响应头。

>![](public_sys-resources/icon-note.gif) **说明：** 
>2021年6月1日后创建的专享版实例支持HTTP响应头管理插件，在这之前创建的专享版实例不支持HTTP响应头管理插件，如需使用HTTP响应头管理插件，请联系客服。

## 使用限制<a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_section12218718182910"></a>

无法修改API网关增加的系统响应头（x-apig-\*，x-request-id等），包括API网关提供的CORS功能增加的响应头。

## 配置参数说明<a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_section16297425153118"></a>

**表 1**  配置参数说明

<a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_table1729413173312"></a>
<table><thead align="left"><tr id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_row2295151173317"><th class="cellrowborder" valign="top" width="30%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p52954133313"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p52954133313"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p52954133313"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="70%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p122957183311"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p122957183311"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p122957183311"></a>配置说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_row1529515133316"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p1629516133316"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p1629516133316"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p1629516133316"></a>Name</p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p1429531183316"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p1429531183316"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p1429531183316"></a>响应头名称。每个插件中不能添加重复名称的响应头（不区分大小写），且最多添加10条响应头。</p>
</td>
</tr>
<tr id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_row42958115339"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p172954116336"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p172954116336"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p172954116336"></a>Value</p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p5296101123313"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p5296101123313"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p5296101123313"></a>响应头的值。当“Action”为“Delete”时响应头的值不生效，可为空。</p>
</td>
</tr>
<tr id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_row129610114337"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p12296119332"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p12296119332"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p12296119332"></a>Action</p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p1429614113316"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p1429614113316"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p1429614113316"></a>响应头操作，您可以覆盖、添加、删除、跳过或新增指定的响应头。</p>
<p id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p211901261212"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p211901261212"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p211901261212"></a><strong id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_b11119412121215"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_b11119412121215"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_b11119412121215"></a>Override</strong>：覆盖</p>
<a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_ul177611084358"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_ul177611084358"></a><ul id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_ul177611084358"><li>当API响应中存在指定的响应头时，使用当前响应头的值覆盖已有响应头的值。</li><li>当API响应中存在多个与指定响应头相同名称的响应头时，该操作只会按当前响应头的值返回一条响应头记录。</li><li>当API响应中不存在指定的响应头时，添加当前响应头。</li></ul>
<p id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p9430171916221"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p9430171916221"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p9430171916221"></a><strong id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_b1343019199221"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_b1343019199221"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_b1343019199221"></a>Append</strong>：添加</p>
<a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_ul1995021243516"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_ul1995021243516"></a><ul id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_ul1995021243516"><li>当API响应中存在指定的响应头时，使用当前响应头的值覆盖已有响应头的值。</li><li>当API响应中存在多个与指定响应头相同名称的响应头时，会将多个响应头的值用“，”拼接后，再添加当前响应头的值。</li><li>当API响应中不存在指定的响应头时，添加当前响应头。</li></ul>
<p id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p10602134393520"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p10602134393520"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p10602134393520"></a><strong id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_b1860215431354"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_b1860215431354"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_b1860215431354"></a>Delete</strong>：删除</p>
<a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_ul19161951183514"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_ul19161951183514"></a><ul id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_ul19161951183514"><li>当API响应中存在指定的响应头时，删除当前响应头。</li><li>当API响应中存在多个与指定响应头相同名称的响应头时，删除所有相同名称的响应头。</li></ul>
<p id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p10551327163812"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p10551327163812"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p10551327163812"></a><strong id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_b1955827173819"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_b1955827173819"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_b1955827173819"></a>Skip</strong>：跳过</p>
<a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_ul64522037123815"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_ul64522037123815"></a><ul id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_ul64522037123815"><li>当API响应中存在指定的响应头时，跳过当前响应头。</li><li>当API响应中存在多个与指定响应头相同名称的响应头时，均不作处理直接返回。</li><li>当API响应中不存在指定的响应头时，添加当前响应头。</li></ul>
<p id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p26161441144012"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p26161441144012"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p26161441144012"></a><strong id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_b16162041134012"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_b16162041134012"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_b16162041134012"></a>Add</strong>：新增</p>
<p id="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p134551528238"><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p134551528238"></a><a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_p134551528238"></a>无论API响应中是否存在指定的响应头，都添加当前响应头。</p>
</td>
</tr>
</tbody>
</table>

## 脚本配置示例<a name="zh-cn_topic_0000001128377392_zh-cn_topic_0000001117215264_section1665538193019"></a>

```
{
    "response_headers": [
        {
            "name": "test",
            "value": "test",
            "action": "append"
        },
        {
            "name": "test1",
            "value": "test1",
            "action": "override"
        }
    ]
}
```

