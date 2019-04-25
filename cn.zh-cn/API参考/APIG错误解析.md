# APIG错误解析<a name="apig-zh-api-180713212"></a>

API调用发生错误时，会有错误信息返回，本章节主要介绍错误信息的结构。

错误结构体中包含：

-   error\_msg：错误描述，用于陈述错误发生的原因。
-   error\_code：错误的唯一编码。

返回结构体示例如下：

```
{
	"error_code": "APIG.1001",
	"error_msg": "token expired"
}
```

