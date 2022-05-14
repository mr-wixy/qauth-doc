### QuickAuth扫码登录界面

#### 1、接口地址

> http://api.qauth.cn/qrconnect

#### 2、接口说明 

开发者应用点击扫码登录时跳转的扫码登录界面，用户扫码并完成登录授权后界面重定向到应用配置的回调地址上并携带code和state参数

#### 3、请求参数

|参数|必须|备注|
|--|--|--|
|appkey|是|开发者在QuickAuth网站创建应用的AppKey|
|state|是|开发者应用附加信息|
|popup|否|true或者false，默认false<br />开发者使用window.open()打开界面时可以设置为true<br />用户授权完成后自动关闭弹窗并使主页面重定向|

#### 4、重定向时携带的参数

|参数|说明|
|--|--|
|code|用于获取授权用户信息的code，该code只能使用一次|
|state|调用时设置的state|

> 示例： https://api.qauth.cn/qrconnect?appkey=123&state=login