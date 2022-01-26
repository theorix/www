# floo::BMXMessageConfig

消息配置

`#include <bmx_message_config.h>`

Inherits from BMXBaseObject

## Public Types

|            | Name                                                                       |
| ---------- | -------------------------------------------------------------------------- |
| enum class | <p><strong>BadgeCountType</strong> { Change, Set}<br>当前读取的Badge数字的操作类型</p> |

## Public Functions

|                         | Name                                                                                                                      |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| virtual                 | **\~BMXMessageConfig**()                                                                                                  |
| void                    | <p><strong>setMentionAll</strong>(bool mentionAll)<br>设置是否@全员</p>                                                         |
| bool                    | <p><strong>getMentionAll</strong>()<br>获取是否@全员</p>                                                                        |
| void                    | <p><strong>setMentionList</strong>(const std::vector&#x3C; int64_t > &#x26; mentionList)<br>设置通知成员id列表</p>                |
| std::vector< int64\_t > | <p><strong>getMentionList</strong>()<br>获取@成员列表</p>                                                                       |
| void                    | <p><strong>setMentionedMessage</strong>(const std::string &#x26; mentionedMessage)<br>设置@消息</p>                           |
| std::string             | <p><strong>getMentionedMessage</strong>()<br>获取@消息</p>                                                                    |
| void                    | <p><strong>setPushMessage</strong>(const std::string &#x26; pushMessage)<br>设置推送消息</p>                                    |
| std::string             | <p><strong>getPushMessage</strong>()<br>获取推送消息</p>                                                                        |
| void                    | <p><strong>setSenderNickname</strong>(const std::string &#x26; senderNickname)<br>设置发送者昵称</p>                             |
| std::string             | <p><strong>getSenderNickname</strong>()<br>获取发送者昵称</p>                                                                    |
| void                    | <p><strong>setGroupMemberList</strong>(const std::vector&#x3C; int64_t > &#x26; groupMemberList)<br>设置需要群已读消息的群成员id列表</p> |
| std::vector< int64\_t > | <p><strong>getGroupMemberList</strong>()<br>获取需要群已读消息的群成员id列表</p>                                                         |
| void                    | <p><strong>addGroupMember</strong>(int64_t id)<br>添加群已读消息的群成员id列表成员</p>                                                   |
| void                    | <p><strong>removeGroupMember</strong>(int64_t id)<br>清除需要群已读消息的群成员id列表成员</p>                                              |
| void                    | <p><strong>clearGroupMemberList</strong>()<br>清空群已读消息的群成员id列表</p>                                                         |
| void                    | <p><strong>setIOSConfig</strong>(const std::string &#x26; iosConfig)<br>设置IOS系统配置信息</p>                                   |
| std::string             | <p><strong>getIOSConfig</strong>()<br>获取IOS系统配置信息</p>                                                                     |
| void                    | <p><strong>setAndroidConfig</strong>(const std::string &#x26; androidConfig)<br>设置Android系统配置信息</p>                       |
| std::string             | <p><strong>getAndroidConfig</strong>()<br>获取Android系统配置信息</p>                                                             |
| void                    | <p><strong>setPushShowBeginTime</strong>(int beginTime)<br>设置推送显示开始时间</p>                                                 |
| int                     | <p><strong>getPushShowBeginTime</strong>()<br>获取推送显示开始时间</p>                                                              |
| void                    | <p><strong>setPushShowEndTime</strong>(int endTime)<br>设置推送显示结束时间</p>                                                     |
| int                     | <p><strong>getPushShowEndTime</strong>()<br>获取推送显示结束时间</p>                                                                |
| void                    | <p><strong>setPushTitle</strong>(const std::string &#x26; pushTitle)<br>设置推送标题</p>                                        |
| std::string             | <p><strong>getPushTitle</strong>()<br>获取推送标题</p>                                                                          |
| bool                    | <p><strong>isSilence</strong>()<br>获取当前的推送消息是否是静默消息</p>                                                                   |
| BadgeCountType          | <p><strong>getBadgeCountType</strong>()<br>获取当前的推送消息中badge计数</p>                                                          |
| int                     | <p><strong>getBadgeCount</strong>(int count)<br>获取当前的推送消息中badge计数</p>                                                     |
| void                    | <p><strong>setUsername</strong>(const std::string &#x26; username)<br>设置用户名</p>                                           |
| std::string             | <p><strong>getUsername</strong>()<br>获得用户名</p>                                                                            |
| std::string             | <p><strong>serialize</strong>() const<br>序列化操作</p>                                                                        |
| BMXMessageConfigPtr     | **createMessageConfig**(bool mentionAll)                                                                                  |

## Friends

|                     | Name                                                   |
| ------------------- | ------------------------------------------------------ |
| std::string         | **encodeBMXMessageConfig**(BMXMessageConfigPtr )       |
| BMXMessageConfigPtr | **decodeBMXMessageConfig**(const std::string & config) |

## Public Types Documentation

### enum BadgeCountType

| Enumerator | Value | Description                     |
| ---------- | ----- | ------------------------------- |
| Change     |       | 读取Badge计数的操作类型为增加或减少。正数为增加负数为减少 |
| Set        |       | 设置Badge的计数为当前的计数值               |

当前读取的Badge数字的操作类型

## Public Functions Documentation

### function \~BMXMessageConfig

```cpp
inline virtual ~BMXMessageConfig()
```

### function setMentionAll

```cpp
void setMentionAll(
    bool mentionAll
)
```

设置是否@全员

**Parameters**:

* **mentionAll**

### function getMentionAll

```cpp
bool getMentionAll()
```

获取是否@全员

**Return**: bool

### function setMentionList

```cpp
void setMentionList(
    const std::vector< int64_t > & mentionList
)
```

设置通知成员id列表

**Parameters**:

* **mentionList**

### function getMentionList

```cpp
std::vector< int64_t > getMentionList()
```

获取@成员列表

**Return**: std::vector\<int64\_t>

### function setMentionedMessage

```cpp
void setMentionedMessage(
    const std::string & mentionedMessage
)
```

设置@消息

**Parameters**:

* **mentionedMessage**

### function getMentionedMessage

```cpp
std::string getMentionedMessage()
```

获取@消息

**Return**: std::string

### function setPushMessage

```cpp
void setPushMessage(
    const std::string & pushMessage
)
```

设置推送消息

**Parameters**:

* **pushMessage**

### function getPushMessage

```cpp
std::string getPushMessage()
```

获取推送消息

**Return**: std::string

### function setSenderNickname

```cpp
void setSenderNickname(
    const std::string & senderNickname
)
```

设置发送者昵称

**Parameters**:

* **senderNickname**

### function getSenderNickname

```cpp
std::string getSenderNickname()
```

获取发送者昵称

**Return**: std::string

### function setGroupMemberList

```cpp
void setGroupMemberList(
    const std::vector< int64_t > & groupMemberList
)
```

设置需要群已读消息的群成员id列表

**Parameters**:

* **groupMemberList**

### function getGroupMemberList

```cpp
std::vector< int64_t > getGroupMemberList()
```

获取需要群已读消息的群成员id列表

**Return**: std::vector\<int64\_t>

### function addGroupMember

```cpp
void addGroupMember(
    int64_t id
)
```

添加群已读消息的群成员id列表成员

### function removeGroupMember

```cpp
void removeGroupMember(
    int64_t id
)
```

清除需要群已读消息的群成员id列表成员

**Return**: std::vector\<int64\_t>

### function clearGroupMemberList

```cpp
void clearGroupMemberList()
```

清空群已读消息的群成员id列表

### function setIOSConfig

```cpp
void setIOSConfig(
    const std::string & iosConfig
)
```

设置IOS系统配置信息

**Parameters**:

* **iosConfig**

### function getIOSConfig

```cpp
std::string getIOSConfig()
```

获取IOS系统配置信息

**Return**: std::string

### function setAndroidConfig

```cpp
void setAndroidConfig(
    const std::string & androidConfig
)
```

设置Android系统配置信息

**Parameters**:

* **androidConfig**

### function getAndroidConfig

```cpp
std::string getAndroidConfig()
```

获取Android系统配置信息

**Return**: std::string

### function setPushShowBeginTime

```cpp
void setPushShowBeginTime(
    int beginTime
)
```

设置推送显示开始时间

**Parameters**:

* **beginTime**

### function getPushShowBeginTime

```cpp
int getPushShowBeginTime()
```

获取推送显示开始时间

**Return**: int

### function setPushShowEndTime

```cpp
void setPushShowEndTime(
    int endTime
)
```

设置推送显示结束时间

**Parameters**:

* **endTime**

### function getPushShowEndTime

```cpp
int getPushShowEndTime()
```

获取推送显示结束时间

**Return**: int

### function setPushTitle

```cpp
void setPushTitle(
    const std::string & pushTitle
)
```

设置推送标题

**Parameters**:

* **pushTitle**

### function getPushTitle

```cpp
std::string getPushTitle()
```

获取推送标题

**Return**: std::string

### function isSilence

```cpp
bool isSilence()
```

获取当前的推送消息是否是静默消息

**Return**: bool

### function getBadgeCountType

```cpp
BadgeCountType getBadgeCountType()
```

获取当前的推送消息中badge计数

**Return**: BadgeCountType

### function getBadgeCount

```cpp
int getBadgeCount(
    int count
)
```

获取当前的推送消息中badge计数

**Return**: int

### function setUsername

```cpp
void setUsername(
    const std::string & username
)
```

设置用户名

**Parameters**:

* **username**

### function getUsername

```cpp
std::string getUsername()
```

获得用户名

**Return**: std::string

### function serialize

```cpp
std::string serialize() const
```

序列化操作

**Return**: std::string

### function createMessageConfig

```cpp
static BMXMessageConfigPtr createMessageConfig(
    bool mentionAll
)
```

## Friends

### friend encodeBMXMessageConfig

```cpp
friend std::string encodeBMXMessageConfig(
    BMXMessageConfigPtr 
);
```

### friend decodeBMXMessageConfig

```cpp
friend BMXMessageConfigPtr decodeBMXMessageConfig(
    const std::string & config
);
```

***

Updated on 2022-01-26 at 17:20:40 +0800
