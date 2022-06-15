## #高级接口（订阅会员可用）

> 高级接口主要包括微信扫码登录、微信客户端内静默授权登录、QQ等其他登录方式、高级统计接口等，仅订阅会员可用

### 接口列表

1. [登录授权界面(/oauth)](/guide/advanced/oauth)
2. [获取用户信息(/user)](/guide/advanced/user)

#### 创建应用

1、登录[quickauth](https://qauth.cn)网站并创建[接入应用](https://qauth.cn/app)

2、填写详细信息和回调地址并发布应用

3、记住`AppKey`

#### 获取解密密钥

进入[用户中心](https://qauth.cn/config/secret)获取`UserSecretKey`

#### 修改现有项目

1、修改自己项目的登录逻辑，携带参数type、appkey和state跳转到[登录授权界面](/guide/advanced/oauth)

2、用户扫码并授权后界面跳转到应用配置的回调地址并带上参数`code`和`state`

3、开发者使用code、Appkey、UserSecretKey发起[获取用户信息](/guide/advanced/user)请求并根据返回信息完成登录逻辑