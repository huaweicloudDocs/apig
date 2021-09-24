# 创建环境<a name="ZH-CN_TOPIC_0000001082135105"></a>

## 功能介绍<a name="zh-cn_topic_0118922244_section55469153"></a>

在实际的生产中，API提供者可能有多个环境，如开发环境、测试环境、生产环境等，用户可以自由将API发布到某个环境，供调用者调用。对于不同的环境，API的版本、请求地址甚至于包括请求消息等均有可能不同。如：某个API，v1.0的版本为稳定版本，发布到了生产环境供生产使用，同时，该API正处于迭代中，v1.1的版本是开发人员交付测试人员进行测试的版本，发布在测试环境上，而v1.2的版本目前开发团队正处于开发过程中，可以发布到开发环境进行自测等。

为此，API网关提供多环境管理功能，使租户能够最大化的模拟实际场景，低成本的接入API网关。

## URI<a name="zh-cn_topic_0118922244_section29460329"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118922244_table9532032"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922244_row526639"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922244_p42657813"><a name="zh-cn_topic_0118922244_p42657813"></a><a name="zh-cn_topic_0118922244_p42657813"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922244_p32730835"><a name="zh-cn_topic_0118922244_p32730835"></a><a name="zh-cn_topic_0118922244_p32730835"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922244_row33952018"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922244_p65758970"><a name="zh-cn_topic_0118922244_p65758970"></a><a name="zh-cn_topic_0118922244_p65758970"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922244_p24876338"><a name="zh-cn_topic_0118922244_p24876338"></a><a name="zh-cn_topic_0118922244_p24876338"></a>/v1.0/apigw/envs</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118922244_section63816370"></a>

**表 2**  参数说明

<a name="zh-cn_topic_0118922244_table1717474"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922244_row29542137"><th class="cellrowborder" valign="top" width="15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118922244_p44102876"><a name="zh-cn_topic_0118922244_p44102876"></a><a name="zh-cn_topic_0118922244_p44102876"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118922244_p15563175"><a name="zh-cn_topic_0118922244_p15563175"></a><a name="zh-cn_topic_0118922244_p15563175"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118922244_p52657667"><a name="zh-cn_topic_0118922244_p52657667"></a><a name="zh-cn_topic_0118922244_p52657667"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.99999999999999%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118922244_p37412631"><a name="zh-cn_topic_0118922244_p37412631"></a><a name="zh-cn_topic_0118922244_p37412631"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922244_row10524300"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922244_p47161994"><a name="zh-cn_topic_0118922244_p47161994"></a><a name="zh-cn_topic_0118922244_p47161994"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922244_p62025144"><a name="zh-cn_topic_0118922244_p62025144"></a><a name="zh-cn_topic_0118922244_p62025144"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922244_p57980734"><a name="zh-cn_topic_0118922244_p57980734"></a><a name="zh-cn_topic_0118922244_p57980734"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.99999999999999%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922244_p65927877"><a name="zh-cn_topic_0118922244_p65927877"></a><a name="zh-cn_topic_0118922244_p65927877"></a>环境的名称</p>
<p id="zh-cn_topic_0118922244_p11475995"><a name="zh-cn_topic_0118922244_p11475995"></a><a name="zh-cn_topic_0118922244_p11475995"></a>支持英文，数字，下划线，且只能以英文字母开头，3 ~ 64字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922244_row49845607"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922244_p10962361"><a name="zh-cn_topic_0118922244_p10962361"></a><a name="zh-cn_topic_0118922244_p10962361"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922244_p15536035"><a name="zh-cn_topic_0118922244_p15536035"></a><a name="zh-cn_topic_0118922244_p15536035"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922244_p50459342"><a name="zh-cn_topic_0118922244_p50459342"></a><a name="zh-cn_topic_0118922244_p50459342"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.99999999999999%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922244_p60674914"><a name="zh-cn_topic_0118922244_p60674914"></a><a name="zh-cn_topic_0118922244_p60674914"></a>描述信息</p>
<p id="zh-cn_topic_0118922244_p7270965"><a name="zh-cn_topic_0118922244_p7270965"></a><a name="zh-cn_topic_0118922244_p7270965"></a>字符长度不能大于255</p>
<div class="note" id="zh-cn_topic_0118922244_note20200152985412"><a name="zh-cn_topic_0118922244_note20200152985412"></a><a name="zh-cn_topic_0118922244_note20200152985412"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118922244_p15200162915544"><a name="zh-cn_topic_0118922244_p15200162915544"></a><a name="zh-cn_topic_0118922244_p15200162915544"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
	"name": "DEV",
	"remark": "开发环境"
}
```

## 响应消息<a name="zh-cn_topic_0118922244_section1743476"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118922244_table5508329"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922244_row35969539"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118922244_p27851519"><a name="zh-cn_topic_0118922244_p27851519"></a><a name="zh-cn_topic_0118922244_p27851519"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118922244_p41380592"><a name="zh-cn_topic_0118922244_p41380592"></a><a name="zh-cn_topic_0118922244_p41380592"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118922244_p63493694"><a name="zh-cn_topic_0118922244_p63493694"></a><a name="zh-cn_topic_0118922244_p63493694"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922244_row42715600"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922244_p37411599"><a name="zh-cn_topic_0118922244_p37411599"></a><a name="zh-cn_topic_0118922244_p37411599"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922244_p10440674"><a name="zh-cn_topic_0118922244_p10440674"></a><a name="zh-cn_topic_0118922244_p10440674"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922244_p40388274"><a name="zh-cn_topic_0118922244_p40388274"></a><a name="zh-cn_topic_0118922244_p40388274"></a>环境ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922244_row27950148"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922244_p49369497"><a name="zh-cn_topic_0118922244_p49369497"></a><a name="zh-cn_topic_0118922244_p49369497"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922244_p39506335"><a name="zh-cn_topic_0118922244_p39506335"></a><a name="zh-cn_topic_0118922244_p39506335"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922244_p45896573"><a name="zh-cn_topic_0118922244_p45896573"></a><a name="zh-cn_topic_0118922244_p45896573"></a>环境名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922244_row10415981"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922244_p38388164"><a name="zh-cn_topic_0118922244_p38388164"></a><a name="zh-cn_topic_0118922244_p38388164"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922244_p22433542"><a name="zh-cn_topic_0118922244_p22433542"></a><a name="zh-cn_topic_0118922244_p22433542"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922244_p5177629"><a name="zh-cn_topic_0118922244_p5177629"></a><a name="zh-cn_topic_0118922244_p5177629"></a>创建时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922244_row46598668"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922244_p16395773"><a name="zh-cn_topic_0118922244_p16395773"></a><a name="zh-cn_topic_0118922244_p16395773"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922244_p52989238"><a name="zh-cn_topic_0118922244_p52989238"></a><a name="zh-cn_topic_0118922244_p52989238"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922244_p64269920"><a name="zh-cn_topic_0118922244_p64269920"></a><a name="zh-cn_topic_0118922244_p64269920"></a>描述信息</p>
</td>
</tr>
</tbody>
</table>

响应参数样例：

```
{
	"id": "cca3616a-f368-4b32-9064-b2a631cb3eeb",
	"name": "DEV",
	"remark": "开发环境",
	"create_time": "2017-12-28T12:50:47.0744311Z"
}
```

## 状态码<a name="zh-cn_topic_0118922244_section37476421"></a>

**表 4**  返回消息说明

<a name="zh-cn_topic_0118922244_table62896751"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922244_row51515956"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922244_p12042908"><a name="zh-cn_topic_0118922244_p12042908"></a><a name="zh-cn_topic_0118922244_p12042908"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922244_p35951505"><a name="zh-cn_topic_0118922244_p35951505"></a><a name="zh-cn_topic_0118922244_p35951505"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922244_row26390778"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922244_p57278272"><a name="zh-cn_topic_0118922244_p57278272"></a><a name="zh-cn_topic_0118922244_p57278272"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922244_p9028426"><a name="zh-cn_topic_0118922244_p9028426"></a><a name="zh-cn_topic_0118922244_p9028426"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922244_row14146972"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922244_p5054088"><a name="zh-cn_topic_0118922244_p5054088"></a><a name="zh-cn_topic_0118922244_p5054088"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922244_p14836248203011"><a name="zh-cn_topic_0118922244_p14836248203011"></a><a name="zh-cn_topic_0118922244_p14836248203011"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922244_row60551827"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922244_p5750975"><a name="zh-cn_topic_0118922244_p5750975"></a><a name="zh-cn_topic_0118922244_p5750975"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922244_p63175864"><a name="zh-cn_topic_0118922244_p63175864"></a><a name="zh-cn_topic_0118922244_p63175864"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922244_row192278368305"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922244_p202279369300"><a name="zh-cn_topic_0118922244_p202279369300"></a><a name="zh-cn_topic_0118922244_p202279369300"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922244_p1222717361307"><a name="zh-cn_topic_0118922244_p1222717361307"></a><a name="zh-cn_topic_0118922244_p1222717361307"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922244_row31711869"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922244_p18524563"><a name="zh-cn_topic_0118922244_p18524563"></a><a name="zh-cn_topic_0118922244_p18524563"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922244_p14947689"><a name="zh-cn_topic_0118922244_p14947689"></a><a name="zh-cn_topic_0118922244_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

