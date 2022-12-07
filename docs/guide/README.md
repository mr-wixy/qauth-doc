# 接入指南

## 普通接入方式

> 通过跳转界面实现用户授权登录

### 特点

- 支持小程序扫码、QQ、Gitee、Github、支付宝、微博、钉钉等永久免费的接入方式
- 支持订阅会员专属的 微信扫码登录、SMS短信登录的方式
- 支持Typecho和WordPress插件接入，无代码接入

### 接口列表

[详细接口文档](/guide/guide)

[QualPro插件接入](https://github.com/mr-wixy/QualPro)

[Typecho接入教程（QuickAuthLogin）](https://github.com/mr-wixy/QuickAuthLogin)

[WordPress接入教程（QuickAuthLogin-WP）](https://github.com/mr-wixy/QuickAuthLogin-WP)

## 复杂接入方式（已归档，停止更新）

> 开发者通过接口获取二维码并展示，用户扫码授权完成后QuickAuth向开发者配置的回调地址发起授权请求并传入用户信息，开发者根据调用参数和回传参数识别用户登录情况

#### 特点

- 可自行获取二维码，自定义登录界面及流程
- 自定义程度高
- 仅支持小程序扫码登录的接入方式

[详细接口文档](/guide/archived/)
