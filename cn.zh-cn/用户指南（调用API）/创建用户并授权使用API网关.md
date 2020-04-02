# 创建用户并授权使用API网关<a name="apig-ug-190529109"></a>

如果您需要对您所拥有的API网关服务进行权限管理，您可以使用[统一身份认证服务](https://support.huaweicloud.com/usermanual-iam/iam_01_0001.html)（Identity and Access Management，简称IAM），通过IAM，您可以：

-   根据企业的业务组织，在您的华为云账号中，给企业中不同职能部门的员工创建IAM用户，让员工拥有唯一安全凭证，并使用API网关服务资源。
-   根据企业用户的职能，设置不同的访问权限，以达到用户之间的权限隔离。
-   将API网关服务资源委托给更专业、高效的其他华为云账号或者云服务，这些账号或者云服务可以根据权限进行代运维。

如果华为云账号已经能满足您的要求，不需要创建独立的IAM用户，您可以跳过本章节，不影响您使用API网关服务的功能。

本章节为您介绍对用户授权的方法，操作流程如[图1](#zh-cn_topic_0170877287_fig15451536531)所示。

## 前提条件<a name="zh-cn_topic_0170877287_section17723185741610"></a>

给用户组授权之前，请您了解用户组可以添加的[表1](#table13382143731910)，并结合实际需求进行选择。若您需要对除API网关服务之外的其它服务授权，IAM支持服务的所有策略请参见[权限策略](https://support.huaweicloud.com/usermanual-permissions/iam_01_0001.html)。

**表 1**  API网关的系统角色或策略

<a name="table13382143731910"></a>
<table><thead align="left"><tr id="row10382193761919"><th class="cellrowborder" valign="top" width="16.04%" id="mcps1.2.5.1.1"><p id="p538314372199"><a name="p538314372199"></a><a name="p538314372199"></a>系统角色/策略名称</p>
</th>
<th class="cellrowborder" valign="top" width="36.53%" id="mcps1.2.5.1.2"><p id="p638393718193"><a name="p638393718193"></a><a name="p638393718193"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="17.18%" id="mcps1.2.5.1.3"><p id="p1138363718194"><a name="p1138363718194"></a><a name="p1138363718194"></a>类别</p>
</th>
<th class="cellrowborder" valign="top" width="30.25%" id="mcps1.2.5.1.4"><p id="p2078410663110"><a name="p2078410663110"></a><a name="p2078410663110"></a>依赖关系</p>
</th>
</tr>
</thead>
<tbody><tr id="row238315376192"><td class="cellrowborder" valign="top" width="16.04%" headers="mcps1.2.5.1.1 "><p id="p14383143721913"><a name="p14383143721913"></a><a name="p14383143721913"></a>APIG Administrator</p>
</td>
<td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.2.5.1.2 "><p id="p038363721913"><a name="p038363721913"></a><a name="p038363721913"></a>API网关服务的管理员权限。拥有该权限的用户可以使用<strong id="b18885142014"><a name="b18885142014"></a><a name="b18885142014"></a>共享版</strong>API网关服务的所有功能。</p>
</td>
<td class="cellrowborder" valign="top" width="17.18%" headers="mcps1.2.5.1.3 "><p id="p1638343771915"><a name="p1638343771915"></a><a name="p1638343771915"></a>系统角色</p>
</td>
<td class="cellrowborder" valign="top" width="30.25%" headers="mcps1.2.5.1.4 "><a name="ul1882803818238"></a><a name="ul1882803818238"></a><ul id="ul1882803818238"><li>使用VPC通道时，用户还需具备VPC Administrator角色权限</li><li>使用自定义认证功能，用户还需具备FunctionGraph Administrator角色权限。</li></ul>
</td>
</tr>
<tr id="row29471637175418"><td class="cellrowborder" valign="top" width="16.04%" headers="mcps1.2.5.1.1 "><p id="p1594818373542"><a name="p1594818373542"></a><a name="p1594818373542"></a>APIG FullAccess</p>
</td>
<td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.2.5.1.2 "><p id="p99480376545"><a name="p99480376545"></a><a name="p99480376545"></a>API网关服务所有权限。拥有该权限的用户可以使用<strong id="b18522018182014"><a name="b18522018182014"></a><a name="b18522018182014"></a>专享版</strong>API网关服务的所有功能。</p>
</td>
<td class="cellrowborder" valign="top" width="17.18%" headers="mcps1.2.5.1.3 "><p id="p2948123718546"><a name="p2948123718546"></a><a name="p2948123718546"></a>系统策略</p>
</td>
<td class="cellrowborder" valign="top" width="30.25%" headers="mcps1.2.5.1.4 "><p id="p878476183110"><a name="p878476183110"></a><a name="p878476183110"></a>无。</p>
</td>
</tr>
<tr id="row17372113817546"><td class="cellrowborder" valign="top" width="16.04%" headers="mcps1.2.5.1.1 "><p id="p43721838135417"><a name="p43721838135417"></a><a name="p43721838135417"></a>APIG ReadOnlyAccess</p>
</td>
<td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.2.5.1.2 "><p id="p1227810374218"><a name="p1227810374218"></a><a name="p1227810374218"></a>API网关服务的只读访问权限。拥有该权限的用户只能查看<strong id="b10277193715213"><a name="b10277193715213"></a><a name="b10277193715213"></a>专享版</strong>API网关的各类信息。</p>
</td>
<td class="cellrowborder" valign="top" width="17.18%" headers="mcps1.2.5.1.3 "><p id="p1537210382547"><a name="p1537210382547"></a><a name="p1537210382547"></a>系统策略</p>
</td>
<td class="cellrowborder" valign="top" width="30.25%" headers="mcps1.2.5.1.4 "><p id="p17244141916304"><a name="p17244141916304"></a><a name="p17244141916304"></a>无。</p>
</td>
</tr>
</tbody>
</table>

## 示例流程<a name="zh-cn_topic_0170877287_section1189416161520"></a>

**图 1**  给用户授权API网关服务权限流程<a name="zh-cn_topic_0170877287_fig15451536531"></a>  
![](figures/给用户授权API网关服务权限流程.png "给用户授权API网关服务权限流程")

1.  <a name="zh-cn_topic_0170877287_li10176121316284"></a>[创建用户组并授权](https://support.huaweicloud.com/usermanual-iam/iam_03_0001.html)

    在IAM控制台创建用户组，并授予API网关服务的权限“APIG Administrator”或“APIG FullAccess”。

2.  [创建用户并加入用户组](https://support.huaweicloud.com/usermanual-iam/iam_02_0001.html)

    在IAM控制台创建用户，并将其加入[1](#zh-cn_topic_0170877287_li10176121316284)中创建的用户组。

3.  [用户登录](https://support.huaweicloud.com/usermanual-iam/iam_01_0552.html)并验证权限

    新创建的用户登录控制台，验证API网关服务的权限。


