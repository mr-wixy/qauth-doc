## #方式二

> 开发者通过接口获取二维码并展示，用户扫码授权完成后QuickAuth向开发者配置的回调地址发起授权请求并传入用户信息，开发者根据调用参数和回传参数识别用户登录情况

### 接口列表

1. [获取二维码(/qrcode)](/guide/method2/qrcode)
2. [获取扫码状态(/qrcode/state)](/guide/method2/state)
3. [用户信息解密(/decrypt)](/guide/method2/decrypt)


#### 创建应用

1. 登录[quickauth](https://qauth.cn)网站并创建[接入应用](https://qauth.cn/app)
2. 填写详细信息和回调地址并发布应用
3. 记住`AppKey`

#### 获取解密密钥

进入[用户中心](https://qauth.cn/config/secret)获取`UserSecretKey`

#### 修改现有项目

修改自己项目的登录逻辑，发起[获取二维码](/api/qrcode)请求

用户扫码后QuickAuth会向上面配置的回调地址并发起授权请求

请求类型：`POST`

请求的Content-Type：`application/x-www-form-urlencoded`

请求内容

|key|说明|
|--|--|
|appkey|用户创建应用的appkey|
|state|用户调用获取二维码接口时的扫码标识<br/>开发者可根据此信息识别登录用户
|encryptedData|用户加密信息（[信息的加密解密](/guide/encrypt)）|
|iv|用户信息加密初始向量|

开发者收到授权请求后需要解密和实现登录逻辑，完成后需返回字符串`success`
