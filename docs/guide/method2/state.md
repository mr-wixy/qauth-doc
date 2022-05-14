### QuickAuth 获取扫码状态接口

#### 1、接口地址

> http://api.qauth.cn/qrcode/state

#### 2、接口说明 

通过`qid`获取询二维码的扫码状态
`qid`是在用户请求二维码时正常情况下返回的响应头

#### 3、请求类型 `GET`

#### 4、请求参数

|参数|必须|备注|
|--|--|--|
|qid|是|在获取二维码时返回的响应头|

5、返回结果

|key|value|说明|
|--|--|--|
|code|0或1|正确0，错误1|
|msg|string|提示信息|
|res|结果|`create`: 已创建未扫码<br/>`scan`：用户已扫码<br/>`auth`：用户已授权|

6、示例

> http://api.qauth.cn/qrcode/state?qid=4a6a6e14fe51484f8ce257c242a3d88e
