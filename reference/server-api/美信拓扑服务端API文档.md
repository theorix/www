# 美信拓扑服务端API文档
[toc]
## 1	环境变量

### 默认环境1
| 参数名 | 字段值 |
| ------ | ------ |
|baseUrl|http://s-1-3-api.maximtop.cn|


## 2	美信拓扑服务端API文档

##### 说明
> 



##### 联系方式
- **联系人：**技术支持请访问
- **邮箱：**
- **网址：**/https://github.com/maxim-top/maxims-bistro/issues/

##### 文档版本
```
v1.0
```


## 3	用户操作

## 3.1	设置加好友验证方式

> POST  /user/authmode
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|value||value|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.2	设置加好友验证方式

> PUT  /user/authmode
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|value||value|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.3	设置头像

> POST  /user/avatar
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| avatar|string||false|头像 url|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.4	设置头像

> PUT  /user/avatar
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| avatar|string||false|头像 url|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.5	批量设置头像

> POST  /user/avatar/batch
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| list|array[object]||false||
|⇥ avatar|string||false|头像 url|
|⇥ user_id|int32||false|用户ID|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ reason|string||false|失败原因|
|⇥ success|boolean||false|是否成功|
|⇥ user_id|int32||false|用户ID|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.6	批量设置头像

> PUT  /user/avatar/batch
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| list|array[object]||false||
|⇥ avatar|string||false|头像 url|
|⇥ user_id|int32||false|用户ID|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ reason|string||false|失败原因|
|⇥ success|boolean||false|是否成功|
|⇥ user_id|int32||false|用户ID|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.7	将openid绑定到账号.(绑定建议使用/app/wechat/bind;解绑建议使用/app/wechat/unbind)

> GET  /user/bind_openid
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|open_id||open_id|
|type||type|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.8	修改密码

> POST  /user/change_password
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| new_password|string||false|new_password 新密码|
| old_password|string||false|old_password 旧密码|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.9	设备列表

> GET  /user/device/list
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| cursor|string||false|游标，返回结果中缺失 cursor，表示已经返回最后一页|
| data|array[object]||false|结果数据|
|⇥ device_sn|int32||false||
|⇥ platform|int32||false|设备平台, 1:ios, 2:android, 3:windows, 4:mac, 5:linux, 6:web|
|⇥ user_agent|string||false||
|⇥ user_id|int32||false|用户 ID|
| message|string||false|错误信息，如果成功，该项为null|
| version|int32||false|版本|

##### 接口描述
> 




## 3.10	删除device

> POST  /user/device/remove
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|device_sn||device_sn|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.11	删除device

> DELETE  /user/device/remove
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|device_sn||device_sn|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.12	封禁用户

> PUT  /user/disable
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| list|array[int32]||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.13	设置是否自动下载缩略图和文件

> POST  /user/download
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|value||value|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.14	设置是否自动下载缩略图和文件

> PUT  /user/download
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|value||value|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.15	解禁用户

> PUT  /user/enable
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| list|array[int32]||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.16	踢指定设备下线

> POST  /user/kick
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|device_sn||不传device_sn表示踢所有设备|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.17	踢指定设备下线

> PUT  /user/kick
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|device_sn||不传device_sn表示踢所有设备|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.18	设置手机号码

> POST  /user/mobile
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|mobile||mobile|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.19	设置手机号码

> PUT  /user/mobile
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|mobile||mobile|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.20	设置昵称

> POST  /user/nickname
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|nick_name||nick_name|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.21	设置昵称

> PUT  /user/nickname
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|nick_name||nick_name|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.22	查询用户在线状态

> GET  /user/online_status
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|用户在线信息|
|⇥ online|boolean||false|是否在线： true - 在线 ，false - 离线|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.23	设置私有扩展信息

> POST  /user/private
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.24	设置私有扩展信息

> PUT  /user/private
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.25	获取用户信息

> GET  /user/profile
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|用户信息|
|⇥ avatar|string||false|头像 url|
|⇥ description|string||false|描述信息|
|⇥ email|string||false|邮箱|
|⇥ mobile|string||false|手机号码|
|⇥ nick_name|string||false|昵称|
|⇥ private_info|string||false|私有信息，仅自己可见|
|⇥ public_info|string||false|公开信息，好友和陌生人可见|
|⇥ user_id|int32||false|用户ID|
|⇥ username|string||false|用户名|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.26	更新用户信息

> POST  /user/profile
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| description|string||false|描述信息|
| nick_name|string||false|昵称|
| private_info|string||false|私有信息，仅自己可见|
| public_info|string||false|公开信息，好友和陌生人可见|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.27	更新用户信息

> PUT  /user/profile
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| description|string||false|描述信息|
| nick_name|string||false|昵称|
| private_info|string||false|私有信息，仅自己可见|
| public_info|string||false|公开信息，好友和陌生人可见|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.28	批量更新用户信息

> POST  /user/profile/batch
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| list|array[object]||false||
|⇥ description|string||false|描述信息|
|⇥ nick_name|string||false|昵称|
|⇥ private_info|string||false|私有信息，仅自己可见|
|⇥ public_info|string||false|公开信息，好友和陌生人可见|
|⇥ user_id|int32||false|用户ID|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ reason|string||false|失败原因|
|⇥ success|boolean||false|是否成功|
|⇥ user_id|int32||false|用户ID|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.29	批量更新用户信息

> PUT  /user/profile/batch
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| list|array[object]||false||
|⇥ description|string||false|描述信息|
|⇥ nick_name|string||false|昵称|
|⇥ private_info|string||false|私有信息，仅自己可见|
|⇥ public_info|string||false|公开信息，好友和陌生人可见|
|⇥ user_id|int32||false|用户ID|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ reason|string||false|失败原因|
|⇥ success|boolean||false|是否成功|
|⇥ user_id|int32||false|用户ID|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.30	设置公开扩展信息

> POST  /user/public
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.31	设置公开扩展信息

> PUT  /user/public
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.32	设置是否关闭推送

> POST  /user/push
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|value||value|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.33	设置是否关闭推送

> PUT  /user/push
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|value||value|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.34	绑定别名

> POST  /user/push/alias
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| alias|string||false|别名|
| push_token|string||false|推送token|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.35	设置badge

> POST  /user/push/badge
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| badge|int32||false|badge|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.36	设置是否关闭推送详情

> POST  /user/push/detail
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|value||value|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.37	设置是否关闭推送详情

> PUT  /user/push/detail
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|value||value|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.38	设置推送免打扰时间

> POST  /user/push/limit
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|no_push_end_hour||no_push_end_hour|
|no_push_start_hour||no_push_start_hour|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.39	设置推送免打扰时间

> PUT  /user/push/limit
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|no_push_end_hour||no_push_end_hour|
|no_push_start_hour||no_push_start_hour|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.40	设置推送昵称

> POST  /user/push/nickname
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|value||value|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.41	设置推送昵称

> PUT  /user/push/nickname
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|value||value|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.42	获取标签

> GET  /user/push/tag
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[string]||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.43	绑定标签

> POST  /user/push/tag
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| tags|array[string]||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.44	解绑标签

> DELETE  /user/push/tag
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| tags|array[string]||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.45	删除所有标签

> DELETE  /user/push/tag/all
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.46	注册用户

> POST  /user/register
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| email|string||false|email|
| mobile|string||false|手机号码|
| password|string||false||
| username|string||false|用户名|
| verification_code|string||false|验证码，结合手机或邮箱使用|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|用户设置信息|
|⇥ auth_answer|string||false|验证问题答案|
|⇥ auth_mode|int32||false|验证方式, 0 - 无需验证，任何人可以加为好友, 1 - 需要同意方可加为好友, 2 - 需要回答问题正确方可加为好友, 3 - 拒绝所有加好友申请|
|⇥ auth_question|string||false|验证问题|
|⇥ auto_download|boolean||false|是否自动下载|
|⇥ group_confirm|boolean||false|邀请入群时是否需要用户确认: true - 需要用户同意才可加入， false - 自动同意邀请|
|⇥ id|int32||false||
|⇥ no_push|boolean||false|是否关闭推送消息|
|⇥ no_push_detail|boolean||false|是否推送详情|
|⇥ no_push_end_hour|int32||false|推送免打扰结束时间|
|⇥ no_push_start_hour|int32||false|推送免打扰开始时间|
|⇥ no_sounds|boolean||false|收到消息时是否静音|
|⇥ push_nick_name|string||false|推送昵称|
|⇥ push_token|string||false|推送token|
|⇥ silence_end_time|int32||false|推送不提醒结束时间|
|⇥ silence_start_time|int32||false|推送不提醒开始时间|
|⇥ user_id|int32||false|用户ID|
|⇥ vibratory|boolean||false|收到消息时否振动|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.47	批量注册用户

> POST  /user/register/batch
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| list|array[object]||false||
|⇥ password|string||false||
|⇥ username|string||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ reason|string||false|失败原因|
|⇥ success|boolean||false|是否成功|
|⇥ user_id|int32||false|用户ID|
|⇥ username|string||false|用户名|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.48	注册推送用户

> POST  /user/register/push
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| alias|string||false|别名|
| device_guid|string||false|设备ID|
| password|string||false||
| push_token|string||false|推送token|
| sign|string||false|签名|
| username|string||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|用户设置信息|
|⇥ auth_answer|string||false|验证问题答案|
|⇥ auth_mode|int32||false|验证方式, 0 - 无需验证，任何人可以加为好友, 1 - 需要同意方可加为好友, 2 - 需要回答问题正确方可加为好友, 3 - 拒绝所有加好友申请|
|⇥ auth_question|string||false|验证问题|
|⇥ auto_download|boolean||false|是否自动下载|
|⇥ group_confirm|boolean||false|邀请入群时是否需要用户确认: true - 需要用户同意才可加入， false - 自动同意邀请|
|⇥ id|int32||false||
|⇥ no_push|boolean||false|是否关闭推送消息|
|⇥ no_push_detail|boolean||false|是否推送详情|
|⇥ no_push_end_hour|int32||false|推送免打扰结束时间|
|⇥ no_push_start_hour|int32||false|推送免打扰开始时间|
|⇥ no_sounds|boolean||false|收到消息时是否静音|
|⇥ push_nick_name|string||false|推送昵称|
|⇥ push_token|string||false|推送token|
|⇥ silence_end_time|int32||false|推送不提醒结束时间|
|⇥ silence_start_time|int32||false|推送不提醒开始时间|
|⇥ user_id|int32||false|用户ID|
|⇥ vibratory|boolean||false|收到消息时否振动|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.49	注册用户

> POST  /user/register/v2
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| password|string||false||
| username|string||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|用户设置信息|
|⇥ auth_answer|string||false|验证问题答案|
|⇥ auth_mode|int32||false|验证方式, 0 - 无需验证，任何人可以加为好友, 1 - 需要同意方可加为好友, 2 - 需要回答问题正确方可加为好友, 3 - 拒绝所有加好友申请|
|⇥ auth_question|string||false|验证问题|
|⇥ auto_download|boolean||false|是否自动下载|
|⇥ group_confirm|boolean||false|邀请入群时是否需要用户确认: true - 需要用户同意才可加入， false - 自动同意邀请|
|⇥ id|int32||false||
|⇥ no_push|boolean||false|是否关闭推送消息|
|⇥ no_push_detail|boolean||false|是否推送详情|
|⇥ no_push_end_hour|int32||false|推送免打扰结束时间|
|⇥ no_push_start_hour|int32||false|推送免打扰开始时间|
|⇥ no_sounds|boolean||false|收到消息时是否静音|
|⇥ push_nick_name|string||false|推送昵称|
|⇥ push_token|string||false|推送token|
|⇥ silence_end_time|int32||false|推送不提醒结束时间|
|⇥ silence_start_time|int32||false|推送不提醒开始时间|
|⇥ user_id|int32||false|用户ID|
|⇥ vibratory|boolean||false|收到消息时否振动|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.50	获取用户设置

> GET  /user/settings
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|用户设置信息|
|⇥ auth_answer|string||false|验证问题答案|
|⇥ auth_mode|int32||false|验证方式, 0 - 无需验证，任何人可以加为好友, 1 - 需要同意方可加为好友, 2 - 需要回答问题正确方可加为好友, 3 - 拒绝所有加好友申请|
|⇥ auth_question|string||false|验证问题|
|⇥ auto_download|boolean||false|是否自动下载|
|⇥ group_confirm|boolean||false|邀请入群时是否需要用户确认: true - 需要用户同意才可加入， false - 自动同意邀请|
|⇥ id|int32||false||
|⇥ no_push|boolean||false|是否关闭推送消息|
|⇥ no_push_detail|boolean||false|是否推送详情|
|⇥ no_push_end_hour|int32||false|推送免打扰结束时间|
|⇥ no_push_start_hour|int32||false|推送免打扰开始时间|
|⇥ no_sounds|boolean||false|收到消息时是否静音|
|⇥ push_nick_name|string||false|推送昵称|
|⇥ push_token|string||false|推送token|
|⇥ silence_end_time|int32||false|推送不提醒结束时间|
|⇥ silence_start_time|int32||false|推送不提醒开始时间|
|⇥ user_id|int32||false|用户ID|
|⇥ vibratory|boolean||false|收到消息时否振动|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.51	修改用户设置

> POST  /user/settings
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| auth_answer|string||false|验证问题答案|
| auth_mode|int32||false|验证方式, 0 - 无需验证，任何人可以加为好友, 1 - 需要同意方可加为好友, 2 - 需要回答问题正确方可加为好友, 3 - 拒绝所有加好友申请|
| auth_question|string||false|验证问题|
| auto_download|boolean||false|是否自动下载|
| group_confirm|boolean||false|邀请入群时是否需要用户确认: true - 需要用户同意才可加入， false - 自动同意邀请|
| id|int32||false||
| no_push|boolean||false|是否关闭推送消息|
| no_push_detail|boolean||false|是否推送详情|
| no_push_end_hour|int32||false|推送免打扰结束时间|
| no_push_start_hour|int32||false|推送免打扰开始时间|
| no_sounds|boolean||false|收到消息时是否静音|
| push_nick_name|string||false|推送昵称|
| push_token|string||false|推送token|
| silence_end_time|int32||false|推送不提醒结束时间|
| silence_start_time|int32||false|推送不提醒开始时间|
| user_id|int32||false|用户ID|
| vibratory|boolean||false|收到消息时否振动|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.52	修改用户设置

> PUT  /user/settings
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| auth_answer|string||false|验证问题答案|
| auth_mode|int32||false|验证方式, 0 - 无需验证，任何人可以加为好友, 1 - 需要同意方可加为好友, 2 - 需要回答问题正确方可加为好友, 3 - 拒绝所有加好友申请|
| auth_question|string||false|验证问题|
| auto_download|boolean||false|是否自动下载|
| group_confirm|boolean||false|邀请入群时是否需要用户确认: true - 需要用户同意才可加入， false - 自动同意邀请|
| id|int32||false||
| no_push|boolean||false|是否关闭推送消息|
| no_push_detail|boolean||false|是否推送详情|
| no_push_end_hour|int32||false|推送免打扰结束时间|
| no_push_start_hour|int32||false|推送免打扰开始时间|
| no_sounds|boolean||false|收到消息时是否静音|
| push_nick_name|string||false|推送昵称|
| push_token|string||false|推送token|
| silence_end_time|int32||false|推送不提醒结束时间|
| silence_start_time|int32||false|推送不提醒开始时间|
| user_id|int32||false|用户ID|
| vibratory|boolean||false|收到消息时否振动|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.53	设置新消息是否关闭声音提醒

> POST  /user/sounds
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|value||value|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.54	设置新消息是否关闭声音提醒

> PUT  /user/sounds
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|value||value|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.55	绑定token

> POST  /user/token/bind
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| device_sn|int32||false|设备SN|
| device_token|string||false|device token|
| notifier_name|string||false|证书名称|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.56	绑定token

> PUT  /user/token/bind
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| device_sn|int32||false|设备SN|
| device_token|string||false|device token|
| notifier_name|string||false|证书名称|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.57	解绑token

> POST  /user/token/unbind
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|deviceSn||deviceSn|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.58	解绑token

> DELETE  /user/token/unbind
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|deviceSn||deviceSn|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.59	修改用户名

> POST  /user/username
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|username||username|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.60	修改用户名

> PUT  /user/username
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|username||username|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.61	设置新消息是否振动

> POST  /user/vibratory
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|value||value|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 3.62	设置新消息是否振动

> PUT  /user/vibratory
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|value||value|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 4	推送接口

## 4.1	获取推送证书

> GET  /push/certificate
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|environment||运行环境， 0 - 开发环境， 1 - 生产环境 , 默认值：1|
|provider||证书提供方, 1-APNS，2-华为，3-小米，4-魅族，5-VIVO， 6-OPPO, 7-FCM|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|推送证书信息|
|⇥ app_id|string||false|APP ID|
|⇥ app_key|string||false|APP KEY|
|⇥ app_secret|string||false|APP SECRET|
|⇥ certificate|string||false|证书|
|⇥ name|string||false|证书名称|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 4.2	发推送通知

> POST  /push/notify
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| audience|object||false|推送目标, 不可为空。类型为字符串或JSONObject:<br>"all", 表示发给所有设备<br>{"tag":["tag1","tag2"]} 表示发给标签为tag1或tag2的设备<br>{"alias":["alias1","alias2"]} 表示发给别名为alias1或alias2的设备<br>{"user_id":[111,222]} 表示发给用户ID为111或222的设备<br>{"push_token":["push_token1","push_token2"]} 表示发给PushToken为push_token1或push_token2的设备<br>使用标签/别名/用户ID/pushToken推送时，列表长度不能超过500<br>|
| setting|object||false|推送设置, 可为空|
|⇥ request_id|string||false|请求ID，用于请求去重，如果请求ID以前出现过，则不推送。可为空，为空则不去重。|
|⇥ distribution_strategy|string||false|通知下发策略: combined - 表示先使用美信通道下发，美信不在线，则使用厂商通道下发；mxpush_only - 表示只使用美信通道下发; ospush_only - 表示只使用厂商通道下发。 可为空，为空则默认为combined|
|⇥ ospush_sequence|array[string]||false|厂商推送顺序：ups - 国内厂商(小米/华为/魅族/oppo/vivo); fcm - FCM推送；huawei - 华为推送；xiaomi - 小米推送; oppo - OPPO推送; vivo - VIVO推送, meizu - 魅族推送。可为空，为空则默认为[ups,fcm]|
| message|object||false|推送消息体|
|⇥ type|string||false|消息类型：text - 文本，image - 图片， cmd - 透传消息。可为空，为空则默认为text|
|⇥ title|string||false|标题。可为空|
|⇥ body|string||false|内容。可为空|
|⇥ attachment_url|string||false|附件地址: 图片/音频/视频的URL地址。可为空。如果是图片地址，需要以jpg/jpeg/png结尾，图片大小需小于1M,推荐876*324px|
|⇥ big_text|string||false|大文本： 如果设置此字段，并且厂商支持推送大文本，则使用此字段推送大文本，否则使用body字段的文本推送普通文本|
|⇥ badge|string||false|应用角标: 如果为数字，则修改角标为此数字；如果以+开头，表示增加此数字到角标，如"+1", 表示角标数加1;如果为空，默认为"+1"|
|⇥ ext|object||false|扩展字段:可为空，类型为JSONObject, 例如: {"key1":123, "key2":"value2"}|
|⇥ show_begin_time|int32||false|定时展示的开始时间戳(秒), 为空时表示立即展示|
|⇥ show_end_time|int32||false|定时展示的结束时间戳(秒)，可为空|
|⇥ ios|object||false|ios平台额外参数，可为空|
|⇥⇥ sound|string||false|通知提示声音， 可为空|
|⇥⇥ content_available|boolean||false|对应APNs的content-available，可为空|
|⇥⇥ mutable_content|boolean||false|对应APNs的mutable-content， 可为空|
|⇥⇥ category|string||false|对应APNs Payload中的category， 可为空|
|⇥⇥ thread_id|string||false|对应APNs的thread-id，可为空，通过该属性来对通知进行分组，相同thread-id 的通知归为一组|
|⇥⇥ subtitle|string||false|对应APNs的subtitle，可为空|
|⇥⇥ apns_collapse_id|string||false|对应APNs的apns-collapse-id，可为空，通知携带apns-collapse-id 参数，将会覆盖通知中心里携带相同apns-collapse-id的通知。|
|⇥ android|object||false|android平台额外参数，可为空|
|⇥⇥ sound|string||false|通知提示声音，可为空|
|⇥⇥ channel_id|string||false|通知栏通道，可为空|
|⇥⇥ click_action|string||false|点击通知的后续动作: intent 打开应用特定页面; open_app 打开应用首页。可为空|
|⇥⇥ intent|string||false|点击通知打开应用特定页面: 可为空，click_action为intent时不可为空。示例：intent:#Intent;component=包名/activity全路径;S.parm1=value1;S.parm2=value2;end|
|⇥ huawei|object||false|huawei厂商额外参数, 可为空，如果设置，会覆盖Android里的相应属性|
|⇥⇥ sound|string||false|通知提示声音，可为空|
|⇥⇥ channel_id|string||false|通知栏通道，可为空|
|⇥⇥ click_action|string||false|点击通知的后续动作: intent 打开应用特定页面; open_app 打开应用首页。可为空|
|⇥⇥ intent|string||false|点击通知打开应用特定页面: 可为空，click_action为intent时不可为空。示例：intent:#Intent;component=包名/activity全路径;S.parm1=value1;S.parm2=value2;end|
|⇥⇥ badge_class|string||false|桌面图标对应的应用入口Activity类， 比如 com.test.badge.MainActivity， 可为空|
|⇥ xiaomi|object||false|xiaomi厂商额外参数, 可为空，如果设置，会覆盖Android里的相应属性|
|⇥⇥ sound|string||false|通知提示声音，可为空|
|⇥⇥ channel_id|string||false|通知栏通道，可为空|
|⇥⇥ click_action|string||false|点击通知的后续动作: intent 打开应用特定页面; open_app 打开应用首页。可为空|
|⇥⇥ intent|string||false|点击通知打开应用特定页面: 可为空，click_action为intent时不可为空。示例：intent:#Intent;component=包名/activity全路径;S.parm1=value1;S.parm2=value2;end|
|⇥ oppo|object||false|oppo厂商额外参数, 可为空，如果设置，会覆盖Android里的相应属性|
|⇥⇥ sound|string||false|通知提示声音，可为空|
|⇥⇥ channel_id|string||false|通知栏通道，可为空|
|⇥⇥ click_action|string||false|点击通知的后续动作: intent 打开应用特定页面; open_app 打开应用首页。可为空|
|⇥⇥ intent|string||false|点击通知打开应用特定页面: 可为空，click_action为intent时不可为空。示例：intent:#Intent;component=包名/activity全路径;S.parm1=value1;S.parm2=value2;end|
|⇥ vivo|object||false|vivo厂商额外参数, 可为空，如果设置，会覆盖Android里的相应属性|
|⇥⇥ sound|string||false|通知提示声音，可为空|
|⇥⇥ channel_id|string||false|通知栏通道，可为空|
|⇥⇥ click_action|string||false|点击通知的后续动作: intent 打开应用特定页面; open_app 打开应用首页。可为空|
|⇥⇥ intent|string||false|点击通知打开应用特定页面: 可为空，click_action为intent时不可为空。示例：intent:#Intent;component=包名/activity全路径;S.parm1=value1;S.parm2=value2;end|
|⇥⇥ push_mode|int32||false|推送模式： 0-正式推送；1-测试推送，不填默认为0|
|⇥⇥ classification|int32||false|消息类型 0：运营类消息，1：系统类消息。不填默认为0|
|⇥ flyme|object||false|魅族厂商额外参数, 可为空，如果设置，会覆盖Android里的相应属性|
|⇥⇥ sound|string||false|通知提示声音，可为空|
|⇥⇥ channel_id|string||false|通知栏通道，可为空|
|⇥⇥ click_action|string||false|点击通知的后续动作: intent 打开应用特定页面; open_app 打开应用首页。可为空|
|⇥⇥ intent|string||false|点击通知打开应用特定页面: 可为空，click_action为intent时不可为空。示例：intent:#Intent;component=包名/activity全路径;S.parm1=value1;S.parm2=value2;end|
|⇥ fcm|object||false|FCM厂商额外参数, 可为空，如果设置，会覆盖Android里的相应属性|
|⇥⇥ sound|string||false|通知提示声音，可为空|
|⇥⇥ channel_id|string||false|通知栏通道，可为空|
|⇥⇥ click_action|string||false|点击通知的后续动作: intent 打开应用特定页面; open_app 打开应用首页。可为空|
|⇥⇥ intent|string||false|点击通知打开应用特定页面: 可为空，click_action为intent时不可为空。示例：intent:#Intent;component=包名/activity全路径;S.parm1=value1;S.parm2=value2;end|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false||
|⇥ task_id|int32||false|任务ID|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 发送推送通知需要在管理后台开通推送功能。
具体请求参数可以参考Model里的定义。
常用请求格式如下:
1. 推送文本给所有设备
{
  "audience": "all",
  "message": {
    "type": "text",
    "title": "this is push title",
    "body": "this is push body"
  }
}
2. 推送图片给push_token为token1或token2的设备
{
  "audience": {"push_token":["token1","token2"]},
  "message": {
    "type": "image",
    "title": "this is push title",
    "body": "this is push body",
    "attachment_url": "https://xxx.com/images/1.jpg"
  }
}
3. 推送透传消息给标签为beijing或shanghai的所有设备，透传消息不会展示到通知栏上
{
  "audience": {"tag":["beijing","shanghai"]},
  "message": {
    "type": "cmd",
    "title": "this is push title",
    "body": "this is push body",
    "ext": {"key1": 12345, "key2": "xxx" }
  }
}




## 4.3	查询推送统计结果

> POST  /push/task/detail
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| list|array[int32]||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ apns_received|int32||false|APNs通道送达数|
|⇥ apns_sent|int32||false|APNs通道发送数|
|⇥ apns_target|int32||false|APNs通道有效目标数|
|⇥ fcm_received|int32||false|FCM通道送达数|
|⇥ fcm_sent|int32||false|FCM通道发送数|
|⇥ fcm_target|int32||false|FCM通道有效目标数|
|⇥ flyme_received|int32||false|魅族通道送达数|
|⇥ flyme_sent|int32||false|魅族通道发送数|
|⇥ flyme_target|int32||false|魅族通道有效目标数|
|⇥ huawei_received|int32||false|华为通道送达数|
|⇥ huawei_sent|int32||false|华为通道发送数|
|⇥ huawei_target|int32||false|华为通道有效目标数|
|⇥ mxpush_received|int32||false|美信通道送达数|
|⇥ mxpush_sent|int32||false|美信通道发送数|
|⇥ mxpush_target|int32||false|美信通道有效目标数|
|⇥ oppo_received|int32||false|oppo通道送达数|
|⇥ oppo_sent|int32||false|oppo通道发送数|
|⇥ oppo_target|int32||false|oppo通道有效目标数|
|⇥ vivo_received|int32||false|vivo通道送达数|
|⇥ vivo_sent|int32||false|vivo通道发送数|
|⇥ vivo_target|int32||false|vivo通道有效目标数|
|⇥ xiaomi_received|int32||false|小米通道送达数|
|⇥ xiaomi_sent|int32||false|小米通道发送数|
|⇥ xiaomi_target|int32||false|小米通道有效目标数|
|⇥ task_id|int32||false|推送任务ID|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 5	token 接口

## 5.1	通过用户ID和密码取普通用户token

> POST  /token/id
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| device_guid|string||false|设备ID, 如果设置，则返回PushToken|
| password|string||false||
| user_id|int32||false|用户ID，仅用于用户ID登录|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|Token 信息|
|⇥ access_key_secret|string||false|文件密钥|
|⇥ encrypt_type|int32||false|是否启用加密连接|
|⇥ expire|int32||false|过期时间戳|
|⇥ public_key|string||false|公钥|
|⇥ push_token|string||false|推送Token|
|⇥ store_token|string||false|文件token|
|⇥ token|string||false|访问token|
|⇥ user_id|int32||false|用户ID|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 5.2	通过用户名/手机号/邮箱取普通用户token

> POST  /token/login
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| device_guid|string||false|设备ID, 如果设置，则返回PushToken|
| login_name|string||false|登录名，可以是手机号，邮箱，用户名|
| password|string||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|Token 信息|
|⇥ access_key_secret|string||false|文件密钥|
|⇥ encrypt_type|int32||false|是否启用加密连接|
|⇥ expire|int32||false|过期时间戳|
|⇥ public_key|string||false|公钥|
|⇥ push_token|string||false|推送Token|
|⇥ store_token|string||false|文件token|
|⇥ token|string||false|访问token|
|⇥ user_id|int32||false|用户ID|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 5.3	通过用户名和密码取普通用户token

> POST  /token/user
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| device_guid|string||false|设备ID, 如果设置，则返回PushToken|
| name|string||false|用户名，仅用于用户名登录|
| password|string||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|Token 信息|
|⇥ access_key_secret|string||false|文件密钥|
|⇥ encrypt_type|int32||false|是否启用加密连接|
|⇥ expire|int32||false|过期时间戳|
|⇥ public_key|string||false|公钥|
|⇥ push_token|string||false|推送Token|
|⇥ store_token|string||false|文件token|
|⇥ token|string||false|访问token|
|⇥ user_id|int32||false|用户ID|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 6	消息处理

## 6.1	发送已读回执

> GET  /message/ack
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|conversation_id||conversation_id|
|device_sn||device_sn|
|msg_id||msg_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 6.2	取指定会话的消息

> GET  /message/conversation
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|limit||limit|
|msg_id_start||msg_id_start|
|opposite_id||opposite_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false||
|⇥ is_last|boolean||false||
|⇥ messages|array[object]||false||
|⇥⇥ attachment|string||false||
|⇥⇥ config|string||false||
|⇥⇥ content|string||false||
|⇥⇥ ctype|string||false||
|⇥⇥ ext|string||false||
|⇥⇥ from_xid|object||false||
|⇥⇥⇥ device_sn|int32||false||
|⇥⇥⇥ set_device_sn|boolean||false||
|⇥⇥⇥ set_uid|boolean||false||
|⇥⇥⇥ uid|int32||false||
|⇥⇥ msg_id|int32||false||
|⇥⇥ set_attachment|boolean||false||
|⇥⇥ set_config|boolean||false||
|⇥⇥ set_content|boolean||false||
|⇥⇥ set_ctype|boolean||false||
|⇥⇥ set_ext|boolean||false||
|⇥⇥ set_from_xid|boolean||false||
|⇥⇥ set_msg_id|boolean||false||
|⇥⇥ set_status|boolean||false||
|⇥⇥ set_timestamp|boolean||false||
|⇥⇥ set_to_xid|boolean||false||
|⇥⇥ status|string||false||
|⇥⇥ timestamp|int32||false||
|⇥⇥ to_xid|object||false||
|⇥⇥⇥ device_sn|int32||false||
|⇥⇥⇥ set_device_sn|boolean||false||
|⇥⇥⇥ set_uid|boolean||false||
|⇥⇥⇥ uid|int32||false||
|⇥ messages_iterator|object||false||
|⇥ messages_size|int32||false||
|⇥ next_msg_id|int32||false||
|⇥ set_is_last|boolean||false||
|⇥ set_messages|boolean||false||
|⇥ set_next_msg_id|boolean||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 6.3	删除用户的指定会话

> DELETE  /message/conversation
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|conversation_id||conversation_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 6.4	发送系统通知

> POST  /message/notify
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| attachment|string||false||
| config|string||false||
| content|string||false||
| content_type|int32||false|消息类型 TEXT      = 0;<br>    IMAGE     = 1;<br>    AUDIO     = 2;<br>    VIDEO     = 3;<br>    FILE      = 4;<br>    LOCATION  = 5;<br>    COMMAND   = 6;<br>    FORWARD   = 7;|
| ext|string||false||
| from_user_id|int32||false|发送者的用户ID|
| targets|array[int32]||false|接收用户ID或群ID|
| transaction_id|int32||false|请求ID，用于消息去重， 如果短时间内收到2个相同transaction_id的请求，第二次请求不会被执行。 如果不设置就不会被去重|
| type|int32||false|目标类型，1 - 普通用户，2 - 群组|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 6.5	发送系统通知

> PUT  /message/notify
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| attachment|string||false||
| config|string||false||
| content|string||false||
| content_type|int32||false|消息类型 TEXT      = 0;<br>    IMAGE     = 1;<br>    AUDIO     = 2;<br>    VIDEO     = 3;<br>    FILE      = 4;<br>    LOCATION  = 5;<br>    COMMAND   = 6;<br>    FORWARD   = 7;|
| ext|string||false||
| from_user_id|int32||false|发送者的用户ID|
| targets|array[int32]||false|接收用户ID或群ID|
| transaction_id|int32||false|请求ID，用于消息去重， 如果短时间内收到2个相同transaction_id的请求，第二次请求不会被执行。 如果不设置就不会被去重|
| type|int32||false|目标类型，1 - 普通用户，2 - 群组|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 6.6	发送消息

> POST  /message/send
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| attachment|string||false||
| config|string||false||
| content|string||false||
| content_type|int32||false|消息类型 TEXT      = 0;<br>    IMAGE     = 1;<br>    AUDIO     = 2;<br>    VIDEO     = 3;<br>    FILE      = 4;<br>    LOCATION  = 5;<br>    COMMAND   = 6;<br>    FORWARD   = 7;|
| ext|string||false||
| from_user_id|int32||false|发送者的用户ID|
| targets|array[int32]||false|接收用户ID或群ID|
| transaction_id|int32||false|请求ID，用于消息去重， 如果短时间内收到2个相同transaction_id的请求，第二次请求不会被执行。 如果不设置就不会被去重|
| type|int32||false|目标类型，1 - 普通用户，2 - 群组|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 6.7	发送消息

> PUT  /message/send
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| attachment|string||false||
| config|string||false||
| content|string||false||
| content_type|int32||false|消息类型 TEXT      = 0;<br>    IMAGE     = 1;<br>    AUDIO     = 2;<br>    VIDEO     = 3;<br>    FILE      = 4;<br>    LOCATION  = 5;<br>    COMMAND   = 6;<br>    FORWARD   = 7;|
| ext|string||false||
| from_user_id|int32||false|发送者的用户ID|
| targets|array[int32]||false|接收用户ID或群ID|
| transaction_id|int32||false|请求ID，用于消息去重， 如果短时间内收到2个相同transaction_id的请求，第二次请求不会被执行。 如果不设置就不会被去重|
| type|int32||false|目标类型，1 - 普通用户，2 - 群组|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 6.8	取指定用户的最近会话列表

> GET  /message/unread
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ conversation_id|object||false||
|⇥⇥ device_sn|int32||false||
|⇥⇥ set_device_sn|boolean||false||
|⇥⇥ set_uid|boolean||false||
|⇥⇥ uid|int32||false||
|⇥ num|int32||false||
|⇥ set_conversation_id|boolean||false||
|⇥ set_num|boolean||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7	群接口

## 7.1	添加群管理员

> POST  /group/admin/add
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| user_list|array[int32]||false|用户id列表|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ reason|string||false||
|⇥ result|string||false||
|⇥ user_id|int32||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.2	移除群管理员

> POST  /group/admin/remove
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| user_list|array[int32]||false|用户id列表|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ reason|string||false||
|⇥ result|string||false||
|⇥ user_id|int32||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.3	移除群管理员

> DELETE  /group/admin/remove
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| user_list|array[int32]||false|用户id列表|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ reason|string||false||
|⇥ result|string||false||
|⇥ user_id|int32||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.4	获取群管理员列表

> GET  /group/admin_list
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|group_id||group_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ display_name|string||false|成员群名片|
|⇥ join_time|int32||false|成员入群时间|
|⇥ user_id|int32||false|用户id|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.5	根据群id和公告id获取群公告详情

> GET  /group/announcement
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|announcement_id||announcement_id|
|group_id||group_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false||
|⇥ author|int32||false|公告发布者|
|⇥ content|string||false|公告内容|
|⇥ created_at|int32||false|公告发布时间|
|⇥ group_id|int32||false|群id|
|⇥ id|int32||false|公告id|
|⇥ title|string||false|公告标题|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.6	删除公告

> POST  /group/announcement/delete
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|announcement_id||announcement_id|
|group_id||group_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.7	删除公告

> DELETE  /group/announcement/delete
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|announcement_id||announcement_id|
|group_id||group_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.8	编辑群公告

> POST  /group/announcement/edit
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| content|string||false|公告内容|
| group_id|int32||false|群组id|
| title|string||false|公告标题|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false||
|⇥ author|int32||false|公告发布者|
|⇥ content|string||false|公告内容|
|⇥ created_at|int32||false|公告发布时间|
|⇥ group_id|int32||false|群id|
|⇥ id|int32||false|公告id|
|⇥ title|string||false|公告标题|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.9	获取最新一条群公告详情

> GET  /group/announcement/last
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|group_id||group_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false||
|⇥ author|int32||false|公告发布者|
|⇥ content|string||false|公告内容|
|⇥ created_at|int32||false|公告发布时间|
|⇥ group_id|int32||false|群id|
|⇥ id|int32||false|公告id|
|⇥ title|string||false|公告标题|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.10	获取群公告列表

> GET  /group/announcement/list
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|group_id||group_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ author|int32||false|公告发布者|
|⇥ content|string||false|公告内容|
|⇥ created_at|int32||false|公告发布时间|
|⇥ group_id|int32||false|群id|
|⇥ id|int32||false|公告id|
|⇥ title|string||false|公告标题|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.11	获取群申请列表

> POST  /group/application_list
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|cursor||cursor|
|limit||limit|
|version||version|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_list|array[int32]||false|群id列表|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| cursor|string||false|游标，用于翻页|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|
| total|int32||false|总数|
| version|int32||false|版本，目前没用到，留作扩展|

##### 接口描述
> 




## 7.12	申请入群

> POST  /group/apply
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| reason|string||false|申请入群原因|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false||
|⇥ reason|string||false||
|⇥ result|string||false||
|⇥ user_id|int32||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.13	管理员处理入群申请

> POST  /group/apply/handle
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| approval|boolean||false|审批，bool类型，true为同意，false为拒绝|
| group_id|int32||false|群id|
| user_id|int32||false|用户id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false||
|⇥ reason|string||false||
|⇥ result|string||false||
|⇥ user_id|int32||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.14	管理员处理入群申请

> PUT  /group/apply/handle
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| approval|boolean||false|审批，bool类型，true为同意，false为拒绝|
| group_id|int32||false|群id|
| user_id|int32||false|用户id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false||
|⇥ reason|string||false||
|⇥ result|string||false||
|⇥ user_id|int32||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.15	将用户禁言

> POST  /group/ban
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| duration|int32||false|禁言时长，单位为分钟|
| group_id|int32||false|群id|
| user_list|array[int32]||false|用户id列表|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ reason|string||false||
|⇥ result|string||false||
|⇥ user_id|int32||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.16	获取禁言列表

> GET  /group/banned_list
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|cursor||cursor|
|group_id||group_id|
|limit||limit|
|version||version|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| cursor|string||false|游标，用于翻页|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|
| total|int32||false|总数|
| version|int32||false|版本，目前没用到，留作扩展|

##### 接口描述
> 




## 7.17	将用户加入黑名单

> POST  /group/block
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| user_list|array[int32]||false|用户id列表|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ reason|string||false||
|⇥ result|string||false||
|⇥ user_id|int32||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.18	获取黑名单列表

> GET  /group/blocked_list
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|cursor||cursor|
|group_id||group_id|
|limit||limit|
|version||version|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| cursor|string||false|游标，用于翻页|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|
| total|int32||false|总数|
| version|int32||false|版本，目前没用到，留作扩展|

##### 接口描述
> 




## 7.19	创建群

> POST  /group/create
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| avatar|string||false|群头像|
| description|string||false|群描述|
| name|string||false|群名称|
| type|int32||false|群类型 1表示公开群，0表示私有群, 2表示聊天室|
| user_list|array[int32]||false|邀请入群的用户id列表|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.20	解散群

> POST  /group/destroy
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|group_id||group_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.21	解散群

> DELETE  /group/destroy
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|group_id||group_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.22	更新群名片

> POST  /group/display_name
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|string||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.23	更新群名片

> PUT  /group/display_name
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|string||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.24	下载群文件

> GET  /group/file
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|file_id||file_id|
|group_id||group_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|群共享文件返回格式|
|⇥ created_at|int32||false||
|⇥ file_id|int32||false|共享文件id|
|⇥ group_id|int32||false|群id|
|⇥ name|string||false|共享文件名称|
|⇥ size|int32||false|共享文件大小|
|⇥ type|string||false|共享文件类型|
|⇥ updated_at|int32||false||
|⇥ uploader|int32||false|共享文件上传者|
|⇥ url|string||false|共享文件url|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.25	删除群文件

> POST  /group/file/delete
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| file_list|array[int32]||false|文件id列表|
| group_id|int32||false|群id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ file_id|int32||false||
|⇥ reason|string||false||
|⇥ result|string||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.26	删除群文件

> DELETE  /group/file/delete
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| file_list|array[int32]||false|文件id列表|
| group_id|int32||false|群id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ file_id|int32||false||
|⇥ reason|string||false||
|⇥ result|string||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.27	获取群文件列表

> GET  /group/file/list
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|group_id||group_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ created_at|int32||false||
|⇥ file_id|int32||false|共享文件id|
|⇥ group_id|int32||false|群id|
|⇥ name|string||false|共享文件名称|
|⇥ size|int32||false|共享文件大小|
|⇥ type|string||false|共享文件类型|
|⇥ updated_at|int32||false||
|⇥ uploader|int32||false|共享文件上传者|
|⇥ url|string||false|共享文件url|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.28	更新群文件名称

> POST  /group/file/update_name
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| file_id|int32||false|文件id|
| group_id|int32||false|群id|
| name|string||false|文件新名称|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.29	更新群文件名称

> PUT  /group/file/update_name
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| file_id|int32||false|文件id|
| group_id|int32||false|群id|
| name|string||false|文件新名称|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.30	上传群文件

> POST  /group/file/upload
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| name|string||false|文件名称|
| size|int32||false|文件大小|
| type|string||false|文件类型|
| url|string||false|文件url|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|群共享文件返回格式|
|⇥ created_at|int32||false||
|⇥ file_id|int32||false|共享文件id|
|⇥ group_id|int32||false|群id|
|⇥ name|string||false|共享文件名称|
|⇥ size|int32||false|共享文件大小|
|⇥ type|string||false|共享文件类型|
|⇥ updated_at|int32||false||
|⇥ uploader|int32||false|共享文件上传者|
|⇥ url|string||false|共享文件url|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.31	根据group id获取群信息

> GET  /group/info
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|group_id||group_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false||
|⇥ apply_approval|int32||false|入群申请审批设置, 0:同意所有申请 1:需要管理员确认 2:拒绝所有申请|
|⇥ avatar|string||false|群头像|
|⇥ ban_expire_time|int32||false|全员禁言过期时间（秒），禁言期间只允许管理员发消息， 为0或小于当前时间表示不禁言, -1表示永久禁言|
|⇥ created_at|int32||false|创建时间|
|⇥ description|string||false|群描述|
|⇥ ext|string||false|群扩展信息|
|⇥ group_id|int32||false|群id|
|⇥ history_visible|boolean||false|新成员可见历史聊天记录设置|
|⇥ member_invite|boolean||false|群成员邀请设置|
|⇥ member_modify|boolean||false|群成员修改群信息设置|
|⇥ msg_mute_mode|int32||false|群消息屏蔽模式|
|⇥ msg_push_mode|int32||false|群消息推送模式|
|⇥ name|string||false|群名称|
|⇥ owner_id|int32||false|群主id|
|⇥ read_ack|boolean||false|群消息已读功能设置|
|⇥ status|int32||false|群状态, 0：正常, 1：已解散|
|⇥ type|int32||false|群类型|
|⇥ updated_at|int32||false|更新时间|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.32	更新群头像

> POST  /group/info/avatar
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|string||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.33	更新群头像

> PUT  /group/info/avatar
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|string||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.34	根据group id获取群信息

> POST  /group/info/batch
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_list|array[int32]||false|群id列表|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ apply_approval|int32||false|入群申请审批设置, 0:同意所有申请 1:需要管理员确认 2:拒绝所有申请|
|⇥ avatar|string||false||
|⇥ capacity|int32||false||
|⇥ count|int32||false||
|⇥ group_id|int32||false||
|⇥ msg_mute_mode|int32||false|群消息屏蔽设置|
|⇥ msg_push_mode|int32||false|群消息推送设置|
|⇥ name|string||false||
|⇥ owner|int32||false||
|⇥ status|int32||false|群状态, 0：正常, 1：已解散|
|⇥ type|int32||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.35	更新群描述

> POST  /group/info/description
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|string||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.36	更新群描述

> PUT  /group/info/description
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|string||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.37	更新扩展信息

> POST  /group/info/ext
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|string||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.38	更新扩展信息

> PUT  /group/info/ext
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|string||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.39	更新群名称

> POST  /group/info/name
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|string||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.40	更新群名称

> PUT  /group/info/name
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|string||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.41	获取群邀请列表

> GET  /group/invitation_list
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|cursor||cursor|
|limit||limit|
|version||version|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| cursor|string||false|游标，用于翻页|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|
| total|int32||false|总数|
| version|int32||false|版本，目前没用到，留作扩展|

##### 接口描述
> 




## 7.42	邀请入群

> POST  /group/invite
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| reason|string||false|邀请理由|
| user_list|array[int32]||false|受邀请者id，List类型，单次可邀请多个用户入群|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ reason|string||false||
|⇥ result|string||false||
|⇥ user_id|int32||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.43	用户处理入群邀请

> POST  /group/invite/handle
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| approval|boolean||false|审批，bool类型，true为同意，false为拒绝|
| group_id|int32||false|群id|
| user_id|int32||false|用户id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.44	用户处理入群邀请

> PUT  /group/invite/handle
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| approval|boolean||false|审批，bool类型，true为同意，false为拒绝|
| group_id|int32||false|群id|
| user_id|int32||false|用户id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.45	将成员踢出群

> POST  /group/kick
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| user_list|array[int32]||false|用户id列表|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ reason|string||false||
|⇥ result|string||false||
|⇥ user_id|int32||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.46	将成员踢出群

> DELETE  /group/kick
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| user_list|array[int32]||false|用户id列表|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ reason|string||false||
|⇥ result|string||false||
|⇥ user_id|int32||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.47	成员退出群

> POST  /group/leave
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|group_id||group_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.48	成员退出群

> DELETE  /group/leave
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|group_id||group_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.49	根据group id获取群成员列表

> GET  /group/member_list
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|cursor||cursor|
|group_id||group_id|
|limit||limit|
|version||version|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| cursor|string||false|游标，用于翻页|
| data|array[object]||false|结果数据|
|⇥ display_name|string||false|成员群名片|
|⇥ join_time|int32||false|成员入群时间|
|⇥ user_id|int32||false|用户id|
| message|string||false|错误信息，如果成功，该项为null|
| total|int32||false|总数|
| version|int32||false|版本，目前没用到，留作扩展|

##### 接口描述
> 




## 7.50	批量获取群成员的群名片

> POST  /group/members/display_name
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| user_list|array[int32]||false|用户id列表|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ display_name|string||false|成员群名片|
|⇥ join_time|int32||false|成员入群时间|
|⇥ user_id|int32||false|用户id|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.51	设置群消息屏蔽模式

> POST  /group/msg/mute_mode
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| msg_mute_mode|int32||false|群消息屏蔽模式： 0 不屏蔽1 屏蔽本地消息通知2 屏蔽消息，不接收消息|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.52	设置群消息屏蔽模式

> PUT  /group/msg/mute_mode
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| msg_mute_mode|int32||false|群消息屏蔽模式： 0 不屏蔽1 屏蔽本地消息通知2 屏蔽消息，不接收消息|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.53	设置群消息推送模式

> POST  /group/msg/push_mode
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| msg_push_mode|int32||false|群消息推送类型： 0:接收所有推送;1:不接受推送;2:接收管理员和@消息推送;3:只接收管理员消息推送;4:只接收@消息推送|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.54	设置群消息推送模式

> PUT  /group/msg/push_mode
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| msg_push_mode|int32||false|群消息推送类型： 0:接收所有推送;1:不接受推送;2:接收管理员和@消息推送;3:只接收管理员消息推送;4:只接收@消息推送|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.55	获取公开群列表

> GET  /group/public_list
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[int32]||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.56	二维码邀请入群

> POST  /group/qrcode/invite
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| qr_info|string||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.57	获取群邀请二维码信息

> GET  /group/qrcode/sign
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|group_id||group_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false||
|⇥ create_at|int32||false|二维码生成时间|
|⇥ expire_at|int32||false|二维码过期时间|
|⇥ qr_info|string||false|二维码信息|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.58	获取群设置

> GET  /group/settings
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|group_id||group_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false||
|⇥ apply_approval|int32||false|入群申请审批设置, 0:同意所有申请 1:需要管理员确认 2:拒绝所有申请|
|⇥ avatar|string||false|群头像|
|⇥ ban_expire_time|int32||false|全员禁言过期时间（秒），禁言期间只允许管理员发消息， 为0或小于当前时间表示不禁言, -1表示永久禁言|
|⇥ created_at|int32||false|创建时间|
|⇥ description|string||false|群描述|
|⇥ ext|string||false|群扩展信息|
|⇥ group_id|int32||false|群id|
|⇥ history_visible|boolean||false|新成员可见历史聊天记录设置|
|⇥ member_invite|boolean||false|群成员邀请设置|
|⇥ member_modify|boolean||false|群成员修改群信息设置|
|⇥ msg_mute_mode|int32||false|群消息屏蔽模式|
|⇥ msg_push_mode|int32||false|群消息推送模式|
|⇥ name|string||false|群名称|
|⇥ owner_id|int32||false|群主id|
|⇥ read_ack|boolean||false|群消息已读功能设置|
|⇥ status|int32||false|群状态, 0：正常, 1：已解散|
|⇥ type|int32||false|群类型|
|⇥ updated_at|int32||false|更新时间|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.59	更新群设置--是否允许成员邀请

> POST  /group/settings/allow_member_invitation
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|boolean||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.60	更新群设置--是否允许成员邀请

> PUT  /group/settings/allow_member_invitation
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|boolean||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.61	更新群设置--群成员是否可修改群信息

> POST  /group/settings/allow_member_modify
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|boolean||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.62	更新群设置--群成员是否可修改群信息

> PUT  /group/settings/allow_member_modify
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|boolean||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.63	全员禁言，只允许管理员发消息

> POST  /group/settings/ban_all
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| duration|int32||false|禁言时长，单位为分钟|
| group_id|int32||false|群id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false||
|⇥ ban_expire_time|int32||false|全员禁言过期时间|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.64	更新群设置--是否开启群消息已读功能

> POST  /group/settings/enable_read_ack
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|boolean||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.65	更新群设置--是否开启群消息已读功能

> PUT  /group/settings/enable_read_ack
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|boolean||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.66	更新群设置--新成员是否可见群历史聊天记录

> POST  /group/settings/history_visible
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|boolean||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.67	更新群设置--新成员是否可见群历史聊天记录

> PUT  /group/settings/history_visible
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| value|boolean||false|更新内容|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.68	更新群设置--群申请是否需要管理员审批

> POST  /group/settings/require_admin_approval
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| apply_approval|int32||false|入群申请审批设置, 0:同意所有申请 1:需要管理员确认 2:拒绝所有申请|
| group_id|int32||false|群id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.69	更新群设置--群申请是否需要管理员审批

> PUT  /group/settings/require_admin_approval
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| apply_approval|int32||false|入群申请审批设置, 0:同意所有申请 1:需要管理员确认 2:拒绝所有申请|
| group_id|int32||false|群id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.70	取消全员禁言

> POST  /group/settings/unban_all
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.71	转让群

> POST  /group/transfer
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| new_owner|int32||false|新群主的user_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false||
|⇥ reason|string||false||
|⇥ result|string||false||
|⇥ user_id|int32||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.72	转让群

> PUT  /group/transfer
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| new_owner|int32||false|新群主的user_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false||
|⇥ reason|string||false||
|⇥ result|string||false||
|⇥ user_id|int32||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.73	从禁言列表移除用户

> POST  /group/unban
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| user_list|array[int32]||false|用户id列表|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ reason|string||false||
|⇥ result|string||false||
|⇥ user_id|int32||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.74	从黑名单移除用户

> POST  /group/unblock
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| user_list|array[int32]||false|用户id列表|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ reason|string||false||
|⇥ result|string||false||
|⇥ user_id|int32||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.75	从黑名单移除用户

> DELETE  /group/unblock
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| group_id|int32||false|群id|
| user_list|array[int32]||false|用户id列表|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ reason|string||false||
|⇥ result|string||false||
|⇥ user_id|int32||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 7.76	获取用户的群组列表

> GET  /group/user_joined
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[int32]||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8	好友管理接口

## 8.1	同意好友申请

> POST  /roster/accept
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|user_id||user_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.2	同意好友申请

> PUT  /roster/accept
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|user_id||user_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.3	申请加好友

> POST  /roster/apply
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| alias|string||false|备注名称|
| auth_answer|string||false|问题答案|
| reason|string||false|申请描述|
| user_id|int32||false|被申请用户 ID|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.4	批量添加好友

> POST  /roster/apply/batch
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| alias|string||false|备注名称|
| reason|string||false|申请描述|
| user_id|int32||false|被申请用户 ID|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|批量添加好友返回结果|
|⇥ fails|array[object]||false||
|⇥⇥ reason|string||false|失败原因|
|⇥⇥ user_id|int32||false|用户ID|
|⇥ success|array[int32]||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.5	好友申请列表

> GET  /roster/apply/list
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|cursor||cursor|
|limit||limit|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| cursor|string||false|游标，返回结果中缺失 cursor，表示已经返回最后一页|
| data|array[object]||false|结果数据|
|⇥ expired_time|int32||false|过期时间|
|⇥ reason|string||false|申请描述|
|⇥ status|int32||false||
|⇥ user_id|int32||false|发起加好友申请的用户ID|
| message|string||false|错误信息，如果成功，该项为null|
| version|int32||false|版本|

##### 接口描述
> 




## 8.6	添加黑名单

> POST  /roster/block
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|user_id||user_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.7	添加黑名单

> PUT  /roster/block
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|user_id||user_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.8	黑名单列表

> GET  /roster/blocked_list
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[int32]||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.9	拒绝好友申请

> POST  /roster/decline
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| reason|string||false|拒绝的原因|
| user_id|int32||false|拒绝的用户ID|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.10	拒绝好友申请

> PUT  /roster/decline
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| reason|string||false|拒绝的原因|
| user_id|int32||false|拒绝的用户ID|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.11	删除好友

> POST  /roster/delete
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|user_id||user_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.12	删除好友

> DELETE  /roster/delete
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|user_id||user_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.13	更新好友扩展信息

> POST  /roster/ext
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| alias|string||false|备注名称|
| ext|string||false|扩展信息|
| mute_notification|boolean||false|是否接收消息提醒|
| user_id|int32||false|好友用户ID|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.14	更新好友扩展信息

> PUT  /roster/ext
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| alias|string||false|备注名称|
| ext|string||false|扩展信息|
| mute_notification|boolean||false|是否接收消息提醒|
| user_id|int32||false|好友用户ID|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.15	用ID搜索用户

> GET  /roster/id
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|user_id||用户ID|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|好友列表|
|⇥ alias|string||false||
|⇥ auth_mode|int32||false|验证方式, 0 - 无需验证，任何人可以加为好友, 1 - 需要同意方可加为好友, 2 - 需要回答问题正确方可加为好友, 3 - 拒绝所有加好友申请|
|⇥ auth_question|string||false|验证问题|
|⇥ avatar|string||false|头像|
|⇥ description|string||false|描述信息|
|⇥ ext|string||false||
|⇥ mute_notification|boolean||false||
|⇥ nick_name|string||false|昵称或名称|
|⇥ public_info|string||false|公开信息，好友和陌生人可见|
|⇥ relation|int32||false||
|⇥ user_id|int32||false|好友用户ID|
|⇥ username|string||false|用户名|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.16	好友列表

> GET  /roster/list
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|cursor||cursor|
|limit||limit|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| cursor|string||false|游标，返回结果中缺失 cursor，表示已经返回最后一页|
| data|array[int32]||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|
| version|int32||false|版本|

##### 接口描述
> 




## 8.17	好友详情列表

> POST  /roster/list
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| list|array[int32]||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|array[object]||false|结果数据|
|⇥ alias|string||false||
|⇥ auth_mode|int32||false|验证方式, 0 - 无需验证，任何人可以加为好友, 1 - 需要同意方可加为好友, 2 - 需要回答问题正确方可加为好友, 3 - 拒绝所有加好友申请|
|⇥ auth_question|string||false|验证问题|
|⇥ avatar|string||false|头像|
|⇥ description|string||false|描述信息|
|⇥ ext|string||false||
|⇥ mute_notification|boolean||false||
|⇥ nick_name|string||false|昵称或名称|
|⇥ public_info|string||false|公开信息，好友和陌生人可见|
|⇥ relation|int32||false||
|⇥ user_id|int32||false|好友用户ID|
|⇥ username|string||false|用户名|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.18	是否允许发消息

> GET  /roster/may_message
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|roster_id||roster_id|
|user_id||user_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.19	用手机号搜索用户

> GET  /roster/mobile
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|mobile||mobile|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|好友列表|
|⇥ alias|string||false||
|⇥ auth_mode|int32||false|验证方式, 0 - 无需验证，任何人可以加为好友, 1 - 需要同意方可加为好友, 2 - 需要回答问题正确方可加为好友, 3 - 拒绝所有加好友申请|
|⇥ auth_question|string||false|验证问题|
|⇥ avatar|string||false|头像|
|⇥ description|string||false|描述信息|
|⇥ ext|string||false||
|⇥ mute_notification|boolean||false||
|⇥ nick_name|string||false|昵称或名称|
|⇥ public_info|string||false|公开信息，好友和陌生人可见|
|⇥ relation|int32||false||
|⇥ user_id|int32||false|好友用户ID|
|⇥ username|string||false|用户名|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.20	用用户名搜索用户

> GET  /roster/name
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|username||username|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false|好友列表|
|⇥ alias|string||false||
|⇥ auth_mode|int32||false|验证方式, 0 - 无需验证，任何人可以加为好友, 1 - 需要同意方可加为好友, 2 - 需要回答问题正确方可加为好友, 3 - 拒绝所有加好友申请|
|⇥ auth_question|string||false|验证问题|
|⇥ avatar|string||false|头像|
|⇥ description|string||false|描述信息|
|⇥ ext|string||false||
|⇥ mute_notification|boolean||false||
|⇥ nick_name|string||false|昵称或名称|
|⇥ public_info|string||false|公开信息，好友和陌生人可见|
|⇥ relation|int32||false||
|⇥ user_id|int32||false|好友用户ID|
|⇥ username|string||false|用户名|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.21	从黑名单移除

> POST  /roster/unblock
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|user_id||user_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 8.22	从黑名单移除

> DELETE  /roster/unblock
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|user_id||user_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|boolean||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 9	文件操作接口

## 9.1	下载头像

> GET  /file/download/avatar
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|image_type||图片类型，1: 原图，2: 缩略图, 3: 封面图|
|object_name||对象名|
|sdk_sign||SDK的签名|
|store_token||文件token|
|thumbnail_strategy||缩略图生成策略, 1 - 第三方服务器生成， 2 - 本地服务器生成，默认值是 1|
### 响应体
● 200 响应数据格式：JSON

##### 接口描述
> 




## 9.2	下载聊天文件

> GET  /file/download/chat
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|file_sign||文件签名|
|format||需要下载的音频文件格式amr/mp3 默认为amr|
|image_type||图片类型，1: 原图，2: 缩略图, 3: 封面图|
|sdk_sign||SDK的签名|
|source||请求来源, miniprogram - 小程序，默认值是 ''|
|store_token||文件token|
|thumbnail_strategy||缩略图生成策略, 1 - 第三方服务器生成， 2 - 本地服务器生成，默认值是 1|
### 响应体
● 200 响应数据格式：JSON

##### 接口描述
> 




## 9.3	获取上传群头像URL

> GET  /file/upload/avatar/group
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|group_id||group_id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false||
|⇥ download_url|string||false||
|⇥ oss_body_param|object||false||
|⇥ upload_url|string||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 9.4	获取上传用户头像URL

> GET  /file/upload/avatar/user
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false||
|⇥ download_url|string||false||
|⇥ oss_body_param|object||false||
|⇥ upload_url|string||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 9.5	获取上传聊天文件的URL

> GET  /file/upload/chat
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|file_type||文件类型 100: 普通聊天文件, 101: 语音聊天文件(amr格式),102: 图片聊天文件, 103: 视频聊天文件, 104: 语音聊天文件(mp3格式)200: 普通共享文件, 201: 语音共享文件, 202: 图片共享文件, 203: 视频共享文件|
|to_id||to_id|
|to_type||1: 用户，2: 群组|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|object||false||
|⇥ download_url|string||false||
|⇥ oss_body_param|object||false||
|⇥ upload_url|string||false||
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 




## 9.6	获取聊天文件转发的URL

> GET  /file/upload/forward
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|access-token||令牌||app_id||应用ID||group_id||仅当access-token为管理员token时，可以设置此字段，表示以此群ID的管理员身份来调用此接口||user_id||仅当access-token为管理员token时，可以设置此字段，表示以此用户ID的身份来调用此接口|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|file_sign||文件签名|
|to_id||to_id|
|to_type||1: 用户，2: 群组|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false|返回码，200是成功|
| data|string||false|结果数据|
| message|string||false|错误信息，如果成功，该项为null|

##### 接口描述
> 



