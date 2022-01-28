# Page 3



### 7 群接口

### 7.1 添加群管理员

> POST /group/admin/add

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求体(Request Body) |                |         |
| 参数名称                  | 数据类型           | 默认值     |
| ------                | ------         | ------  |
| group\_id             | int32          | false   |
| user\_list            | array\[int32]  | false   |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ reason              | string         | false   |
| ⇥ result              | string         | false   |
| ⇥ user\_id            | int32          | false   |
| message               | string         | false   |

**接口描述**

>

### 7.2 移除群管理员

> POST /group/admin/remove

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求体(Request Body) |                |         |
| 参数名称                  | 数据类型           | 默认值     |
| ------                | ------         | ------  |
| group\_id             | int32          | false   |
| user\_list            | array\[int32]  | false   |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ reason              | string         | false   |
| ⇥ result              | string         | false   |
| ⇥ user\_id            | int32          | false   |
| message               | string         | false   |

**接口描述**

>

### 7.3 移除群管理员

> DELETE /group/admin/remove

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求体(Request Body) |                |         |
| 参数名称                  | 数据类型           | 默认值     |
| ------                | ------         | ------  |
| group\_id             | int32          | false   |
| user\_list            | array\[int32]  | false   |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ reason              | string         | false   |
| ⇥ result              | string         | false   |
| ⇥ user\_id            | int32          | false   |
| message               | string         | false   |

**接口描述**

>

### 7.4 获取群管理员列表

> GET /group/admin\_list

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求参数(Query Param) |                |         |
| 参数名称                  | 默认值            | 描述      |
| ------                | ------         | ------  |
| group\_id             | group\_id      |         |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ display\_name       | string         | false   |
| ⇥ join\_time          | int32          | false   |
| ⇥ user\_id            | int32          | false   |
| message               | string         | false   |

**接口描述**

>

### 7.5 根据群id和公告id获取群公告详情

> GET /group/announcement

#### 请求头

| 参数名称                  | 默认值              | 描述      |
| --------------------- | ---------------- | ------- |
| access-token          | 令牌               | app\_id |
| ### 请求参数(Query Param) |                  |         |
| 参数名称                  | 默认值              | 描述      |
| ------                | ------           | ------  |
| announcement\_id      | announcement\_id |         |
| group\_id             | group\_id        |         |
| ### 响应体               |                  |         |
| ● 200 响应数据格式：JSON     |                  |         |
| 参数名称                  | 类型               | 默认值     |
| ------                | ------           | ------  |
| code                  | int32            | false   |
| data                  | object           | false   |
| ⇥ author              | int32            | false   |
| ⇥ content             | string           | false   |
| ⇥ created\_at         | int32            | false   |
| ⇥ group\_id           | int32            | false   |
| ⇥ id                  | int32            | false   |
| ⇥ title               | string           | false   |
| message               | string           | false   |

**接口描述**

>

### 7.6 删除公告

> POST /group/announcement/delete

#### 请求头

| 参数名称                  | 默认值              | 描述      |
| --------------------- | ---------------- | ------- |
| access-token          | 令牌               | app\_id |
| ### 请求参数(Query Param) |                  |         |
| 参数名称                  | 默认值              | 描述      |
| ------                | ------           | ------  |
| announcement\_id      | announcement\_id |         |
| group\_id             | group\_id        |         |
| ### 响应体               |                  |         |
| ● 200 响应数据格式：JSON     |                  |         |
| 参数名称                  | 类型               | 默认值     |
| ------                | ------           | ------  |
| code                  | int32            | false   |
| data                  | object           | false   |
| message               | string           | false   |

**接口描述**

>

### 7.7 删除公告

> DELETE /group/announcement/delete

#### 请求头

| 参数名称                  | 默认值              | 描述      |
| --------------------- | ---------------- | ------- |
| access-token          | 令牌               | app\_id |
| ### 请求参数(Query Param) |                  |         |
| 参数名称                  | 默认值              | 描述      |
| ------                | ------           | ------  |
| announcement\_id      | announcement\_id |         |
| group\_id             | group\_id        |         |
| ### 响应体               |                  |         |
| ● 200 响应数据格式：JSON     |                  |         |
| 参数名称                  | 类型               | 默认值     |
| ------                | ------           | ------  |
| code                  | int32            | false   |
| data                  | object           | false   |
| message               | string           | false   |

**接口描述**

>

### 7.8 编辑群公告

> POST /group/announcement/edit

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| content               | string | false   |
| group\_id             | int32  | false   |
| title                 | string | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| ⇥ author              | int32  | false   |
| ⇥ content             | string | false   |
| ⇥ created\_at         | int32  | false   |
| ⇥ group\_id           | int32  | false   |
| ⇥ id                  | int32  | false   |
| ⇥ title               | string | false   |
| message               | string | false   |

**接口描述**

>

### 7.9 获取最新一条群公告详情

> GET /group/announcement/last

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
| ⇥ author              | int32     | false   |
| ⇥ content             | string    | false   |
| ⇥ created\_at         | int32     | false   |
| ⇥ group\_id           | int32     | false   |
| ⇥ id                  | int32     | false   |
| ⇥ title               | string    | false   |
| message               | string    | false   |

**接口描述**

>

### 7.10 获取群公告列表

> GET /group/announcement/list

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求参数(Query Param) |                |         |
| 参数名称                  | 默认值            | 描述      |
| ------                | ------         | ------  |
| group\_id             | group\_id      |         |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ author              | int32          | false   |
| ⇥ content             | string         | false   |
| ⇥ created\_at         | int32          | false   |
| ⇥ group\_id           | int32          | false   |
| ⇥ id                  | int32          | false   |
| ⇥ title               | string         | false   |
| message               | string         | false   |

**接口描述**

>

### 7.11 获取群申请列表

> POST /group/application\_list

#### 请求头

| 参数名称                  | 默认值           | 描述      |
| --------------------- | ------------- | ------- |
| access-token          | 令牌            | app\_id |
| ### 请求参数(Query Param) |               |         |
| 参数名称                  | 默认值           | 描述      |
| ------                | ------        | ------  |
| cursor                | cursor        |         |
| limit                 | limit         |         |
| version               | version       |         |
| ### 请求体(Request Body) |               |         |
| 参数名称                  | 数据类型          | 默认值     |
| ------                | ------        | ------  |
| group\_list           | array\[int32] | false   |
| ### 响应体               |               |         |
| ● 200 响应数据格式：JSON     |               |         |
| 参数名称                  | 类型            | 默认值     |
| ------                | ------        | ------  |
| code                  | int32         | false   |
| cursor                | string        | false   |
| data                  | object        | false   |
| message               | string        | false   |
| total                 | int32         | false   |
| version               | int32         | false   |

**接口描述**

>

### 7.12 申请入群

> POST /group/apply

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| group\_id             | int32  | false   |
| reason                | string | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| ⇥ reason              | string | false   |
| ⇥ result              | string | false   |
| ⇥ user\_id            | int32  | false   |
| message               | string | false   |

**接口描述**

>

### 7.13 管理员处理入群申请

> POST /group/apply/handle

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求体(Request Body) |         |         |
| 参数名称                  | 数据类型    | 默认值     |
| ------                | ------  | ------  |
| approval              | boolean | false   |
| group\_id             | int32   | false   |
| user\_id              | int32   | false   |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| data                  | object  | false   |
| ⇥ reason              | string  | false   |
| ⇥ result              | string  | false   |
| ⇥ user\_id            | int32   | false   |
| message               | string  | false   |

**接口描述**

>

### 7.14 管理员处理入群申请

> PUT /group/apply/handle

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求体(Request Body) |         |         |
| 参数名称                  | 数据类型    | 默认值     |
| ------                | ------  | ------  |
| approval              | boolean | false   |
| group\_id             | int32   | false   |
| user\_id              | int32   | false   |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| data                  | object  | false   |
| ⇥ reason              | string  | false   |
| ⇥ result              | string  | false   |
| ⇥ user\_id            | int32   | false   |
| message               | string  | false   |

**接口描述**

>

### 7.15 将用户禁言

> POST /group/ban

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求体(Request Body) |                |         |
| 参数名称                  | 数据类型           | 默认值     |
| ------                | ------         | ------  |
| duration              | int32          | false   |
| group\_id             | int32          | false   |
| user\_list            | array\[int32]  | false   |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ reason              | string         | false   |
| ⇥ result              | string         | false   |
| ⇥ user\_id            | int32          | false   |
| message               | string         | false   |

**接口描述**

>

### 7.16 获取禁言列表

> GET /group/banned\_list

#### 请求头

| 参数名称                  | 默认值       | 描述      |
| --------------------- | --------- | ------- |
| access-token          | 令牌        | app\_id |
| ### 请求参数(Query Param) |           |         |
| 参数名称                  | 默认值       | 描述      |
| ------                | ------    | ------  |
| cursor                | cursor    |         |
| group\_id             | group\_id |         |
| limit                 | limit     |         |
| version               | version   |         |
| ### 响应体               |           |         |
| ● 200 响应数据格式：JSON     |           |         |
| 参数名称                  | 类型        | 默认值     |
| ------                | ------    | ------  |
| code                  | int32     | false   |
| cursor                | string    | false   |
| data                  | object    | false   |
| message               | string    | false   |
| total                 | int32     | false   |
| version               | int32     | false   |

**接口描述**

>

### 7.17 将用户加入黑名单

> POST /group/block

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求体(Request Body) |                |         |
| 参数名称                  | 数据类型           | 默认值     |
| ------                | ------         | ------  |
| group\_id             | int32          | false   |
| user\_list            | array\[int32]  | false   |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ reason              | string         | false   |
| ⇥ result              | string         | false   |
| ⇥ user\_id            | int32          | false   |
| message               | string         | false   |

**接口描述**

>

### 7.18 获取黑名单列表

> GET /group/blocked\_list

#### 请求头

| 参数名称                  | 默认值       | 描述      |
| --------------------- | --------- | ------- |
| access-token          | 令牌        | app\_id |
| ### 请求参数(Query Param) |           |         |
| 参数名称                  | 默认值       | 描述      |
| ------                | ------    | ------  |
| cursor                | cursor    |         |
| group\_id             | group\_id |         |
| limit                 | limit     |         |
| version               | version   |         |
| ### 响应体               |           |         |
| ● 200 响应数据格式：JSON     |           |         |
| 参数名称                  | 类型        | 默认值     |
| ------                | ------    | ------  |
| code                  | int32     | false   |
| cursor                | string    | false   |
| data                  | object    | false   |
| message               | string    | false   |
| total                 | int32     | false   |
| version               | int32     | false   |

**接口描述**

>

### 7.19 创建群

> POST /group/create

#### 请求头

| 参数名称                  | 默认值           | 描述      |
| --------------------- | ------------- | ------- |
| access-token          | 令牌            | app\_id |
| ### 请求体(Request Body) |               |         |
| 参数名称                  | 数据类型          | 默认值     |
| ------                | ------        | ------  |
| avatar                | string        | false   |
| description           | string        | false   |
| name                  | string        | false   |
| type                  | int32         | false   |
| user\_list            | array\[int32] | false   |
| ### 响应体               |               |         |
| ● 200 响应数据格式：JSON     |               |         |
| 参数名称                  | 类型            | 默认值     |
| ------                | ------        | ------  |
| code                  | int32         | false   |
| data                  | object        | false   |
| message               | string        | false   |

**接口描述**

>

### 7.20 解散群

> POST /group/destroy

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
| data                  | boolean   | false   |
| message               | string    | false   |

**接口描述**

>

### 7.21 解散群

> DELETE /group/destroy

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
| data                  | boolean   | false   |
| message               | string    | false   |

**接口描述**

>

### 7.22 更新群名片

> POST /group/display\_name

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求体(Request Body) |         |         |
| 参数名称                  | 数据类型    | 默认值     |
| ------                | ------  | ------  |
| group\_id             | int32   | false   |
| value                 | string  | false   |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| data                  | boolean | false   |
| message               | string  | false   |

**接口描述**

>

### 7.23 更新群名片

> PUT /group/display\_name

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求体(Request Body) |         |         |
| 参数名称                  | 数据类型    | 默认值     |
| ------                | ------  | ------  |
| group\_id             | int32   | false   |
| value                 | string  | false   |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| data                  | boolean | false   |
| message               | string  | false   |

**接口描述**

>

### 7.24 下载群文件

> GET /group/file

#### 请求头

| 参数名称                  | 默认值       | 描述      |
| --------------------- | --------- | ------- |
| access-token          | 令牌        | app\_id |
| ### 请求参数(Query Param) |           |         |
| 参数名称                  | 默认值       | 描述      |
| ------                | ------    | ------  |
| file\_id              | file\_id  |         |
| group\_id             | group\_id |         |
| ### 响应体               |           |         |
| ● 200 响应数据格式：JSON     |           |         |
| 参数名称                  | 类型        | 默认值     |
| ------                | ------    | ------  |
| code                  | int32     | false   |
| data                  | object    | false   |
| ⇥ created\_at         | int32     | false   |
| ⇥ file\_id            | int32     | false   |
| ⇥ group\_id           | int32     | false   |
| ⇥ name                | string    | false   |
| ⇥ size                | int32     | false   |
| ⇥ type                | string    | false   |
| ⇥ updated\_at         | int32     | false   |
| ⇥ uploader            | int32     | false   |
| ⇥ url                 | string    | false   |
| message               | string    | false   |

**接口描述**

>

### 7.25 删除群文件

> POST /group/file/delete

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求体(Request Body) |                |         |
| 参数名称                  | 数据类型           | 默认值     |
| ------                | ------         | ------  |
| file\_list            | array\[int32]  | false   |
| group\_id             | int32          | false   |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ file\_id            | int32          | false   |
| ⇥ reason              | string         | false   |
| ⇥ result              | string         | false   |
| message               | string         | false   |

**接口描述**

>

### 7.26 删除群文件

> DELETE /group/file/delete

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求体(Request Body) |                |         |
| 参数名称                  | 数据类型           | 默认值     |
| ------                | ------         | ------  |
| file\_list            | array\[int32]  | false   |
| group\_id             | int32          | false   |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ file\_id            | int32          | false   |
| ⇥ reason              | string         | false   |
| ⇥ result              | string         | false   |
| message               | string         | false   |

**接口描述**

>

### 7.27 获取群文件列表

> GET /group/file/list

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求参数(Query Param) |                |         |
| 参数名称                  | 默认值            | 描述      |
| ------                | ------         | ------  |
| group\_id             | group\_id      |         |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ created\_at         | int32          | false   |
| ⇥ file\_id            | int32          | false   |
| ⇥ group\_id           | int32          | false   |
| ⇥ name                | string         | false   |
| ⇥ size                | int32          | false   |
| ⇥ type                | string         | false   |
| ⇥ updated\_at         | int32          | false   |
| ⇥ uploader            | int32          | false   |
| ⇥ url                 | string         | false   |
| message               | string         | false   |

**接口描述**

>

### 7.28 更新群文件名称

> POST /group/file/update\_name

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| file\_id              | int32  | false   |
| group\_id             | int32  | false   |
| name                  | string | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| message               | string | false   |

**接口描述**

>

### 7.29 更新群文件名称

> PUT /group/file/update\_name

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| file\_id              | int32  | false   |
| group\_id             | int32  | false   |
| name                  | string | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| message               | string | false   |

**接口描述**

>

### 7.30 上传群文件

> POST /group/file/upload

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| group\_id             | int32  | false   |
| name                  | string | false   |
| size                  | int32  | false   |
| type                  | string | false   |
| url                   | string | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| ⇥ created\_at         | int32  | false   |
| ⇥ file\_id            | int32  | false   |
| ⇥ group\_id           | int32  | false   |
| ⇥ name                | string | false   |
| ⇥ size                | int32  | false   |
| ⇥ type                | string | false   |
| ⇥ updated\_at         | int32  | false   |
| ⇥ uploader            | int32  | false   |
| ⇥ url                 | string | false   |
| message               | string | false   |

**接口描述**

>

### 7.31 根据group id获取群信息

> GET /group/info

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
| ⇥ apply\_approval     | int32     | false   |
| ⇥ avatar              | string    | false   |
| ⇥ ban\_expire\_time   | int32     | false   |
| ⇥ created\_at         | int32     | false   |
| ⇥ description         | string    | false   |
| ⇥ ext                 | string    | false   |
| ⇥ group\_id           | int32     | false   |
| ⇥ history\_visible    | boolean   | false   |
| ⇥ member\_invite      | boolean   | false   |
| ⇥ member\_modify      | boolean   | false   |
| ⇥ msg\_mute\_mode     | int32     | false   |
| ⇥ msg\_push\_mode     | int32     | false   |
| ⇥ name                | string    | false   |
| ⇥ owner\_id           | int32     | false   |
| ⇥ read\_ack           | boolean   | false   |
| ⇥ status              | int32     | false   |
| ⇥ type                | int32     | false   |
| ⇥ updated\_at         | int32     | false   |
| message               | string    | false   |

**接口描述**

>

### 7.32 更新群头像

> POST /group/info/avatar

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| group\_id             | int32  | false   |
| value                 | string | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| message               | string | false   |

**接口描述**

>

### 7.33 更新群头像

> PUT /group/info/avatar

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| group\_id             | int32  | false   |
| value                 | string | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| message               | string | false   |

**接口描述**

>

### 7.34 根据group id获取群信息

> POST /group/info/batch

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求体(Request Body) |                |         |
| 参数名称                  | 数据类型           | 默认值     |
| ------                | ------         | ------  |
| group\_list           | array\[int32]  | false   |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ apply\_approval     | int32          | false   |
| ⇥ avatar              | string         | false   |
| ⇥ capacity            | int32          | false   |
| ⇥ count               | int32          | false   |
| ⇥ group\_id           | int32          | false   |
| ⇥ msg\_mute\_mode     | int32          | false   |
| ⇥ msg\_push\_mode     | int32          | false   |
| ⇥ name                | string         | false   |
| ⇥ owner               | int32          | false   |
| ⇥ status              | int32          | false   |
| ⇥ type                | int32          | false   |
| message               | string         | false   |

**接口描述**

>

### 7.35 更新群描述

> POST /group/info/description

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| group\_id             | int32  | false   |
| value                 | string | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| message               | string | false   |

**接口描述**

>

### 7.36 更新群描述

> PUT /group/info/description

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| group\_id             | int32  | false   |
| value                 | string | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| message               | string | false   |

**接口描述**

>

### 7.37 更新扩展信息

> POST /group/info/ext

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| group\_id             | int32  | false   |
| value                 | string | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| message               | string | false   |

**接口描述**

>

### 7.38 更新扩展信息

> PUT /group/info/ext

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| group\_id             | int32  | false   |
| value                 | string | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| message               | string | false   |

**接口描述**

>

### 7.39 更新群名称

> POST /group/info/name

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| group\_id             | int32  | false   |
| value                 | string | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| message               | string | false   |

**接口描述**

>

### 7.40 更新群名称

> PUT /group/info/name

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| group\_id             | int32  | false   |
| value                 | string | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| message               | string | false   |

**接口描述**

>

### 7.41 获取群邀请列表

> GET /group/invitation\_list

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求参数(Query Param) |         |         |
| 参数名称                  | 默认值     | 描述      |
| ------                | ------  | ------  |
| cursor                | cursor  |         |
| limit                 | limit   |         |
| version               | version |         |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| cursor                | string  | false   |
| data                  | object  | false   |
| message               | string  | false   |
| total                 | int32   | false   |
| version               | int32   | false   |

**接口描述**

>

### 7.42 邀请入群

> POST /group/invite

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求体(Request Body) |                |         |
| 参数名称                  | 数据类型           | 默认值     |
| ------                | ------         | ------  |
| group\_id             | int32          | false   |
| reason                | string         | false   |
| user\_list            | array\[int32]  | false   |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ reason              | string         | false   |
| ⇥ result              | string         | false   |
| ⇥ user\_id            | int32          | false   |
| message               | string         | false   |

**接口描述**

>

### 7.43 用户处理入群邀请

> POST /group/invite/handle

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求体(Request Body) |         |         |
| 参数名称                  | 数据类型    | 默认值     |
| ------                | ------  | ------  |
| approval              | boolean | false   |
| group\_id             | int32   | false   |
| user\_id              | int32   | false   |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| data                  | object  | false   |
| message               | string  | false   |

**接口描述**

>

### 7.44 用户处理入群邀请

> PUT /group/invite/handle

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求体(Request Body) |         |         |
| 参数名称                  | 数据类型    | 默认值     |
| ------                | ------  | ------  |
| approval              | boolean | false   |
| group\_id             | int32   | false   |
| user\_id              | int32   | false   |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| data                  | object  | false   |
| message               | string  | false   |

**接口描述**

>

### 7.45 将成员踢出群

> POST /group/kick

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求体(Request Body) |                |         |
| 参数名称                  | 数据类型           | 默认值     |
| ------                | ------         | ------  |
| group\_id             | int32          | false   |
| user\_list            | array\[int32]  | false   |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ reason              | string         | false   |
| ⇥ result              | string         | false   |
| ⇥ user\_id            | int32          | false   |
| message               | string         | false   |

**接口描述**

>

### 7.46 将成员踢出群

> DELETE /group/kick

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求体(Request Body) |                |         |
| 参数名称                  | 数据类型           | 默认值     |
| ------                | ------         | ------  |
| group\_id             | int32          | false   |
| user\_list            | array\[int32]  | false   |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ reason              | string         | false   |
| ⇥ result              | string         | false   |
| ⇥ user\_id            | int32          | false   |
| message               | string         | false   |

**接口描述**

>

### 7.47 成员退出群

> POST /group/leave

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
| data                  | boolean   | false   |
| message               | string    | false   |

**接口描述**

>

### 7.48 成员退出群

> DELETE /group/leave

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
| data                  | boolean   | false   |
| message               | string    | false   |

**接口描述**

>

### 7.49 根据group id获取群成员列表

> GET /group/member\_list

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求参数(Query Param) |                |         |
| 参数名称                  | 默认值            | 描述      |
| ------                | ------         | ------  |
| cursor                | cursor         |         |
| group\_id             | group\_id      |         |
| limit                 | limit          |         |
| version               | version        |         |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| cursor                | string         | false   |
| data                  | array\[object] | false   |
| ⇥ display\_name       | string         | false   |
| ⇥ join\_time          | int32          | false   |
| ⇥ user\_id            | int32          | false   |
| message               | string         | false   |
| total                 | int32          | false   |
| version               | int32          | false   |

**接口描述**

>

### 7.50 批量获取群成员的群名片

> POST /group/members/display\_name

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求体(Request Body) |                |         |
| 参数名称                  | 数据类型           | 默认值     |
| ------                | ------         | ------  |
| group\_id             | int32          | false   |
| user\_list            | array\[int32]  | false   |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ display\_name       | string         | false   |
| ⇥ join\_time          | int32          | false   |
| ⇥ user\_id            | int32          | false   |
| message               | string         | false   |

**接口描述**

>

### 7.51 设置群消息屏蔽模式

> POST /group/msg/mute\_mode

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| group\_id             | int32  | false   |
| msg\_mute\_mode       | int32  | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| message               | string | false   |

**接口描述**

>

### 7.52 设置群消息屏蔽模式

> PUT /group/msg/mute\_mode

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| group\_id             | int32  | false   |
| msg\_mute\_mode       | int32  | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| message               | string | false   |

**接口描述**

>

### 7.53 设置群消息推送模式

> POST /group/msg/push\_mode

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| group\_id             | int32  | false   |
| msg\_push\_mode       | int32  | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| message               | string | false   |

**接口描述**

>

### 7.54 设置群消息推送模式

> PUT /group/msg/push\_mode

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| group\_id             | int32  | false   |
| msg\_push\_mode       | int32  | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| message               | string | false   |

**接口描述**

>

### 7.55 获取公开群列表

> GET /group/public\_list

#### 请求头

| 参数名称              | 默认值           | 描述      |
| ----------------- | ------------- | ------- |
| access-token      | 令牌            | app\_id |
| ### 响应体           |               |         |
| ● 200 响应数据格式：JSON |               |         |
| 参数名称              | 类型            | 默认值     |
| ------            | ------        | ------  |
| code              | int32         | false   |
| data              | array\[int32] | false   |
| message           | string        | false   |

**接口描述**

>

### 7.56 二维码邀请入群

> POST /group/qrcode/invite

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| qr\_info              | string | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| message               | string | false   |

**接口描述**

>

### 7.57 获取群邀请二维码信息

> GET /group/qrcode/sign

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
| ⇥ create\_at          | int32     | false   |
| ⇥ expire\_at          | int32     | false   |
| ⇥ qr\_info            | string    | false   |
| message               | string    | false   |

**接口描述**

>

### 7.58 获取群设置

> GET /group/settings

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
| ⇥ apply\_approval     | int32     | false   |
| ⇥ avatar              | string    | false   |
| ⇥ ban\_expire\_time   | int32     | false   |
| ⇥ created\_at         | int32     | false   |
| ⇥ description         | string    | false   |
| ⇥ ext                 | string    | false   |
| ⇥ group\_id           | int32     | false   |
| ⇥ history\_visible    | boolean   | false   |
| ⇥ member\_invite      | boolean   | false   |
| ⇥ member\_modify      | boolean   | false   |
| ⇥ msg\_mute\_mode     | int32     | false   |
| ⇥ msg\_push\_mode     | int32     | false   |
| ⇥ name                | string    | false   |
| ⇥ owner\_id           | int32     | false   |
| ⇥ read\_ack           | boolean   | false   |
| ⇥ status              | int32     | false   |
| ⇥ type                | int32     | false   |
| ⇥ updated\_at         | int32     | false   |
| message               | string    | false   |

**接口描述**

>

### 7.59 更新群设置--是否允许成员邀请

> POST /group/settings/allow\_member\_invitation

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求体(Request Body) |         |         |
| 参数名称                  | 数据类型    | 默认值     |
| ------                | ------  | ------  |
| group\_id             | int32   | false   |
| value                 | boolean | false   |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| data                  | boolean | false   |
| message               | string  | false   |

**接口描述**

>

### 7.60 更新群设置--是否允许成员邀请

> PUT /group/settings/allow\_member\_invitation

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求体(Request Body) |         |         |
| 参数名称                  | 数据类型    | 默认值     |
| ------                | ------  | ------  |
| group\_id             | int32   | false   |
| value                 | boolean | false   |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| data                  | boolean | false   |
| message               | string  | false   |

**接口描述**

>

### 7.61 更新群设置--群成员是否可修改群信息

> POST /group/settings/allow\_member\_modify

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求体(Request Body) |         |         |
| 参数名称                  | 数据类型    | 默认值     |
| ------                | ------  | ------  |
| group\_id             | int32   | false   |
| value                 | boolean | false   |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| data                  | boolean | false   |
| message               | string  | false   |

**接口描述**

>

### 7.62 更新群设置--群成员是否可修改群信息

> PUT /group/settings/allow\_member\_modify

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求体(Request Body) |         |         |
| 参数名称                  | 数据类型    | 默认值     |
| ------                | ------  | ------  |
| group\_id             | int32   | false   |
| value                 | boolean | false   |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| data                  | boolean | false   |
| message               | string  | false   |

**接口描述**

>

### 7.63 全员禁言，只允许管理员发消息

> POST /group/settings/ban\_all

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| duration              | int32  | false   |
| group\_id             | int32  | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| ⇥ ban\_expire\_time   | int32  | false   |
| message               | string | false   |

**接口描述**

>

### 7.64 更新群设置--是否开启群消息已读功能

> POST /group/settings/enable\_read\_ack

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求体(Request Body) |         |         |
| 参数名称                  | 数据类型    | 默认值     |
| ------                | ------  | ------  |
| group\_id             | int32   | false   |
| value                 | boolean | false   |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| data                  | boolean | false   |
| message               | string  | false   |

**接口描述**

>

### 7.65 更新群设置--是否开启群消息已读功能

> PUT /group/settings/enable\_read\_ack

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求体(Request Body) |         |         |
| 参数名称                  | 数据类型    | 默认值     |
| ------                | ------  | ------  |
| group\_id             | int32   | false   |
| value                 | boolean | false   |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| data                  | boolean | false   |
| message               | string  | false   |

**接口描述**

>

### 7.66 更新群设置--新成员是否可见群历史聊天记录

> POST /group/settings/history\_visible

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求体(Request Body) |         |         |
| 参数名称                  | 数据类型    | 默认值     |
| ------                | ------  | ------  |
| group\_id             | int32   | false   |
| value                 | boolean | false   |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| data                  | boolean | false   |
| message               | string  | false   |

**接口描述**

>

### 7.67 更新群设置--新成员是否可见群历史聊天记录

> PUT /group/settings/history\_visible

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求体(Request Body) |         |         |
| 参数名称                  | 数据类型    | 默认值     |
| ------                | ------  | ------  |
| group\_id             | int32   | false   |
| value                 | boolean | false   |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| data                  | boolean | false   |
| message               | string  | false   |

**接口描述**

>

### 7.68 更新群设置--群申请是否需要管理员审批

> POST /group/settings/require\_admin\_approval

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求体(Request Body) |         |         |
| 参数名称                  | 数据类型    | 默认值     |
| ------                | ------  | ------  |
| apply\_approval       | int32   | false   |
| group\_id             | int32   | false   |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| data                  | boolean | false   |
| message               | string  | false   |

**接口描述**

>

### 7.69 更新群设置--群申请是否需要管理员审批

> PUT /group/settings/require\_admin\_approval

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求体(Request Body) |         |         |
| 参数名称                  | 数据类型    | 默认值     |
| ------                | ------  | ------  |
| apply\_approval       | int32   | false   |
| group\_id             | int32   | false   |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| data                  | boolean | false   |
| message               | string  | false   |

**接口描述**

>

### 7.70 取消全员禁言

> POST /group/settings/unban\_all

#### 请求头

| 参数名称                  | 默认值     | 描述      |
| --------------------- | ------- | ------- |
| access-token          | 令牌      | app\_id |
| ### 请求体(Request Body) |         |         |
| 参数名称                  | 数据类型    | 默认值     |
| ------                | ------  | ------  |
| group\_id             | int32   | false   |
| ### 响应体               |         |         |
| ● 200 响应数据格式：JSON     |         |         |
| 参数名称                  | 类型      | 默认值     |
| ------                | ------  | ------  |
| code                  | int32   | false   |
| data                  | boolean | false   |
| message               | string  | false   |

**接口描述**

>

### 7.71 转让群

> POST /group/transfer

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| group\_id             | int32  | false   |
| new\_owner            | int32  | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| ⇥ reason              | string | false   |
| ⇥ result              | string | false   |
| ⇥ user\_id            | int32  | false   |
| message               | string | false   |

**接口描述**

>

### 7.72 转让群

> PUT /group/transfer

#### 请求头

| 参数名称                  | 默认值    | 描述      |
| --------------------- | ------ | ------- |
| access-token          | 令牌     | app\_id |
| ### 请求体(Request Body) |        |         |
| 参数名称                  | 数据类型   | 默认值     |
| ------                | ------ | ------  |
| group\_id             | int32  | false   |
| new\_owner            | int32  | false   |
| ### 响应体               |        |         |
| ● 200 响应数据格式：JSON     |        |         |
| 参数名称                  | 类型     | 默认值     |
| ------                | ------ | ------  |
| code                  | int32  | false   |
| data                  | object | false   |
| ⇥ reason              | string | false   |
| ⇥ result              | string | false   |
| ⇥ user\_id            | int32  | false   |
| message               | string | false   |

**接口描述**

>

### 7.73 从禁言列表移除用户

> POST /group/unban

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求体(Request Body) |                |         |
| 参数名称                  | 数据类型           | 默认值     |
| ------                | ------         | ------  |
| group\_id             | int32          | false   |
| user\_list            | array\[int32]  | false   |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ reason              | string         | false   |
| ⇥ result              | string         | false   |
| ⇥ user\_id            | int32          | false   |
| message               | string         | false   |

**接口描述**

>

### 7.74 从黑名单移除用户

> POST /group/unblock

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求体(Request Body) |                |         |
| 参数名称                  | 数据类型           | 默认值     |
| ------                | ------         | ------  |
| group\_id             | int32          | false   |
| user\_list            | array\[int32]  | false   |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ reason              | string         | false   |
| ⇥ result              | string         | false   |
| ⇥ user\_id            | int32          | false   |
| message               | string         | false   |

**接口描述**

>

### 7.75 从黑名单移除用户

> DELETE /group/unblock

#### 请求头

| 参数名称                  | 默认值            | 描述      |
| --------------------- | -------------- | ------- |
| access-token          | 令牌             | app\_id |
| ### 请求体(Request Body) |                |         |
| 参数名称                  | 数据类型           | 默认值     |
| ------                | ------         | ------  |
| group\_id             | int32          | false   |
| user\_list            | array\[int32]  | false   |
| ### 响应体               |                |         |
| ● 200 响应数据格式：JSON     |                |         |
| 参数名称                  | 类型             | 默认值     |
| ------                | ------         | ------  |
| code                  | int32          | false   |
| data                  | array\[object] | false   |
| ⇥ reason              | string         | false   |
| ⇥ result              | string         | false   |
| ⇥ user\_id            | int32          | false   |
| message               | string         | false   |

**接口描述**

>

### 7.76 获取用户的群组列表

> GET /group/user\_joined

#### 请求头

| 参数名称              | 默认值           | 描述      |
| ----------------- | ------------- | ------- |
| access-token      | 令牌            | app\_id |
| ### 响应体           |               |         |
| ● 200 响应数据格式：JSON |               |         |
| 参数名称              | 类型            | 默认值     |
| ------            | ------        | ------  |
| code              | int32         | false   |
| data              | array\[int32] | false   |
| message           | string        | false   |

**接口描述**

>
