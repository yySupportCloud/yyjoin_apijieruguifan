# 规范约束

第一：APIlink开发者入驻的API产品交易必须遵循《云市场平台服务协议》  
第二：API接口整体接入规范  
APIlink整体规范建议采用RESTful 方式来接入  
（1）协议：APIlink与ISV的通信协议同时支持http和https的协议，但用户调用APIlink的服务只支持https服务，为保证交互数据的安全，建议ISV尽可能采用https协议。  
（2）域名：APIlink接入的服务，APIlink会在api.yonyoucloud.com的域名后面做统一路由处理，所以我们支持ip和域名接入。  
（3）API请求方式：要求为常用的HTTP动词：  
GET（SELECT）：从服务器取出资源（一项或多项）。  
POST（CREATE）：在服务器新建一个资源。  
PUT（UPDATE）：在服务器更新资源（客户端提供改变后的完整资源）。  
DELETE（DELETE）：从服务器删除资源。  
（4）	API传入参数  
要求接入API的参类型为header,body,cookie，query。  
(5) 对接入API的安全认证  
要求接入API支持Oauth，口令，token认证中的一个。   
（6）调用示例代码  
根据API定义自动生成JAVA，PHP，.NET,CURL的demo，API开发者也可以定义调用代码的demo。  
（7）错误码定义  
APIlink网关提供公共网关层面的错误码，http状态码是500，具体参见API详情页面，开发者必须对每个API定义自己业务逻辑调用的错误码。  
（8）返回值  
要求返回值是xml或json格式。  
（9）API描述:API开发者需要尽可能详细的对API的主要功能和场景进行描述,方便使用者参考。
