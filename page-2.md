# Page 2



### 9 文件操作接口

### 9.1 下载头像

> GET /file/download/avatar

#### 请求头

| 参数名称                  | 默认值                                       | 描述      |
| --------------------- | ----------------------------------------- | ------- |
| access-token          | 令牌                                        | app\_id |
| ### 请求参数(Query Param) |                                           |         |
| 参数名称                  | 默认值                                       | 描述      |
| ------                | ------                                    | ------  |
| image\_type           | 图片类型，1: 原图，2: 缩略图, 3: 封面图                 |         |
| object\_name          | 对象名                                       |         |
| sdk\_sign             | SDK的签名                                    |         |
| store\_token          | 文件token                                   |         |
| thumbnail\_strategy   | 缩略图生成策略, 1 - 第三方服务器生成， 2 - 本地服务器生成，默认值是 1 |         |
| ### 响应体               |                                           |         |
| ● 200 响应数据格式：JSON     |                                           |         |

**接口描述**

>

### 9.2 下载聊天文件

> GET /file/download/chat

#### 请求头

| 参数名称                  | 默认值                                       | 描述      |
| --------------------- | ----------------------------------------- | ------- |
| access-token          | 令牌                                        | app\_id |
| ### 请求参数(Query Param) |                                           |         |
| 参数名称                  | 默认值                                       | 描述      |
| ------                | ------                                    | ------  |
| file\_sign            | 文件签名                                      |         |
| format                | 需要下载的音频文件格式amr/mp3 默认为amr                 |         |
| image\_type           | 图片类型，1: 原图，2: 缩略图, 3: 封面图                 |         |
| sdk\_sign             | SDK的签名                                    |         |
| source                | 请求来源, miniprogram - 小程序，默认值是 ''           |         |
| store\_token          | 文件token                                   |         |
| thumbnail\_strategy   | 缩略图生成策略, 1 - 第三方服务器生成， 2 - 本地服务器生成，默认值是 1 |         |
| ### 响应体               |                                           |         |
| ● 200 响应数据格式：JSON     |                                           |         |

**接口描述**

>

### 9.3 获取上传群头像URL

> GET /file/upload/avatar/group

#### 请求头

| 参数名称                  | 默认值       | 描述      |
| --------------------- | --------- | ------- |
| access-token          | 令牌        | app\_id |
| ### 请求参数(Query Param) |           |         |
| 参数名称                  | 默认值       | 描述      |
| ------                | ------    | ------  |
| group\_id             | group\_id |         |
| ### 响应体               |           |         |
| ● 200 响应数据格式：JSON     |           |         |
| 参数名称                  | 类型        | 默认值     |
| ------                | ------    | ------  |
| code                  | int32     | false   |
| data                  | object    | false   |
| ⇥ download\_url       | string    | false   |
| ⇥ oss\_body\_param    | object    | false   |
| ⇥ upload\_url         | string    | false   |
| message               | string    | false   |

**接口描述**

>

### 9.4 获取上传用户头像URL

> GET /file/upload/avatar/user

#### 请求头

| 参数名称               | 默认值    | 描述      |
| ------------------ | ------ | ------- |
| access-token       | 令牌     | app\_id |
| ### 响应体            |        |         |
| ● 200 响应数据格式：JSON  |        |         |
| 参数名称               | 类型     | 默认值     |
| ------             | ------ | ------  |
| code               | int32  | false   |
| data               | object | false   |
| ⇥ download\_url    | string | false   |
| ⇥ oss\_body\_param | object | false   |
| ⇥ upload\_url      | string | false   |
| message            | string | false   |

**接口描述**

>

### 9.5 获取上传聊天文件的URL

> GET /file/upload/chat

#### 请求头

| 参数名称                  | 默认值                                                                                                                                 | 描述      |
| --------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ------- |
| access-token          | 令牌                                                                                                                                  | app\_id |
| ### 请求参数(Query Param) |                                                                                                                                     |         |
| 参数名称                  | 默认值                                                                                                                                 | 描述      |
| ------                | ------                                                                                                                              | ------  |
| file\_type            | 文件类型 100: 普通聊天文件, 101: 语音聊天文件(amr格式),102: 图片聊天文件, 103: 视频聊天文件, 104: 语音聊天文件(mp3格式)200: 普通共享文件, 201: 语音共享文件, 202: 图片共享文件, 203: 视频共享文件 |         |
| to\_id                | to\_id                                                                                                                              |         |
| to\_type              | 1: 用户，2: 群组                                                                                                                         |         |
| ### 响应体               |                                                                                                                                     |         |
| ● 200 响应数据格式：JSON     |                                                                                                                                     |         |
| 参数名称                  | 类型                                                                                                                                  | 默认值     |
| ------                | ------                                                                                                                              | ------  |
| code                  | int32                                                                                                                               | false   |
| data                  | object                                                                                                                              | false   |
| ⇥ download\_url       | string                                                                                                                              | false   |
| ⇥ oss\_body\_param    | object                                                                                                                              | false   |
| ⇥ upload\_url         | string                                                                                                                              | false   |
| message               | string                                                                                                                              | false   |

**接口描述**

>

### 9.6 获取聊天文件转发的URL

> GET /file/upload/forward

#### 请求头

| 参数名称                  | 默认值         | 描述      |
| --------------------- | ----------- | ------- |
| access-token          | 令牌          | app\_id |
| ### 请求参数(Query Param) |             |         |
| 参数名称                  | 默认值         | 描述      |
| ------                | ------      | ------  |
| file\_sign            | 文件签名        |         |
| to\_id                | to\_id      |         |
| to\_type              | 1: 用户，2: 群组 |         |
| ### 响应体               |             |         |
| ● 200 响应数据格式：JSON     |             |         |
| 参数名称                  | 类型          | 默认值     |
| ------                | ------      | ------  |
| code                  | int32       | false   |
| data                  | string      | false   |
| message               | string      | false   |

**接口描述**

>
