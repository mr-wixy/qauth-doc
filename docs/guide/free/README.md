## #基础接口（永久免费使用）

> 该接入方式为微信小程序扫码授权的方式

> 前端点击微信扫码登录按钮跳转到QuickAuth扫码登录界面（或者弹出扫码登录窗口），用户扫码完成后重定向到开发者配置的回调地址并携带相应的参数

### 接口列表

1. [扫码界面(/qrconnect)](/guide/free/qrconnect)
2. [获取用户信息(/user)](/guide/free/user)

#### 创建应用

1、登录[quickauth](https://qauth.cn)网站并创建[接入应用](https://qauth.cn/app)

2、填写详细信息和回调地址并发布应用

3、记住`AppKey`

#### 获取解密密钥

进入[用户中心](https://qauth.cn/config/secret)获取`UserSecretKey`

#### 修改现有项目

1、修改自己项目的登录逻辑，携带参数appkey和state跳转到[扫码界面](/guide/free/qrconnect)

2、用户扫码并授权后界面跳转到应用配置的回调地址并带上参数`code`和`state`

3、开发者使用code、Appkey、UserSecretKey发起[获取用户信息](/guide/free/user)请求并根据返回信息完成登录逻辑