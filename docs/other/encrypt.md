### QuickAuth 用户信息的加解密

#### 加密方法

QuickAuth对用户信息使用的是AES对称加密

1. 对称解密使用的算法为 AES-128-CBC
2. 数据采用PKCS#7填充
3. 对称解密的目标密文为 Base64_Decode(encryptedData)
4. 对称解密秘钥是用户中心获取的`AesEncryptKey`
5. 对称解密算法初始向量iv为发起授权请求时的参数

<br/>

#### 解密

开发者需要对接口返回的加密数据`encryptedData`进行解密

开发者有两种方式解密：

1. 自行实现AES解密方法
2. 调用qauth的解密接口[decrypt](/api/decrypt)