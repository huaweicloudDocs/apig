# 编辑VPC通道<a name="apig-zh-ug-180425082"></a>

## 操作场景<a name="section1049118613499"></a>

创建VPC通道后，通过编辑VPC通道修改创建时设置的参数。

## 前提条件<a name="section2234711104910"></a>

已创建VPC通道。

## 操作步骤<a name="section1854781612494"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域。
3.  在服务列表中，单击“应用服务 \> API网关”，进入API网关服务管理页面。
4.  单击“开放API \> VPC通道”，进入到VPC通道列表页面。
5.  通过以下任意一种方法，进入“编辑VPC通道”页面。
    -   在待编辑的VPC通道所在行，单击“编辑”。
    -   单击“_VPC通道__名称_”，进入VPC通道详情页面。在右上角单击“编辑”。

6.  在“VPC通道配置”页面，编辑如[表1](#table19544124604213)所示信息。

    **表 1**  VPC通道配置

    <a name="table19544124604213"></a>
    <table><thead align="left"><tr id="apig-zh-ug-180425081_row11118189178"><th class="cellrowborder" valign="top" width="18%" id="mcps1.2.4.1.1"><p id="apig-zh-ug-180425081_p11112181178"><a name="apig-zh-ug-180425081_p11112181178"></a><a name="apig-zh-ug-180425081_p11112181178"></a>信息项</p>
    </th>
    <th class="cellrowborder" valign="top" width="40%" id="mcps1.2.4.1.2"><p id="apig-zh-ug-180425081_p4111018131716"><a name="apig-zh-ug-180425081_p4111018131716"></a><a name="apig-zh-ug-180425081_p4111018131716"></a>描述</p>
    </th>
    <th class="cellrowborder" valign="top" width="42%" id="mcps1.2.4.1.3"><p id="apig-zh-ug-180425081_p7111111841712"><a name="apig-zh-ug-180425081_p7111111841712"></a><a name="apig-zh-ug-180425081_p7111111841712"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="apig-zh-ug-180425081_row6111191851715"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="apig-zh-ug-180425081_p16111181817177"><a name="apig-zh-ug-180425081_p16111181817177"></a><a name="apig-zh-ug-180425081_p16111181817177"></a>通道名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.2 "><p id="apig-zh-ug-180425081_p3111101851711"><a name="apig-zh-ug-180425081_p3111101851711"></a><a name="apig-zh-ug-180425081_p3111101851711"></a>自定义VPC通道名称，用于识别不同的VPC通道。</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.4.1.3 "><a name="apig-zh-ug-180425081_ul9322050165213"></a><a name="apig-zh-ug-180425081_ul9322050165213"></a><ul id="apig-zh-ug-180425081_ul9322050165213"><li>支持汉字、英文、数字、下划线和中划线。</li><li>只能以汉字或者英文开头。</li><li>3 ~ 64个字符。</li></ul>
    </td>
    </tr>
    <tr id="apig-zh-ug-180425081_row18111101816173"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="apig-zh-ug-180425081_p611161871720"><a name="apig-zh-ug-180425081_p611161871720"></a><a name="apig-zh-ug-180425081_p611161871720"></a>端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.2 "><p id="apig-zh-ug-180425081_p11119181176"><a name="apig-zh-ug-180425081_p11119181176"></a><a name="apig-zh-ug-180425081_p11119181176"></a>VPC通道中主机的端口号。</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.4.1.3 "><p id="apig-zh-ug-180425081_p85434411179"><a name="apig-zh-ug-180425081_p85434411179"></a><a name="apig-zh-ug-180425081_p85434411179"></a>1 ~ 65535</p>
    </td>
    </tr>
    <tr id="apig-zh-ug-180425081_row311112189175"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="apig-zh-ug-180425081_p711181861718"><a name="apig-zh-ug-180425081_p711181861718"></a><a name="apig-zh-ug-180425081_p711181861718"></a>分发算法</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.2 "><p id="apig-zh-ug-180425081_p61112186175"><a name="apig-zh-ug-180425081_p61112186175"></a><a name="apig-zh-ug-180425081_p61112186175"></a>通过分发算法确定请求被发送到哪台主机。</p>
    <p id="apig-zh-ug-180425081_p243201117507"><a name="apig-zh-ug-180425081_p243201117507"></a><a name="apig-zh-ug-180425081_p243201117507"></a>分发算法包含如下几种：</p>
    <a name="apig-zh-ug-180425081_ul24918264502"></a><a name="apig-zh-ug-180425081_ul24918264502"></a><ul id="apig-zh-ug-180425081_ul24918264502"><li>加权轮询</li><li>加权最少连接</li><li>源地址哈希</li><li>URI哈希</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.4.1.3 "><p id="apig-zh-ug-180425081_p311118181174"><a name="apig-zh-ug-180425081_p311118181174"></a><a name="apig-zh-ug-180425081_p311118181174"></a>仅在“通道类型”为“快速通道”时，需要配置。</p>
    </td>
    </tr>
    <tr id="apig-zh-ug-180425081_row131116181170"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="apig-zh-ug-180425081_p9111018101714"><a name="apig-zh-ug-180425081_p9111018101714"></a><a name="apig-zh-ug-180425081_p9111018101714"></a>协议</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.2 "><p id="apig-zh-ug-180425081_p2011131851712"><a name="apig-zh-ug-180425081_p2011131851712"></a><a name="apig-zh-ug-180425081_p2011131851712"></a>使用以下协议，对VPC中主机执行健康检查。</p>
    <a name="apig-zh-ug-180425081_ul19904951155719"></a><a name="apig-zh-ug-180425081_ul19904951155719"></a><ul id="apig-zh-ug-180425081_ul19904951155719"><li>TCP</li><li>HTTP</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.4.1.3 "><p id="apig-zh-ug-180425081_p15111121815177"><a name="apig-zh-ug-180425081_p15111121815177"></a><a name="apig-zh-ug-180425081_p15111121815177"></a>默认为TCP协议。</p>
    </td>
    </tr>
    <tr id="apig-zh-ug-180425081_row18456130124815"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="apig-zh-ug-180425081_p184571630114817"><a name="apig-zh-ug-180425081_p184571630114817"></a><a name="apig-zh-ug-180425081_p184571630114817"></a>路径</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.2 "><p id="apig-zh-ug-180425081_p613810287424"><a name="apig-zh-ug-180425081_p613810287424"></a><a name="apig-zh-ug-180425081_p613810287424"></a>健康检查时的目标路径。</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.4.1.3 "><p id="apig-zh-ug-180425081_p11381528154218"><a name="apig-zh-ug-180425081_p11381528154218"></a><a name="apig-zh-ug-180425081_p11381528154218"></a>仅在协议为“HTTP”时，需要设置。</p>
    </td>
    </tr>
    <tr id="apig-zh-ug-180425081_row311151817174"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="apig-zh-ug-180425081_p12111518111715"><a name="apig-zh-ug-180425081_p12111518111715"></a><a name="apig-zh-ug-180425081_p12111518111715"></a>检查端口</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.2 "><p id="apig-zh-ug-180425081_p141118181171"><a name="apig-zh-ug-180425081_p141118181171"></a><a name="apig-zh-ug-180425081_p141118181171"></a>健康检查的目标端口。</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.4.1.3 "><p id="apig-zh-ug-180425081_p31121118191714"><a name="apig-zh-ug-180425081_p31121118191714"></a><a name="apig-zh-ug-180425081_p31121118191714"></a>缺省时为VPC中主机的端口号。</p>
    </td>
    </tr>
    <tr id="apig-zh-ug-180425081_row1611281881717"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="apig-zh-ug-180425081_p511241811178"><a name="apig-zh-ug-180425081_p511241811178"></a><a name="apig-zh-ug-180425081_p511241811178"></a>正常阈值</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.2 "><p id="apig-zh-ug-180425081_p311281816174"><a name="apig-zh-ug-180425081_p311281816174"></a><a name="apig-zh-ug-180425081_p311281816174"></a>判定VPC通道中主机正常的依据为：连续检查<em id="apig-zh-ug-180425081_i421224922811"><a name="apig-zh-ug-180425081_i421224922811"></a><a name="apig-zh-ug-180425081_i421224922811"></a>x</em>成功，x为您设置的正常阈值。</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.4.1.3 "><p id="apig-zh-ug-180425081_p1211261861710"><a name="apig-zh-ug-180425081_p1211261861710"></a><a name="apig-zh-ug-180425081_p1211261861710"></a>取值为2 ~ 10。缺省时为2。</p>
    </td>
    </tr>
    <tr id="apig-zh-ug-180425081_row1852365410195"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="apig-zh-ug-180425081_p1952385471913"><a name="apig-zh-ug-180425081_p1952385471913"></a><a name="apig-zh-ug-180425081_p1952385471913"></a>异常阈值</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.2 "><p id="apig-zh-ug-180425081_p75241154111912"><a name="apig-zh-ug-180425081_p75241154111912"></a><a name="apig-zh-ug-180425081_p75241154111912"></a>判定VPC通道中主机异常的依据为：连续检查<em id="apig-zh-ug-180425081_i37296135294"><a name="apig-zh-ug-180425081_i37296135294"></a><a name="apig-zh-ug-180425081_i37296135294"></a>x失败</em>，x为您设置的异常阈值。</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.4.1.3 "><p id="apig-zh-ug-180425081_p35246549198"><a name="apig-zh-ug-180425081_p35246549198"></a><a name="apig-zh-ug-180425081_p35246549198"></a>取值为2 ~ 10。缺省时为5。</p>
    </td>
    </tr>
    <tr id="apig-zh-ug-180425081_row9935144112016"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="apig-zh-ug-180425081_p1393513414209"><a name="apig-zh-ug-180425081_p1393513414209"></a><a name="apig-zh-ug-180425081_p1393513414209"></a>超时时间</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.2 "><p id="apig-zh-ug-180425081_p109350415202"><a name="apig-zh-ug-180425081_p109350415202"></a><a name="apig-zh-ug-180425081_p109350415202"></a>检查期间，无响应的时间，单位为秒。</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.4.1.3 "><p id="apig-zh-ug-180425081_p29359472013"><a name="apig-zh-ug-180425081_p29359472013"></a><a name="apig-zh-ug-180425081_p29359472013"></a>取值为2 ~ 30。缺省时为5。</p>
    </td>
    </tr>
    <tr id="apig-zh-ug-180425081_row12537112014201"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="apig-zh-ug-180425081_p653772016204"><a name="apig-zh-ug-180425081_p653772016204"></a><a name="apig-zh-ug-180425081_p653772016204"></a>间隔时间</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.2 "><p id="apig-zh-ug-180425081_p145371520162013"><a name="apig-zh-ug-180425081_p145371520162013"></a><a name="apig-zh-ug-180425081_p145371520162013"></a>连续两次检查的间隔时间，单位为秒。</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.4.1.3 "><p id="apig-zh-ug-180425081_p15537152082011"><a name="apig-zh-ug-180425081_p15537152082011"></a><a name="apig-zh-ug-180425081_p15537152082011"></a>取值为5 ~ 300。缺省时为10。</p>
    </td>
    </tr>
    <tr id="apig-zh-ug-180425081_row154521040174814"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="apig-zh-ug-180425081_p29821396421"><a name="apig-zh-ug-180425081_p29821396421"></a><a name="apig-zh-ug-180425081_p29821396421"></a>HTTP响应码</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.2 "><p id="apig-zh-ug-180425081_p33611150135410"><a name="apig-zh-ug-180425081_p33611150135410"></a><a name="apig-zh-ug-180425081_p33611150135410"></a>检查目标HTTP响应时，判断成功使用的HTTP响应码。</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.4.1.3 "><p id="apig-zh-ug-180425081_p3982103914426"><a name="apig-zh-ug-180425081_p3982103914426"></a><a name="apig-zh-ug-180425081_p3982103914426"></a>仅在协议为“HTTP”时，需要设置。</p>
    </td>
    </tr>
    </tbody>
    </table>

7.  单击“下一步”，进入“添加弹性云服务器”页面。
8.  添加弹性云服务器、删除弹性云服务器、修改弹性云服务器权重，单击“完成”，完成VPC通道的修改。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >待添加的弹性云服务器的安全组必须允许100.125.0.0/16网段访问，否则将导致健康检查失败及业务不通。  


