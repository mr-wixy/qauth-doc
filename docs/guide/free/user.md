### 通过code获取用户信息接口

#### 1、接口地址

> http://api.qauth.cn/user

#### 2、接口说明 

通过code、appkey、usersecret获取用户信息接口

#### 3、请求类型 `GET`

#### 4、请求参数

|参数|说明|必须|备注|
|--|--|--|--|
|code|用户信息获取标识|是|用户完成扫码登录后重定向到开发者的应用回调地址时携带的参数|
|appkey|应用标识|是|开发者在QuickAuth网站创建应用的AppKey|
|secret|加密秘钥|是|开发者在QuickAuth网站中的UserSecretKey|
|isTest|是否测试调用|否|true or false, QuickAuth网站中点测试按钮生成的code可调用，正式环境请勿传该参数|

5、返回结果

|key|value|说明|
|--|--|--|
|code|0或1|正确0，错误1|
|msg|string|提示信息|
|res|结果|用户的基本信息包含openid、nickname、avatarurl|
