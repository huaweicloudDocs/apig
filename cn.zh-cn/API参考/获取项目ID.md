# 获取项目ID<a name="ZH-CN_TOPIC_0000001081976241"></a>

## 调用API获取项目ID<a name="zh-cn_topic_0172449255_section414113577116"></a>

项目ID还可通过调用[查询指定条件下的项目信息](https://support.huaweicloud.com/api-iam/iam_06_0001.html)API获取。

获取项目ID的接口为“GET https://\{Endpoint\}/v3/projects/”，其中\{Endpoint\}为IAM的终端节点，可以从[地区与终端节点](https://developer.huaweicloud.com/dev/endpoint)获取。接口的认证鉴权请参见[认证鉴权](认证鉴权.md#ZH-CN_TOPIC_0000001082221165)。

响应示例如下，其中projects下的“id”即为项目ID。

```
{
    "projects": [
        {
            "domain_id": "65382450e8f64ac0870cd180d14e684b",
            "is_domain": false,
            "parent_id": "65382450e8f64ac0870cd180d14e684b",
            "name": "xx-north-4",
            "description": "",
            "links": {
                "next": null,
                "previous": null,
                "self": "https://www.example.com/v3/projects/a4a5d4098fb4474fa22cd05f897d6b99"
            },
            "id": "a4a5d4098fb4474fa22cd05f897d6b99",
            "enabled": true
        }
    ],
    "links": {
        "next": null,
        "previous": null,
        "self": "https://www.example.com/v3/projects"
    }
}
```

## 从控制台获取项目ID<a name="zh-cn_topic_0172449255_section15182163514118"></a>

在调用接口的时候，部分URL中需要填入项目编号，所以需要获取到项目编号。项目编号获取步骤如下：

1.  登录管理控制台。
2.  单击用户名，在下拉列表中单击“我的凭证”。

    在“API凭证”页面的项目列表中查看项目ID。

    **图 1**  查看项目ID<a name="zh-cn_topic_0172449255_fig27431423193018"></a>  
    ![](figures/查看项目ID.png "查看项目ID")

    多项目时，展开“所属区域”，从“项目ID”列获取子项目ID。


