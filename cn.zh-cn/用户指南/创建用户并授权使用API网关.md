# 创建用户并授权使用API网关<a name="ZH-CN_TOPIC_0000001188957147"></a>

如果您需要对您所拥有的API网关服务进行权限管理，您可以使用[统一身份认证服务](https://support.huaweicloud.com/usermanual-iam/iam_01_0001.html)（Identity and Access Management，简称IAM），通过IAM，您可以：

-   根据企业的业务组织，在您的华为云帐号中，给企业中不同职能部门的员工创建IAM用户，让员工拥有唯一安全凭证，并使用API网关服务资源。
-   根据企业用户的职能，设置不同的访问权限，以达到用户之间的权限隔离。
-   将API网关服务资源委托给更专业、高效的其他华为云帐号或者云服务，这些帐号或者云服务可以根据权限进行代运维。

如果华为云帐号已经能满足您的要求，不需要创建独立的IAM用户，您可以跳过本章节，不影响您使用API网关服务的功能。

本章节为您介绍对用户授权的方法，操作流程如[图1](#zh-cn_topic_0000001174416917_zh-cn_topic_0172480077_zh-cn_topic_0170877287_fig15451536531)所示。

## 前提条件<a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172480077_zh-cn_topic_0170877287_section17723185741610"></a>

给用户组授权之前，请您了解用户组可以添加的[表1](#zh-cn_topic_0000001174416917_zh-cn_topic_0172480077_table13382143731910)，并结合实际需求进行选择。若您需要对除API网关服务之外的其它服务授权，IAM支持服务的所有策略请参见[权限策略](https://support.huaweicloud.com/usermanual-permissions/iam_01_0001.html)。

**表 1**  API网关的系统角色或策略

<a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172480077_table13382143731910"></a>
<table><thead align="left"><tr id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_row17131111218122"><th class="cellrowborder" valign="top" width="16.04%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p14131131231217"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p14131131231217"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p14131131231217"></a>系统角色/策略名称</p>
</th>
<th class="cellrowborder" valign="top" width="36.53%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p141311112151214"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p141311112151214"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p141311112151214"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="17.18%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p7131912181212"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p7131912181212"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p7131912181212"></a>类别</p>
</th>
<th class="cellrowborder" valign="top" width="30.25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p2078410663110"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p2078410663110"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p2078410663110"></a>依赖关系</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_row17132191291216"><td class="cellrowborder" valign="top" width="16.04%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p1413231216124"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p1413231216124"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p1413231216124"></a>APIG Administrator</p>
</td>
<td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p41321012191210"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p41321012191210"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p41321012191210"></a>API网关服务的管理员权限。拥有该权限的用户可以使用<strong id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_b296282316429"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_b296282316429"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_b296282316429"></a>共享版</strong>和<strong id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_b106352081619"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_b106352081619"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_b106352081619"></a>专享版</strong>API网关服务的所有功能。</p>
</td>
<td class="cellrowborder" valign="top" width="17.18%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p188281101814"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p188281101814"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p188281101814"></a>系统角色</p>
</td>
<td class="cellrowborder" valign="top" width="30.25%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_ul1882803818238"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_ul1882803818238"></a><ul id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_ul1882803818238"><li>使用VPC通道时，用户还需具备VPC Administrator角色权限</li><li>使用自定义认证功能，用户还需具备FunctionGraph Administrator角色权限。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_row29471637175418"><td class="cellrowborder" valign="top" width="16.04%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p1594818373542"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p1594818373542"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p1594818373542"></a>APIG FullAccess</p>
</td>
<td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p99480376545"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p99480376545"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p99480376545"></a>API网关服务所有权限。拥有该权限的用户可以使用<strong id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_b84662213421"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_b84662213421"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_b84662213421"></a>专享版</strong>API网关服务的所有功能。</p>
</td>
<td class="cellrowborder" valign="top" width="17.18%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p2948123718546"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p2948123718546"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p2948123718546"></a>系统策略</p>
</td>
<td class="cellrowborder" valign="top" width="30.25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p878476183110"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p878476183110"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p878476183110"></a>无。</p>
</td>
</tr>
<tr id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_row17372113817546"><td class="cellrowborder" valign="top" width="16.04%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p43721838135417"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p43721838135417"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p43721838135417"></a>APIG ReadOnlyAccess</p>
</td>
<td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p1437213819540"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p1437213819540"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p1437213819540"></a>API网关服务的只读访问权限。拥有该权限的用户只能查看<strong id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_b1674375154712"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_b1674375154712"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_b1674375154712"></a>专享版</strong>API网关的各类信息。</p>
</td>
<td class="cellrowborder" valign="top" width="17.18%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p1537210382547"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p1537210382547"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p1537210382547"></a>系统策略</p>
</td>
<td class="cellrowborder" valign="top" width="30.25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p17244141916304"><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p17244141916304"></a><a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172474100_p17244141916304"></a>无。</p>
</td>
</tr>
</tbody>
</table>

## 示例流程<a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172480077_zh-cn_topic_0170877287_section1189416161520"></a>

**图 1**  给用户授权API网关服务权限流程<a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172480077_zh-cn_topic_0170877287_fig15451536531"></a>  
![](figures/给用户授权API网关服务权限流程.png "给用户授权API网关服务权限流程")

1.  <a name="zh-cn_topic_0000001174416917_zh-cn_topic_0172480077_zh-cn_topic_0170877287_li10176121316284"></a>[创建用户组并授权](https://support.huaweicloud.com/usermanual-iam/iam_03_0001.html)

    在IAM控制台创建用户组，并授予API网关服务的权限“APIG Administrator”或“APIG FullAccess”。

2.  [创建用户并加入用户组](https://support.huaweicloud.com/usermanual-iam/iam_02_0001.html)

    在IAM控制台创建用户，并将其加入[1](#zh-cn_topic_0000001174416917_zh-cn_topic_0172480077_zh-cn_topic_0170877287_li10176121316284)中创建的用户组。

3.  [用户登录](https://support.huaweicloud.com/usermanual-iam/iam_01_0552.html)并验证权限

    新创建的用户登录控制台，验证API网关服务的权限。


