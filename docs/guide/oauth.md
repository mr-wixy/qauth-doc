# QuickAuth登录授权界面

## 1、接口地址

> <http://api.qauth.cn/oauth>

## 2、接口说明

开发者应用点击第三方登录按钮跳转的界面

## 3、请求参数

|参数|必须|备注|
|--|--|--|
|type|是|授权方式，支持（wechat、qq、github、gitee、alipay、weibo、dingtalk、sms）|
|detailType|否|type传入wechat时，可传入detailType参数来控制微信接入的调用方式，支持（offiaccount、miniprogram和oplatform），不传或者传入其他值则默认为offiaccount|
|appkey|是|开发者在QuickAuth网站创建应用的AppKey|
|state|否|开发者应用附加信息|
|redirect|否|授权成功后需要重新跳转的地址|

### 备注

type参数传wechat，detailType传入offiaccount或默认传参时，如果是在微信客户端内打开网站，则不需要扫码，直接完成静默授权逻辑，实现无感登录

## 4、重定向时携带的参数

用户完成授权后会重定向到用户配置的回调地址上，并携带code和state参数

|参数|说明|
|--|--|
|code|用于获取授权用户信息的code，该code只能使用一次|
|state|调用时设置的state|

> 示例： <https://api.qauth.cn/oauth?type=wechat&appkey=e0176d4b&state=login>