# floo::BMXMessage

消息

`#include <bmx_message.h>`

Inherits from BMXBaseObject

## Public Types

|            | Name                                                                                                         |
| ---------- | ------------------------------------------------------------------------------------------------------------ |
| enum class | <p><strong>DeliveryStatus</strong> { New, Delivering, Deliveried, Failed, Recalled}<br>消息投递状态</p>            |
| enum class | <p><strong>MessageType</strong> { Single, Group, System}<br>消息类型</p>                                         |
| enum class | <p><strong>ContentType</strong> { Text, Image, Voice, Video, File, Location, Command, Forward}<br>消息内容类型</p> |
| enum class | <p><strong>DeliveryQos</strong> { AtLastOnce, AtMostOnce, ExactlyOnce}<br>消息投递质量</p>                         |

## Public Functions

|                         | Name                                                                                                                                                                                                                                        |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| virtual                 | <p><strong>~BMXMessage</strong>()<br>析构函数</p>                                                                                                                                                                                               |
| int64\_t                | <p><strong>msgId</strong>()<br>消息唯一ID</p>                                                                                                                                                                                                   |
| int64\_t                | <p><strong>clientMsgId</strong>()<br>消息客户端ID,仅在消息发送端存在</p>                                                                                                                                                                                  |
| int64\_t                | <p><strong>fromId</strong>()<br>消息发送方ID</p>                                                                                                                                                                                                 |
| int64\_t                | <p><strong>toId</strong>()<br>消息接收方ID</p>                                                                                                                                                                                                   |
| MessageType             | <p><strong>type</strong>()<br>消息类型</p>                                                                                                                                                                                                      |
| int64\_t                | <p><strong>conversationId</strong>()<br>消息所属会话ID</p>                                                                                                                                                                                        |
| DeliveryStatus          | <p><strong>deliveryStatus</strong>()<br>消息投递状态</p>                                                                                                                                                                                          |
| void                    | <p><strong>setDeliveryStatus</strong>(DeliveryStatus )<br>设置消息投递状态</p>                                                                                                                                                                      |
| int64\_t                | <p><strong>serverTimestamp</strong>()<br>消息时间戳（服务端收到时的时间）</p>                                                                                                                                                                               |
| void                    | <p><strong>setServerTimestamp</strong>(int64_t )<br>设置时间戳（服务端收到时的时间）</p>                                                                                                                                                                    |
| int64\_t                | <p><strong>clientTimestamp</strong>()<br>本地时间戳（消息创建或者收到时的本地时间）</p>                                                                                                                                                                          |
| void                    | <p><strong>setClientTimestamp</strong>(int64_t )<br>设置消息本地时间戳</p>                                                                                                                                                                           |
| bool                    | <p><strong>isPlayed</strong>()<br>语音或者视频消息是否播放过，仅对收到的音视频消息有效</p>                                                                                                                                                                            |
| void                    | <p><strong>setIsPlayed</strong>(bool )<br>设置语音或者视频消息是否播放过，仅对收到的音视频消息有效</p>                                                                                                                                                                  |
| bool                    | <p><strong>isPlayAcked</strong>()<br>对于发送方表示是否收到了已播放回执，对于接收方表示是否发送了已播放回执</p>                                                                                                                                                                |
| void                    | <p><strong>setIsPlayAcked</strong>(bool )<br>设置已播放回执</p>                                                                                                                                                                                    |
| bool                    | <p><strong>isReceiveMsg</strong>()<br>是否接收的消息</p>                                                                                                                                                                                           |
| void                    | <p><strong>setIsReceiveMsg</strong>(bool )<br>设置是否接收的消息</p>                                                                                                                                                                                 |
| bool                    | <p><strong>isRead</strong>()<br>消息是否已读标志</p>                                                                                                                                                                                                |
| void                    | <p><strong>setIsRead</strong>(bool )<br>消息是否已读标志</p>                                                                                                                                                                                        |
| bool                    | <p><strong>isReadAcked</strong>()<br>对于发送方表示是否收到了已读回执，对于接收方表示是否发送了已读回执</p>                                                                                                                                                                  |
| void                    | <p><strong>setIsReadAcked</strong>(bool )<br>设置已读回执</p>                                                                                                                                                                                     |
| bool                    | <p><strong>isDeliveryAcked</strong>()<br>对于发送方表示消息是否已投递到对方，对于接收方表示是否发送了消息已到达回执</p>                                                                                                                                                          |
| void                    | <p><strong>setIsDeliveryAcked</strong>(bool )<br>设置投递回执</p>                                                                                                                                                                                 |
| const std::string &     | <p><strong>content</strong>()<br>消息文本内容</p>                                                                                                                                                                                                 |
| void                    | <p><strong>setContent</strong>(const std::string &#x26; content)<br>消息文本内容</p>                                                                                                                                                              |
| ContentType             | <p><strong>contentType</strong>()<br>消息内容类型，如果带附件就表示附件类型，不带附件就是文本类型</p>                                                                                                                                                                     |
| BMXMessageAttachmentPtr | <p><strong>attachment</strong>()<br>消息附件，BMXMessage拥有附件的所有权，负责释放</p>                                                                                                                                                                        |
| BMXMessageConfigPtr     | <p><strong>config</strong>()<br>消息的配置信息</p>                                                                                                                                                                                                 |
| void                    | <p><strong>setConfig</strong>(BMXMessageConfigPtr )<br>设置消息配置信息</p>                                                                                                                                                                         |
| const JSON &            | <p><strong>extension</strong>()<br>消息扩展信息</p>                                                                                                                                                                                               |
| void                    | <p><strong>setExtension</strong>(const JSON &#x26; )<br>设置消息扩展信息</p>                                                                                                                                                                        |
| DeliveryQos             | <p><strong>deliveryQos</strong>()<br>消息投递QOS</p>                                                                                                                                                                                            |
| void                    | <p><strong>setDeliveryQos</strong>(DeliveryQos qos)<br>设置消息投递QOS</p>                                                                                                                                                                        |
| const std::string &     | <p><strong>senderName</strong>()<br>消息发送者的显示名称</p>                                                                                                                                                                                          |
| void                    | <p><strong>setSenderName</strong>(const std::string &#x26; senderName)<br>设置消息的发送者显示名称</p>                                                                                                                                                  |
| int                     | <p><strong>groupAckCount</strong>()<br>群消息已读AckCount数目</p>                                                                                                                                                                                  |
| void                    | <p><strong>setGroupAckCount</strong>(int count)<br>设置消息已读groupAckCount数目(SDK 内部调用接口，上层不应该调用)</p>                                                                                                                                            |
| int                     | <p><strong>groupAckUnreadCount</strong>()<br>群消息未读AckCount数目</p>                                                                                                                                                                            |
| void                    | <p><strong>setGroupAckUnreadCount</strong>(int count)<br>设置消息未读groupAckCount数目(SDK 内部调用接口，上层不应该调用)</p>                                                                                                                                      |
| bool                    | <p><strong>groupAckReadAll</strong>()<br>群消息是否全部已读</p>                                                                                                                                                                                      |
| int                     | <p><strong>groupPlayAckCount</strong>()<br>群消息已播放AckCount数目（仅用于音频/视频附件消息）</p>                                                                                                                                                               |
| void                    | <p><strong>setGroupPlayAckCount</strong>(int count)<br>设置消息已播放groupAckCount数目(SDK 内部调用接口，上层不应该调用)（仅用于音频/视频附件消息）</p>                                                                                                                         |
| int                     | <p><strong>groupPlayAckUnreadCount</strong>()<br>群消息未播放AckCount数目（仅用于音频/视频附件消息）</p>                                                                                                                                                         |
| void                    | <p><strong>setGroupPlayAckUnreadCount</strong>(int count)<br>设置消息未播放groupAckCount数目(SDK 内部调用接口，上层不应该调用)（仅用于音频/视频附件消息）</p>                                                                                                                   |
| bool                    | <p><strong>groupPlayAckReadAll</strong>()<br>群消息是否全部已播放</p>                                                                                                                                                                                 |
| void                    | <p><strong>setPriority</strong>(int priority)<br>设置消息的扩散优先级，默认为0。0表示扩散，数字越小扩散的越多。</p>                                                                                                                                                       |
| int                     | <p><strong>priority</strong>()<br>消息的扩散优先级</p>                                                                                                                                                                                              |
| void                    | <p><strong>setPushMessageMode</strong>(bool )<br>设置消息是否为推送消息。</p>                                                                                                                                                                           |
| bool                    | <p><strong>isPushMessage</strong>()<br>消息是否是推送消息</p>                                                                                                                                                                                        |
| BMXMessagePtr           | <p><strong>createMessage</strong>(int64_t from, int64_t to, MessageType type, int64_t conversationId, const std::string &#x26; content)<br>创建发送文本消息</p>                                                                                     |
| BMXMessagePtr           | <p><strong>createMessage</strong>(int64_t from, int64_t to, MessageType type, int64_t conversationId, BMXMessageAttachmentPtr attachment)<br>创建发送附件消息</p>                                                                                   |
| BMXMessagePtr           | <p><strong>createCommandMessage</strong>(int64_t from, int64_t to, MessageType type, int64_t conversationId, const std::string &#x26; content)<br>创建发送命令消息(命令消息通过content字段或者extension字段存放命令信息)</p>                                          |
| BMXMessagePtr           | <p><strong>createMessage</strong>(int64_t msgId, int64_t from, int64_t to, MessageType type, int64_t conversationId, const std::string &#x26; content, int64_t serverTimestamp)<br>创建收到的消息</p>                                              |
| BMXMessagePtr           | <p><strong>createMessage</strong>(int64_t msgId, int64_t from, int64_t to, MessageType type, int64_t conversationId, BMXMessageAttachmentPtr attachment, int64_t serverTimestamp)<br>创建收到的消息</p>                                            |
| BMXMessagePtr           | <p><strong>createCommandMessage</strong>(int64_t msgId, int64_t from, int64_t to, MessageType type, int64_t conversationId, const std::string &#x26; content, int64_t serverTimestamp)<br>创建收到的命令消息(命令消息通过content字段或者extension字段存放命令信息)</p> |
| BMXMessagePtr           | <p><strong>createForwardMessage</strong>(BMXMessagePtr msg, int64_t from, int64_t to, MessageType type, int64_t conversationId)<br>创建转发消息</p>                                                                                               |

## Public Types Documentation

### enum DeliveryStatus

| Enumerator | Value | Description |
| ---------- | ----- | ----------- |
| New        |       | 新创建消息       |
| Delivering |       | 消息投递中       |
| Deliveried |       | 消息已投递       |
| Failed     |       | 消息投递失败      |
| Recalled   |       | 消息已撤回       |

消息投递状态

### enum MessageType

| Enumerator | Value | Description |
| ---------- | ----- | ----------- |
| Single     |       | 单聊消息        |
| Group      |       | 群聊消息        |
| System     |       | 系统消息        |

消息类型

### enum ContentType

| Enumerator | Value | Description |
| ---------- | ----- | ----------- |
| Text       |       | 文本消息        |
| Image      |       | 图片消息        |
| Voice      |       | 语音消息        |
| Video      |       | 视频片段消息      |
| File       |       | 文件消息        |
| Location   |       | 位置消息        |
| Command    |       | 命令消息        |
| Forward    |       | 转发消息        |

消息内容类型

### enum DeliveryQos

| Enumerator  | Value | Description |
| ----------- | ----- | ----------- |
| AtLastOnce  |       | 最少投递一次      |
| AtMostOnce  |       | 最多投递一次      |
| ExactlyOnce |       | 仅投递一次       |

消息投递质量

## Public Functions Documentation

### function \~BMXMessage

```cpp
virtual ~BMXMessage()
```

析构函数

### function msgId

```cpp
int64_t msgId()
```

消息唯一ID

**Return**: int64\_t

### function clientMsgId

```cpp
int64_t clientMsgId()
```

消息客户端ID,仅在消息发送端存在

**Return**: int64\_t

### function fromId

```cpp
int64_t fromId()
```

消息发送方ID

**Return**: int64\_t

### function toId

```cpp
int64_t toId()
```

消息接收方ID

**Return**: int64\_t

### function type

```cpp
MessageType type()
```

消息类型

**Return**: MessageType

### function conversationId

```cpp
int64_t conversationId()
```

消息所属会话ID

**Return**: int64\_t

### function deliveryStatus

```cpp
DeliveryStatus deliveryStatus()
```

消息投递状态

**Return**: DeliveryStatus

### function setDeliveryStatus

```cpp
void setDeliveryStatus(
    DeliveryStatus 
)
```

设置消息投递状态

### function serverTimestamp

```cpp
int64_t serverTimestamp()
```

消息时间戳（服务端收到时的时间）

**Return**: int64\_t

### function setServerTimestamp

```cpp
void setServerTimestamp(
    int64_t 
)
```

设置时间戳（服务端收到时的时间）

### function clientTimestamp

```cpp
int64_t clientTimestamp()
```

本地时间戳（消息创建或者收到时的本地时间）

**Return**: int64\_t

### function setClientTimestamp

```cpp
void setClientTimestamp(
    int64_t 
)
```

设置消息本地时间戳

### function isPlayed

```cpp
bool isPlayed()
```

语音或者视频消息是否播放过，仅对收到的音视频消息有效

**Return**: bool

### function setIsPlayed

```cpp
void setIsPlayed(
    bool 
)
```

设置语音或者视频消息是否播放过，仅对收到的音视频消息有效

### function isPlayAcked

```cpp
bool isPlayAcked()
```

对于发送方表示是否收到了已播放回执，对于接收方表示是否发送了已播放回执

**Return**: bool

### function setIsPlayAcked

```cpp
void setIsPlayAcked(
    bool 
)
```

设置已播放回执

### function isReceiveMsg

```cpp
bool isReceiveMsg()
```

是否接收的消息

**Return**: bool

### function setIsReceiveMsg

```cpp
void setIsReceiveMsg(
    bool 
)
```

设置是否接收的消息

### function isRead

```cpp
bool isRead()
```

消息是否已读标志

**Return**: bool

### function setIsRead

```cpp
void setIsRead(
    bool 
)
```

消息是否已读标志

### function isReadAcked

```cpp
bool isReadAcked()
```

对于发送方表示是否收到了已读回执，对于接收方表示是否发送了已读回执

**Return**: bool

### function setIsReadAcked

```cpp
void setIsReadAcked(
    bool 
)
```

设置已读回执

### function isDeliveryAcked

```cpp
bool isDeliveryAcked()
```

对于发送方表示消息是否已投递到对方，对于接收方表示是否发送了消息已到达回执

**Return**: bool

### function setIsDeliveryAcked

```cpp
void setIsDeliveryAcked(
    bool 
)
```

设置投递回执

### function content

```cpp
const std::string & content()
```

消息文本内容

**Return**: std::string

### function setContent

```cpp
void setContent(
    const std::string & content
)
```

消息文本内容

**Parameters**:

* **content** 消息文本内容

### function contentType

```cpp
ContentType contentType()
```

消息内容类型，如果带附件就表示附件类型，不带附件就是文本类型

**Return**: ContentType

### function attachment

```cpp
BMXMessageAttachmentPtr attachment()
```

消息附件，BMXMessage拥有附件的所有权，负责释放

**Return**: BMXMessageAttachmentPtr

### function config

```cpp
BMXMessageConfigPtr config()
```

消息的配置信息

**Return**: JSON(std::string)

### function setConfig

```cpp
void setConfig(
    BMXMessageConfigPtr 
)
```

设置消息配置信息

### function extension

```cpp
const JSON & extension()
```

消息扩展信息

**Return**: JSON(std::string)

### function setExtension

```cpp
void setExtension(
    const JSON & 
)
```

设置消息扩展信息

### function deliveryQos

```cpp
DeliveryQos deliveryQos()
```

消息投递QOS

**Return**: DeliveryQos

### function setDeliveryQos

```cpp
void setDeliveryQos(
    DeliveryQos qos
)
```

设置消息投递QOS

**Parameters**:

* **qos** 消息投递QOS

### function senderName

```cpp
const std::string & senderName()
```

消息发送者的显示名称

**Return**: std::string

### function setSenderName

```cpp
void setSenderName(
    const std::string & senderName
)
```

设置消息的发送者显示名称

**Parameters**:

* **senderName** 消息文本内容

### function groupAckCount

```cpp
int groupAckCount()
```

群消息已读AckCount数目

**Return**: int

### function setGroupAckCount

```cpp
void setGroupAckCount(
    int count
)
```

设置消息已读groupAckCount数目(SDK 内部调用接口，上层不应该调用)

**Parameters**:

* **count** 设置群消息已读数目

### function groupAckUnreadCount

```cpp
int groupAckUnreadCount()
```

群消息未读AckCount数目

**Return**: int

### function setGroupAckUnreadCount

```cpp
void setGroupAckUnreadCount(
    int count
)
```

设置消息未读groupAckCount数目(SDK 内部调用接口，上层不应该调用)

**Parameters**:

* **count** 设置群消息未读数目

### function groupAckReadAll

```cpp
bool groupAckReadAll()
```

群消息是否全部已读

**Return**: bool

### function groupPlayAckCount

```cpp
int groupPlayAckCount()
```

群消息已播放AckCount数目（仅用于音频/视频附件消息）

**Return**: int

### function setGroupPlayAckCount

```cpp
void setGroupPlayAckCount(
    int count
)
```

设置消息已播放groupAckCount数目(SDK 内部调用接口，上层不应该调用)（仅用于音频/视频附件消息）

**Parameters**:

* **count** 设置群消息已读数目

### function groupPlayAckUnreadCount

```cpp
int groupPlayAckUnreadCount()
```

群消息未播放AckCount数目（仅用于音频/视频附件消息）

**Return**: int

### function setGroupPlayAckUnreadCount

```cpp
void setGroupPlayAckUnreadCount(
    int count
)
```

设置消息未播放groupAckCount数目(SDK 内部调用接口，上层不应该调用)（仅用于音频/视频附件消息）

**Parameters**:

* **count** 设置群消息未播放数目

### function groupPlayAckReadAll

```cpp
bool groupPlayAckReadAll()
```

群消息是否全部已播放

**Return**: bool

### function setPriority

```cpp
void setPriority(
    int priority
)
```

设置消息的扩散优先级，默认为0。0表示扩散，数字越小扩散的越多。

**Parameters**:

* **priority** 设置群消息未读数目

取值范围0-10。普通人在聊天室发送的消息级别默认为5，可以丢弃。管理员默认为0不会丢弃。其它值可以根据业务自行设置。

### function priority

```cpp
int priority()
```

消息的扩散优先级

**Return**: int

### function setPushMessageMode

```cpp
void setPushMessageMode(
    bool 
)
```

设置消息是否为推送消息。

### function isPushMessage

```cpp
bool isPushMessage()
```

消息是否是推送消息

**Return**: bool

### function createMessage

```cpp
static BMXMessagePtr createMessage(
    int64_t from,
    int64_t to,
    MessageType type,
    int64_t conversationId,
    const std::string & content
)
```

创建发送文本消息

**Parameters**:

* **from** 消息发送者
* **to** 消息接收者
* **type** 消息类型
* **conversationId** 会话id
* **content** 消息内容

### function createMessage

```cpp
static BMXMessagePtr createMessage(
    int64_t from,
    int64_t to,
    MessageType type,
    int64_t conversationId,
    BMXMessageAttachmentPtr attachment
)
```

创建发送附件消息

**Parameters**:

* **from** 消息发送者
* **to** 消息接收者
* **type** 消息类型
* **conversationId** 会话id
* **attachment** 附件

### function createCommandMessage

```cpp
static BMXMessagePtr createCommandMessage(
    int64_t from,
    int64_t to,
    MessageType type,
    int64_t conversationId,
    const std::string & content
)
```

创建发送命令消息(命令消息通过content字段或者extension字段存放命令信息)

**Parameters**:

* **from** 消息发送者
* **to** 消息接收者
* **type** 消息类型
* **conversationId** 会话id
* **content** 消息内容

### function createMessage

```cpp
static BMXMessagePtr createMessage(
    int64_t msgId,
    int64_t from,
    int64_t to,
    MessageType type,
    int64_t conversationId,
    const std::string & content,
    int64_t serverTimestamp
)
```

创建收到的消息

**Parameters**:

* **msgId** 消息id
* **from** 消息发送者
* **to** 消息接收者
* **type** 消息类型
* **conversationId** 会话id
* **content** 消息内容
* **serverTimestamp** 服务器时间戳

### function createMessage

```cpp
static BMXMessagePtr createMessage(
    int64_t msgId,
    int64_t from,
    int64_t to,
    MessageType type,
    int64_t conversationId,
    BMXMessageAttachmentPtr attachment,
    int64_t serverTimestamp
)
```

创建收到的消息

**Parameters**:

* **msgId** 消息id
* **from** 消息发送者
* **to** 消息接收者
* **type** 消息类型
* **conversationId** 会话id
* **attachment** 附件
* **serverTimestamp** 服务器时间戳

### function createCommandMessage

```cpp
static BMXMessagePtr createCommandMessage(
    int64_t msgId,
    int64_t from,
    int64_t to,
    MessageType type,
    int64_t conversationId,
    const std::string & content,
    int64_t serverTimestamp
)
```

创建收到的命令消息(命令消息通过content字段或者extension字段存放命令信息)

**Parameters**:

* **msgId** 消息id
* **from** 消息发送者
* **to** 消息接收者
* **type** 消息类型
* **conversationId** 会话id
* **content** 消息内容
* **serverTimestamp** 服务器时间戳

### function createForwardMessage

```cpp
static BMXMessagePtr createForwardMessage(
    BMXMessagePtr msg,
    int64_t from,
    int64_t to,
    MessageType type,
    int64_t conversationId
)
```

创建转发消息

**Parameters**:

* **msg** 要转发的消息
* **from** 消息发送者
* **to** 消息接收者
* **type** 消息类型
* **conversationId** 会话id

***

Updated on 2022-01-26 at 17:20:40 +0800
