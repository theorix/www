# floo::BMXPushService

## Public Types

|            | Name                                                                                          |
| ---------- | --------------------------------------------------------------------------------------------- |
| enum class | <p><strong>PushSdkStatus</strong> { Starting = 1, Started, Stoped, Offline}<br>push sdk状态</p> |
| enum class | <p><strong>PushDirection</strong> { Up, Down}<br>本地推送消息搜索方向</p>                               |

## Public Functions

|                             | Name                                                                                                                                                                                                          |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| virtual                     | **\~BMXPushService**()                                                                                                                                                                                        |
| virtual BMXErrorCode        | <p><strong>start</strong>(const std::string &#x26; alias ="", const std::string &#x26; bmxToken ="") =0<br>初始化推送sdk。在仅使用推送的情况下使用该接口初始化推送sdk。在同时使用IM功能的时候直接在BMXClient调用登陆功能即可。config对象初始化的时候需要传入平台类型和设备id。</p> |
| virtual BMXErrorCode        | <p><strong>stop</strong>() =0<br>停止推送功能接口。</p>                                                                                                                                                                |
| virtual BMXErrorCode        | <p><strong>resume</strong>() =0<br>恢复推送功能接口。</p>                                                                                                                                                              |
| virtual BMXErrorCode        | <p><strong>unbindAlias</strong>(const std::string &#x26; alias) =0<br>解除用户别名绑定。</p>                                                                                                                           |
| virtual const std::string & | <p><strong>getToken</strong>() =0<br>获取登陆后使用的用户token。</p>                                                                                                                                                     |
| virtual const std::string & | <p><strong>getCert</strong>() =0<br>获取登陆后服务器返回的推送证书。</p>                                                                                                                                                      |
| virtual PushSdkStatus       | <p><strong>status</strong>() =0<br>推送sdk当前的状态。</p>                                                                                                                                                            |
| virtual BMXErrorCode        | <p><strong>bindDeviceToken</strong>(const std::string &#x26; token) =0<br>推送绑定设备token。</p>                                                                                                                    |
| virtual BMXErrorCode        | <p><strong>bindVoipToken</strong>(const std::string &#x26; token) =0<br>绑定推送设备的voiptoken。</p>                                                                                                                 |
| virtual BMXErrorCode        | <p><strong>getPushProfile</strong>(BMXPushUserProfilePtr &#x26; pushProfile, bool forceRefresh) =0<br>获取推送用户详情，如果forceRefresh == true，则强制从服务端拉取</p>                                                           |
| virtual BMXErrorCode        | <p><strong>setTags</strong>(const std::vector&#x3C; std::string > &#x26; tags, const std::string &#x26; operationId) =0<br>设置推送用户的标签。</p>                                                                     |
| virtual BMXErrorCode        | <p><strong>getTags</strong>(std::vector&#x3C; std::string > &#x26; tags, const std::string &#x26; operationId) =0<br>获取推送用户的标签。</p>                                                                           |
| virtual BMXErrorCode        | <p><strong>deleteTags</strong>(const std::vector&#x3C; std::string > &#x26; tags, const std::string &#x26; operationId) =0<br>删除推送用户的标签。</p>                                                                  |
| virtual BMXErrorCode        | <p><strong>clearTags</strong>(const std::string &#x26; operationId) =0<br>清空推送用户的标签。</p>                                                                                                                      |
| virtual BMXErrorCode        | <p><strong>setBadge</strong>(int count) =0<br>设置推送用户的未读角标。</p>                                                                                                                                                |
| virtual BMXErrorCode        | <p><strong>setPushMode</strong>(bool enable =true) =0<br>设置推送启用状态。默认为使用推送。</p>                                                                                                                                |
| virtual BMXErrorCode        | <p><strong>setPushTime</strong>(int startHour, int endHour) =0<br>设置允许推送时间。</p>                                                                                                                               |
| virtual BMXErrorCode        | <p><strong>setSilenceTime</strong>(int startHour, int endHour) =0<br>设置推送静默的起始结束时间。</p>                                                                                                                       |
| virtual BMXErrorCode        | <p><strong>setRunBackgroundMode</strong>(bool enable =false) =0<br>设置推送是否可以后台运行。默认是false。</p>                                                                                                                 |
| virtual BMXErrorCode        | <p><strong>setGeoFenceMode</strong>(bool enable =false, bool isAllow =false) =0<br>设置推送的地理围栏功能是否运行。</p>                                                                                                       |
| virtual void                | <p><strong>clearNotification</strong>(int64_t notificationId) =0<br>清除指定id的通知。</p>                                                                                                                            |
| virtual void                | <p><strong>clearAllNotifications</strong>() =0<br>清空下拉通知栏全部通知。</p>                                                                                                                                            |
| virtual void                | <p><strong>sendMessage</strong>(const std::string &#x26; content) =0<br>发送推送上行消息，消息状态变化会通过listener通知</p>                                                                                                      |
| virtual BMXErrorCode        | <p><strong>loadLocalPushMessages</strong>(int64_t refMsgId, size_t size, BMXMessageList &#x26; result, PushDirection =PushDirection::Up) =0<br>加载数据库本地存储的推送消息。如果不指定则从最新消息开始</p>                               |
| virtual void                | <p><strong>addPushListener</strong>(BMXPushServiceListener * listener) =0<br>添加推送监听者</p>                                                                                                                      |
| virtual void                | <p><strong>removePushListener</strong>(BMXPushServiceListener * listener) =0<br>移除推送监听者</p>                                                                                                                   |

## Public Types Documentation

### enum PushSdkStatus

| Enumerator | Value | Description |
| ---------- | ----- | ----------- |
| Starting   | 1     | 正在启动        |
| Started    |       | 启动，在线       |
| Stoped     |       | 停止          |
| Offline    |       | 离线          |

push sdk状态

### enum PushDirection

| Enumerator | Value | Description |
| ---------- | ----- | ----------- |
| Up         |       | 取更旧消息       |
| Down       |       | 取更新消息       |

本地推送消息搜索方向

## Public Functions Documentation

### function \~BMXPushService

```cpp
inline virtual ~BMXPushService()
```

### function start

```cpp
virtual BMXErrorCode start(
    const std::string & alias ="",
    const std::string & bmxToken =""
) =0
```

初始化推送sdk。在仅使用推送的情况下使用该接口初始化推送sdk。在同时使用IM功能的时候直接在BMXClient调用登陆功能即可。config对象初始化的时候需要传入平台类型和设备id。

**Parameters**:

* **alias** 推送初始化使用的当前用户别名
* **bmxToken** 推送初始化的时候App传入的使用的用户的token，无用户的状态下不传入即可。

**Return**: BMXErrorCode

### function stop

```cpp
virtual BMXErrorCode stop() =0
```

停止推送功能接口。

**Return**: BMXErrorCode

### function resume

```cpp
virtual BMXErrorCode resume() =0
```

恢复推送功能接口。

**Return**: BMXErrorCode

### function unbindAlias

```cpp
virtual BMXErrorCode unbindAlias(
    const std::string & alias
) =0
```

解除用户别名绑定。

**Parameters**:

* **alias** 需要解除绑定的用户别名。

**Return**: BMXErrorCode

### function getToken

```cpp
virtual const std::string & getToken() =0
```

获取登陆后使用的用户token。

**Return**: std::stirng

### function getCert

```cpp
virtual const std::string & getCert() =0
```

获取登陆后服务器返回的推送证书。

**Return**: std::stirng

### function status

```cpp
virtual PushSdkStatus status() =0
```

推送sdk当前的状态。

**Return**: PushSdkStatus

### function bindDeviceToken

```cpp
virtual BMXErrorCode bindDeviceToken(
    const std::string & token
) =0
```

推送绑定设备token。

**Parameters**:

* **token** 设备的推送token

**Return**: BMXErrorCode

### function bindVoipToken

```cpp
virtual BMXErrorCode bindVoipToken(
    const std::string & token
) =0
```

绑定推送设备的voiptoken。

**Parameters**:

* **token** 设备的voip推送token

**Return**: BMXErrorCode

### function getPushProfile

```cpp
virtual BMXErrorCode getPushProfile(
    BMXPushUserProfilePtr & pushProfile,
    bool forceRefresh
) =0
```

获取推送用户详情，如果forceRefresh == true，则强制从服务端拉取

**Parameters**:

* **profile** 推送用户profile信息，初始传入指向为空的shared\_ptr对象，函数返回后从此处获取用户profile信息。
* **forceRefresh** 是否强制从服务器拉取，本地获取失败的情况下会自动从服务器拉取

**Return**: BMXErrorCode

### function setTags

```cpp
virtual BMXErrorCode setTags(
    const std::vector< std::string > & tags,
    const std::string & operationId
) =0
```

设置推送用户的标签。

**Parameters**:

* **tags** 用户标签
* **operationId** 操作id。在回调通知中对应通知提醒。

**Return**: BMXErrorCode

### function getTags

```cpp
virtual BMXErrorCode getTags(
    std::vector< std::string > & tags,
    const std::string & operationId
) =0
```

获取推送用户的标签。

**Parameters**:

* **tags** 用户标签
* **operationId** 操作id。在回调通知中对应通知提醒。

**Return**: BMXErrorCode

### function deleteTags

```cpp
virtual BMXErrorCode deleteTags(
    const std::vector< std::string > & tags,
    const std::string & operationId
) =0
```

删除推送用户的标签。

**Parameters**:

* **tags** 要删除用户标签
* **operationId** 操作id。在回调通知中对应通知提醒。

**Return**: BMXErrorCode

### function clearTags

```cpp
virtual BMXErrorCode clearTags(
    const std::string & operationId
) =0
```

清空推送用户的标签。

**Parameters**:

* **operationId** 操作id。在回调通知中对应通知提醒。

**Return**: BMXErrorCode

### function setBadge

```cpp
virtual BMXErrorCode setBadge(
    int count
) =0
```

设置推送用户的未读角标。

**Parameters**:

* **count** 用户未读角标数

**Return**: BMXErrorCode

### function setPushMode

```cpp
virtual BMXErrorCode setPushMode(
    bool enable =true
) =0
```

设置推送启用状态。默认为使用推送。

**Parameters**:

* **enable** 推送的启用状态

**Return**: BMXErrorCode

### function setPushTime

```cpp
virtual BMXErrorCode setPushTime(
    int startHour,
    int endHour
) =0
```

设置允许推送时间。

**Parameters**:

* **startHour** 静默允许推送的起始时间小时
* **endHour** 静默允许推送的结束时间小时

**Return**: BMXErrorCode

### function setSilenceTime

```cpp
virtual BMXErrorCode setSilenceTime(
    int startHour,
    int endHour
) =0
```

设置推送静默的起始结束时间。

**Parameters**:

* **startHour** 静默推送的起始时间小时
* **endHour** 静默推送的结束时间小时

**Return**: BMXErrorCode

### function setRunBackgroundMode

```cpp
virtual BMXErrorCode setRunBackgroundMode(
    bool enable =false
) =0
```

设置推送是否可以后台运行。默认是false。

**Parameters**:

* **enable** 推送后台运行状态。

**Return**: BMXErrorCode

### function setGeoFenceMode

```cpp
virtual BMXErrorCode setGeoFenceMode(
    bool enable =false,
    bool isAllow =false
) =0
```

设置推送的地理围栏功能是否运行。

**Parameters**:

* **enable** 地理围栏功能是否运行。
* **isAllow** 用户是否主动弹出用户定位请求。

**Return**: BMXErrorCode

### function clearNotification

```cpp
virtual void clearNotification(
    int64_t notificationId
) =0
```

清除指定id的通知。

**Parameters**:

* **notificationId** 通知id

### function clearAllNotifications

```cpp
virtual void clearAllNotifications() =0
```

清空下拉通知栏全部通知。

### function sendMessage

```cpp
virtual void sendMessage(
    const std::string & content
) =0
```

发送推送上行消息，消息状态变化会通过listener通知

**Parameters**:

* **content** 发送的上行推送消息内容

### function loadLocalPushMessages

```cpp
virtual BMXErrorCode loadLocalPushMessages(
    int64_t refMsgId,
    size_t size,
    BMXMessageList & result,
    PushDirection  =PushDirection::Up
) =0
```

加载数据库本地存储的推送消息。如果不指定则从最新消息开始

**Parameters**:

* **refMsgId** 加载推送消息的起始id
* **size** 最大加载消息条数
* **result** 数据库返回的加载本地推送消息列表
* **Direction** 加载推送消息的方向，默认是加载更早的消息

### function addPushListener

```cpp
virtual void addPushListener(
    BMXPushServiceListener * listener
) =0
```

添加推送监听者

**Parameters**:

* **listener** 推送监听者

### function removePushListener

```cpp
virtual void removePushListener(
    BMXPushServiceListener * listener
) =0
```

移除推送监听者

**Parameters**:

* **listener** 推送监听者

***

Updated on 2022-01-26 at 17:20:40 +0800
