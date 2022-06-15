### QuickAuth 用户信息解密接口

#### 1、接口地址

> http://api.qauth.cn/decrypt

#### 2、接口说明 

加密数据解密接口

#### 3、请求类型  `POST`

Content-Type: `application/json`

#### 4、请求参数

|参数|说明|必须|备注|
|--|--|--|--|
|encryptedData|加密数据|是|用户授权登录后<br/>qauth调用开发者应用回调地址是发送的数据|
|key|加密密钥|是|开发者在qauth网站设置的加密密钥|
|iv|加密初始向量|是|用户授权登录后 qauth调用开发者应用回调地址是发送的数据|

5、返回结果

|key|value|说明|
|--|--|--|
|code|0或1|正确0，错误1|
|msg|string|提示信息|
|res|结果|解密的用户信息|
