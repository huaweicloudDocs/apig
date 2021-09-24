# 对象模型<a name="ZH-CN_TOPIC_0000001081976185"></a>

本节介绍环境变量的对象模型，如下表所示：

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   “操作类型”用于描述字段的属性，表示对应字段的值可进行的操作：
>    C：创建；U：更新；R：读取。
>-   “是否必选”列表示对于“操作类型”为“C”的创建操作，对应字段是否为必选字段。

**表 1**  环境变量对象模型

<a name="zh-cn_topic_0225568854_table15446427"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568854_row13652882"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0225568854_p32141673"><a name="zh-cn_topic_0225568854_p32141673"></a><a name="zh-cn_topic_0225568854_p32141673"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0225568854_p53338749"><a name="zh-cn_topic_0225568854_p53338749"></a><a name="zh-cn_topic_0225568854_p53338749"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0225568854_p25471413"><a name="zh-cn_topic_0225568854_p25471413"></a><a name="zh-cn_topic_0225568854_p25471413"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0225568854_p49918586"><a name="zh-cn_topic_0225568854_p49918586"></a><a name="zh-cn_topic_0225568854_p49918586"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0225568854_p16873651"><a name="zh-cn_topic_0225568854_p16873651"></a><a name="zh-cn_topic_0225568854_p16873651"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568854_row24588489"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568854_p45510563"><a name="zh-cn_topic_0225568854_p45510563"></a><a name="zh-cn_topic_0225568854_p45510563"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568854_p62476969"><a name="zh-cn_topic_0225568854_p62476969"></a><a name="zh-cn_topic_0225568854_p62476969"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568854_p27469765"><a name="zh-cn_topic_0225568854_p27469765"></a><a name="zh-cn_topic_0225568854_p27469765"></a>环境变量编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568854_p10458460"><a name="zh-cn_topic_0225568854_p10458460"></a><a name="zh-cn_topic_0225568854_p10458460"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568854_p41828952"><a name="zh-cn_topic_0225568854_p41828952"></a><a name="zh-cn_topic_0225568854_p41828952"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568854_row40916256"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568854_p25882414"><a name="zh-cn_topic_0225568854_p25882414"></a><a name="zh-cn_topic_0225568854_p25882414"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568854_p16100756"><a name="zh-cn_topic_0225568854_p16100756"></a><a name="zh-cn_topic_0225568854_p16100756"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568854_p29092859"><a name="zh-cn_topic_0225568854_p29092859"></a><a name="zh-cn_topic_0225568854_p29092859"></a>环境编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568854_p7711370"><a name="zh-cn_topic_0225568854_p7711370"></a><a name="zh-cn_topic_0225568854_p7711370"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568854_p20641258"><a name="zh-cn_topic_0225568854_p20641258"></a><a name="zh-cn_topic_0225568854_p20641258"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568854_row51553600"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568854_p15092060"><a name="zh-cn_topic_0225568854_p15092060"></a><a name="zh-cn_topic_0225568854_p15092060"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568854_p14497308"><a name="zh-cn_topic_0225568854_p14497308"></a><a name="zh-cn_topic_0225568854_p14497308"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568854_p33431272"><a name="zh-cn_topic_0225568854_p33431272"></a><a name="zh-cn_topic_0225568854_p33431272"></a>API分组编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568854_p23578537"><a name="zh-cn_topic_0225568854_p23578537"></a><a name="zh-cn_topic_0225568854_p23578537"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568854_p30813383"><a name="zh-cn_topic_0225568854_p30813383"></a><a name="zh-cn_topic_0225568854_p30813383"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568854_row8884996"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568854_p48596088"><a name="zh-cn_topic_0225568854_p48596088"></a><a name="zh-cn_topic_0225568854_p48596088"></a>variable_name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568854_p43969019"><a name="zh-cn_topic_0225568854_p43969019"></a><a name="zh-cn_topic_0225568854_p43969019"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568854_p4720824"><a name="zh-cn_topic_0225568854_p4720824"></a><a name="zh-cn_topic_0225568854_p4720824"></a>变量名</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568854_p46842453"><a name="zh-cn_topic_0225568854_p46842453"></a><a name="zh-cn_topic_0225568854_p46842453"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568854_p36142330"><a name="zh-cn_topic_0225568854_p36142330"></a><a name="zh-cn_topic_0225568854_p36142330"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568854_row56845520"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568854_p41084373"><a name="zh-cn_topic_0225568854_p41084373"></a><a name="zh-cn_topic_0225568854_p41084373"></a>variable_value</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568854_p39499894"><a name="zh-cn_topic_0225568854_p39499894"></a><a name="zh-cn_topic_0225568854_p39499894"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568854_p45374877"><a name="zh-cn_topic_0225568854_p45374877"></a><a name="zh-cn_topic_0225568854_p45374877"></a>变量值</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568854_p51486383"><a name="zh-cn_topic_0225568854_p51486383"></a><a name="zh-cn_topic_0225568854_p51486383"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568854_p9647510"><a name="zh-cn_topic_0225568854_p9647510"></a><a name="zh-cn_topic_0225568854_p9647510"></a>是</p>
</td>
</tr>
</tbody>
</table>

