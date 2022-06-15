## QuickAuth介绍

> QuickAuth（简称 QAuth) 是一个快捷扫码登陆项目
该项目致力于帮助个人开发者为自己的项目接入扫码登陆功能


### 接入指南

- [接入指南](guide/)	
- [订阅功能说明](subscribe)
- [信息的加解密](other/encrypt)

### 接口列表

#### 普通接口（免费用户永久可用）

1. [小程序扫码登录界面(/qrconnect)](/guide/method1/qrconnect)
2. [获取用户信息(/user)](/guide/method1/user)

#### 高级接口（订阅会员可用）

1. [授权登录界面(/oauth)](/guide/advanced/oauth)
2. [获取用户信息(/user)](/guide/advanced/user)

#### 即将停止维护的接口

1. [获取二维码(/qrcode)](/guide/archived/qrcode)
2. [获取扫码状态(/qrcode/state)](/guide/archived/state)
3. [用户信息解密(/decrypt)](/guide/archived/decrypt)


### 接入应用

- [QuickAuth](https://qauth.cn) （QuickAuth项目网站）
- [SiliSchedule](https://sc.wixy.cn) （HTTP定时任务管理系统）
- [UltronBlog](https://blog.wixy.cn) （wixy的个人博客）


### 相关插件

- [QuickAuthLogin](https://gitee.com/wixy/QuickAuthLogin) （Typecho博客微信扫码登录插件）
- [QuickAuthLogin-WP](https://gitee.com/wixy/QuickAuthLogin-WP) （WordPress微信扫码登录插件）

### 其他

- [更新历史](other/update)
- [开发计划](other/plan)
