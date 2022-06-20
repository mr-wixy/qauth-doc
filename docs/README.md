## QuickAuth介绍

> QuickAuth是一个便捷的第三方登录集成平台，支持微信（开放平台、服务号、小程序）、QQ、Github、Gitee等多平台授权登录方式，支持通过Typecho、WordPress插件实现免代码接入

### 接入指南

- [接入指南](guide/)	
- [订阅功能说明](subscribe)

### 接口列表

#### 普通接口（免费用户可用）

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
- [UltronBlog](https://blog.wixy.cn) （wixy的个人博客）
- [SiliSchedule](https://sc.wixy.cn) （HTTP定时任务管理系统）
- [更多接入应用](https://qauth.cn/home)


### 相关插件

- [QuickAuthLogin](https://gitee.com/wixy/QuickAuthLogin) （Typecho博客微信扫码登录插件）
- [QuickAuthLogin-WP](https://gitee.com/wixy/QuickAuthLogin-WP) （WordPress微信扫码登录插件）

### 其他

- [信息的加解密](other/encrypt)
- [更新历史](other/update)
- [开发计划](other/plan)
