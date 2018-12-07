# Token认证<a name="apig-zh-api-180713004"></a>

## 应用场景<a name="section5608799912249"></a>

当您请求API网关的接口并选择使用Token认证方式进行认证时，需要在请求消息头中携带Token信息，携带的方式为：在请求消息头中设置“X-Auth-Token”。

本节介绍如何调用接口完成Token认证。

## Token的获取方式<a name="section3546598312249"></a>

1.  <a name="li17145102315153"></a>获取Token，请参考[获取用户Token](http://support.huaweicloud.com/api-iam/zh-cn_topic_0057845583.html)。发送“**POST https://_IAM的Endpoint_/v3/auth/tokens**”，获取IAM的Endpoint及消息体中的区域名称，请参考[地区和终端节点](http://developer.huaweicloud.com/endpoint.html)。请求消息体中的project的id的获取方式请参考[获取项目编号](获取项目编号.md)。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。

    请求内容示例如下：

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >下面示例代码中的password、username、domainname和id需要替换为实际内容，详情请参考《_统一身份认证服务API参考_》。  

    ```
    {
    	"auth": {
    		"identity": {
    			"methods": ["password"],
    			"password": {
    				"user": {
    					"name": "username",
    					"password": "password",
    					"domain": {
    						"name": "domainname"
    					}
    				}
    			}
    		},
    		"scope": {
    			"project": {
    				"id": "0215ef11e49d4743be23dd97a1561e91"//假设id是"0215ef11e49d4743be23dd97a1561e91"
    			}
    		}
    	}
    }
    ```

2.  调用业务接口，在请求消息头中增加“X-Auth-Token”，“X-Auth-Token”的取值为[1](#li17145102315153)中获取的Token。例如：curl aaaa.com/bbbb –H "X-Auth-Token:$token"。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >获取Token后，请清理相关使用痕迹，避免隐私信息泄露。  


