# QuickAuth介绍

> QuickAuth是一个便捷的第三方登录集成平台，支持微信（开放平台、服务号、小程序）、QQ、短信验证码、Github、Gitee、支付宝、微博、钉钉等多平台授权登录方式，支持通过Typecho、WordPress插件实现免代码接入

## 接入指南

- [接入指南](guide/)
- [推广奖励说明](invite)
- [订阅功能说明](subscribe)

## 接口列表

### 接口

1. [授权登录界面(/oauth)](/guide/oauth)
2. [获取用户授权信息（/user接口的升级版）(/authinfo)](/guide/authinfo)

### 归档接口（可用但停止更新）

1. [小程序扫码登录界面(/qrconnect)](/guide/archived/qrconnect)
2. [获取用户信息(/user)](/guide/archived/user)
3. [获取二维码(/qrcode)](/guide/archived/qrcode)
4. [获取扫码状态(/qrcode/state)](/guide/archived/state)
5. [用户信息解密(/decrypt)](/guide/archived/decrypt)

## 接入应用

- [QuickAuth](https://qauth.cn) （QuickAuth项目网站）
- [UltronBlog](https://blog.wixy.cn) （wixy的个人博客）
- [SiliSchedule](https://sc.wixy.cn) （HTTP定时任务管理系统）
- [更多接入应用](https://qauth.cn/home)

## 相关插件

- [QualPro](https://github.com/mr-wixy/QualPro) （WordPress集成登录插件）
- [QuickAuthLogin](https://github.com/mr-wixy/QuickAuthLogin) （Typecho博客微信扫码登录插件）
- [QuickAuthLogin-WP](https://github.com/mr-wixy/QuickAuthLogin-WP) （WordPress微信扫码登录插件）

### 其他

- [信息的加解密](other/encrypt)
- [更新历史](other/update)
- [开发计划](other/plan)
