# 创建用户并授权使用API网关<a name="apig-ug-190529109"></a>

如果您需要对您所拥有的API网关服务进行权限管理，您可以使用[统一身份认证服务](https://support.huaweicloud.com/usermanual-iam/zh-cn_topic_0079496985.html)（Identity and Access Management，简称IAM），通过IAM，您可以：

-   根据企业的业务组织，在您的华为云账号中，给企业中不同职能部门的员工创建IAM用户，让员工拥有唯一安全凭证，并使用API网关服务资源。
-   根据企业用户的职能，设置不同的访问权限，以达到用户之间的权限隔离。
-   将API网关服务资源委托给更专业、高效的其他华为云账号或者云服务，这些账号或者云服务可以根据权限进行代运维。

如果华为云账号已经能满足您的要求，不需要创建独立的IAM用户，您可以跳过本章节，不影响您使用API网关服务的功能。

本章节为您介绍对用户授权的方法，操作流程如[图1](#zh-cn_topic_0170877287_fig15451536531)所示。

## 前提条件<a name="zh-cn_topic_0170877287_section17723185741610"></a>

给用户组授权之前，请您了解用户组可以添加的[API网关服务系统策略](#table1934161212122)，并结合实际需求进行选择。若您需要对除API网关服务之外的其它服务授权，IAM支持服务的所有策略请参见[权限策略](https://support.huaweicloud.com/usermanual-permissions/zh-cn_topic_0063498930.html)。

**表 1**  API网关服务系统策略

<a name="table1934161212122"></a>
<table><thead align="left"><tr id="row17131111218122"><th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.4.1.1"><p id="p14131131231217"><a name="p14131131231217"></a><a name="p14131131231217"></a>策略名称</p>
</th>
<th class="cellrowborder" valign="top" width="28.037196280371962%" id="mcps1.2.4.1.2"><p id="p141311112151214"><a name="p141311112151214"></a><a name="p141311112151214"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="54.61453854614538%" id="mcps1.2.4.1.3"><p id="p7131912181212"><a name="p7131912181212"></a><a name="p7131912181212"></a>操作</p>
</th>
</tr>
</thead>
<tbody><tr id="row17132191291216"><td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.4.1.1 "><p id="p1413231216124"><a name="p1413231216124"></a><a name="p1413231216124"></a>APIG Administrator</p>
</td>
<td class="cellrowborder" valign="top" width="28.037196280371962%" headers="mcps1.2.4.1.2 "><p id="p41321012191210"><a name="p41321012191210"></a><a name="p41321012191210"></a>API网关服务的管理员权限。</p>
</td>
<td class="cellrowborder" valign="top" width="54.61453854614538%" headers="mcps1.2.4.1.3 "><p id="p188281101814"><a name="p188281101814"></a><a name="p188281101814"></a>创建API、发布API、删除API等</p>
</td>
</tr>
</tbody>
</table>

## 示例流程<a name="zh-cn_topic_0170877287_section1189416161520"></a>

**图 1**  给用户授权API网关服务权限流程<a name="zh-cn_topic_0170877287_fig15451536531"></a>  
![](figures/给用户授权API网关服务权限流程.png "给用户授权API网关服务权限流程")

1.  <a name="zh-cn_topic_0170877287_li10176121316284"></a>[创建用户组并授权](https://support.huaweicloud.com/usermanual-iam/zh-cn_topic_0046611269.html)

    在IAM控制台创建用户组，并授予API网关服务的权限“APIG Administrator”。

2.  [创建用户并加入用户组](https://support.huaweicloud.com/usermanual-iam/zh-cn_topic_0046611303.html)

    在IAM控制台创建用户，并将其加入[1](#zh-cn_topic_0170877287_li10176121316284)中创建的用户组。

3.  [用户登录](https://support.huaweicloud.com/usermanual-iam/iam_01_0552.html)并验证权限

    新创建的用户登录控制台，验证API网关服务的权限。


## API网关系统策略说明<a name="section56559289544"></a>

API网关当前只有一个系统策略，名称为“APIG Administrator”。

```
{
        "Version": "1.0",
        "Statement": [
                {
                        "Effect": "Allow",
                        "Action": [
                                "apig:*:*"
                        ]
                }
        ]
}
```

<a name="table33321739133117"></a>
<table><thead align="left"><tr id="row645212399314"><th class="cellrowborder" colspan="2" valign="top" id="mcps1.1.5.1.1"><p id="p14452153933119"><a name="p14452153933119"></a><a name="p14452153933119"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" id="mcps1.1.5.1.2"><p id="p34521839193112"><a name="p34521839193112"></a><a name="p34521839193112"></a>含义</p>
</th>
<th class="cellrowborder" valign="top" id="mcps1.1.5.1.3"><p id="p20452173933117"><a name="p20452173933117"></a><a name="p20452173933117"></a>值</p>
</th>
</tr>
</thead>
<tbody><tr id="row7452203973118"><td class="cellrowborder" colspan="2" valign="top" headers="mcps1.1.5.1.1 "><p id="p7452163911319"><a name="p7452163911319"></a><a name="p7452163911319"></a>Version</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.5.1.2 "><p id="p8453193903116"><a name="p8453193903116"></a><a name="p8453193903116"></a>策略的版本</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.5.1.3 "><p id="p14531039103116"><a name="p14531039103116"></a><a name="p14531039103116"></a>固定为“1.0”</p>
</td>
</tr>
<tr id="row1645315392311"><td class="cellrowborder" rowspan="2" valign="top" width="17.22172217221722%" headers="mcps1.1.5.1.1 "><p id="p5453133973114"><a name="p5453133973114"></a><a name="p5453133973114"></a>Statement</p>
</td>
<td class="cellrowborder" valign="top" width="17.121712171217123%" headers="mcps1.1.5.1.1 "><p id="p94531397312"><a name="p94531397312"></a><a name="p94531397312"></a>Effect</p>
</td>
<td class="cellrowborder" valign="top" width="28.28282828282828%" headers="mcps1.1.5.1.2 "><p id="p12453339123116"><a name="p12453339123116"></a><a name="p12453339123116"></a>定义Action中所包含的具体操作是否允许执行。</p>
</td>
<td class="cellrowborder" valign="top" width="37.37373737373737%" headers="mcps1.1.5.1.3 "><a name="ul14535391313"></a><a name="ul14535391313"></a><ul id="ul14535391313"><li>Allow：允许执行。</li><li>Deny：不允许执行。</li></ul>
</td>
</tr>
<tr id="row9453153910318"><td class="cellrowborder" valign="top" headers="mcps1.1.5.1.1 "><p id="p194532391314"><a name="p194532391314"></a><a name="p194532391314"></a>Action</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.5.1.1 "><p id="p1945319396315"><a name="p1945319396315"></a><a name="p1945319396315"></a>定义对API网关的具体操作。</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.5.1.2 "><p id="p3453103914318"><a name="p3453103914318"></a><a name="p3453103914318"></a>格式为：服务名:资源类型:操作</p>
<p id="p8453193916312"><a name="p8453193916312"></a><a name="p8453193916312"></a>"apig:*:*"，其中apig为服务名称；“*”为通配符，表示对所有资源类型可以执行所有操作。</p>
</td>
</tr>
</tbody>
</table>

