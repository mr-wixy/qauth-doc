# 通过code获取用户授权信息接口

## 1、接口地址

> <http://api.qauth.cn/authinfo>

## 2、接口说明

通过code、appkey、usersecret获取用户信息接口

2.1.0.0版本新增的接口，修改了数据输出格式，用于替换旧版/user接口

## 3、请求类型

`GET`

## 4、请求参数

|参数|说明|必须|备注|
|--|--|--|--|
|code|用户信息获取标识|是|用户完成扫码登录后重定向到开发者的应用回调地址时携带的参数|
|appkey|应用标识|是|开发者在QuickAuth网站创建应用的AppKey|
|secret|加密秘钥|是|开发者在QuickAuth网站中的UserSecretKey|
|isTest|是否测试调用|否|true or false, QuickAuth网站中点测试按钮生成的code可调用，正式环境请勿传该参数|

## 5、返回结果

|key|value|说明|
|--|--|--|
|code|0或1|正确0，错误1|
|msg|string|提示信息|
|res|结果|用户授权信息|

### 返回结果示例

```json
{
    "code": 0,
    "msg": "success",
    "res": {
        "state": "login",//调用/oauth接口时传入的参数
        "redirectUrl": "https://qauth.cn/app",//调用/oauth接口时传入的参数
        "authType": "wechat",//调用/oauth接口时传入的参数
        "detailType": "offiaccount",//调用/oauth接口时传入的参数
        "userInfo": {
            "openId": "03af4fa4-f755-471d-a9be-1080c133ed03",
            "unionId": "665049e8-c8c0-4ef9-adb6-5e254ce5ce98",//仅微信登录方式会有内容
            "nickName": "wixy",
            "avatarUrl": "https://gravatar.loli.net/avatar",
            "mobile": "13888888888",//仅验证码登录方式返回
            "email": "wixy@qq.com"
        }
    }
}

```
