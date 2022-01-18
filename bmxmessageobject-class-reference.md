# BMXMessageObject Class Reference

| Inherits from | NSObject           |
| ------------- | ------------------ |
| Declared in   | BMXMessageObject.h |

#### &#x20; `msgId`

`@property (nonatomic, assign, readonly) long long msgId`

#### &#x20; `fromId`

`@property (nonatomic, assign, readonly) long long fromId`

#### &#x20; `toId`

`@property (nonatomic, assign, readonly) long long toId`

#### &#x20; `conversationId`

`@property (nonatomic, assign) long long conversationId`

#### &#x20; `deliverystatus`

`@property (nonatomic, assign) BMXDeliveryStatus deliverystatus`

#### &#x20; `qos`

`@property (nonatomic, assign) DeliveryQosMode qos`

#### &#x20; `messageType`

`@property (nonatomic, assign, readonly) BMXMessageType messageType`

#### &#x20; `serverTimestamp`

`@property (nonatomic, assign, readonly) long long serverTimestamp`

#### &#x20; `clientTimestamp`

`@property (nonatomic, assign) long long clientTimestamp`

#### &#x20; `isPlayed`

`@property (nonatomic, assign) BOOL isPlayed`

#### &#x20; `isReceiveMsg`

`@property (nonatomic, assign) BOOL isReceiveMsg`

#### &#x20; `isRead`

`@property (nonatomic, assign) BOOL isRead`

#### &#x20; `isReadAcked`

`@property (nonatomic, assign) BOOL isReadAcked`

#### &#x20; `isDeliveryAcked`

`@property (nonatomic, assign) BOOL isDeliveryAcked`

#### &#x20; `content`

`@property (nonatomic, copy) NSString *content`

#### &#x20; `messageconfig`

`@property (nonatomic, strong) BMXMessageConfig *messageconfig`

#### &#x20; `extensionJson`

`@property (nonatomic, copy) NSString *extensionJson`

#### &#x20; `contentType`

`@property (nonatomic, assign) BMXContentType contentType`

#### &#x20; `senderName`

`@property (nonatomic, copy) NSString *senderName`

#### &#x20; `groupAckCount`

`@property (nonatomic, assign) int groupAckCount`

#### &#x20; `attachment`

`@property (nonatomic, strong, readonly) BMXMessageAttachment *attachment`

#### `– initWithBMXMessageText:fromId:toId:type:conversationId:`

创建文本消息

`- (instancetype)initWithBMXMessageText:(NSString *)`_`content`_` ``fromId:(long long)`_`fromId`_` ``toId:(long long)`_`toId`_` ``type:(BMXMessageType)`_`mtype`_` ``conversationId:(long long)`_`conversationId`_

**Parameters**

| `content`        | 内容   |
| ---------------- | ---- |
| `fromId`         | 发送id |
| `toId`           | 接收id |
| `mtype`          | 消息类型 |
| `conversationId` | 会话id |

**Return Value**

BMXMessageObject

**Declared In**

`BMXMessageObject.h`

#### `– initWithBMXCommandMessageText:fromId:toId:type:conversationId:`

创建发送命令消息(命令消息通过content字段或者extension字段存放命令信息)

`- (instancetype)initWithBMXCommandMessageText:(NSString *)`_`content`_` ``fromId:(long long)`_`fromId`_` ``toId:(long long)`_`toId`_` ``type:(BMXMessageType)`_`mtype`_` ``conversationId:(long long)`_`conversationId`_

**Parameters**

| `content`        | 消息内容  |
| ---------------- | ----- |
| `fromId`         | 消息发送者 |
| `toId`           | 消息接收者 |
| `mtype`          | 消息类型  |
| `conversationId` | 会话id  |

**Discussion**

创建发送命令消息(命令消息通过content字段或者extension字段存放命令信息)

**Declared In**

`BMXMessageObject.h`

#### `– initWithBMXMessageAttachment:fromId:toId:type:conversationId:`

创建附件消息

`- (instancetype)initWithBMXMessageAttachment:(BMXMessageAttachment *)`_`attachment`_` ``fromId:(long long)`_`fromId`_` ``toId:(long long)`_`toId`_` ``type:(BMXMessageType)`_`mtype`_` ``conversationId:(long long)`_`conversationId`_

**Return Value**

BMXMessageObject

**Declared In**

`BMXMessageObject.h`

#### `– initWithRecieveBMXMessageText:msgId:fromId:toId:type:conversationId:timeStamp:`

创建接收文本消息

`- (instancetype)initWithRecieveBMXMessageText:(NSString *)`_`content`_` ``msgId:(long long)`_`msgId`_` ``fromId:(long long)`_`fromId`_` ``toId:(long long)`_`toId`_` ``type:(BMXMessageType)`_`mtype`_` ``conversationId:(long long)`_`conversationId`_` ``timeStamp:(long long)`_`timeStamp`_

**Parameters**

| `content`        | 内容   |
| ---------------- | ---- |
| `msgId`          | 消息id |
| `fromId`         | 发送id |
| `toId`           | 接收id |
| `mtype`          | 消息类型 |
| `conversationId` | 会话id |
| `timeStamp`      | 时间戳  |

**Return Value**

BMXMessageObject

**Declared In**

`BMXMessageObject.h`

#### `– initWithRecieveBMXMessageCommandMessageText:msgId:fromId:toId:type:conversationId:timeStamp:`

创建收到的命令消息(命令消息通过content字段或者extension字段存放命令信息)

`- (instancetype)initWithRecieveBMXMessageCommandMessageText:(NSString *)`_`content`_` ``msgId:(long long)`_`msgId`_` ``fromId:(long long)`_`fromId`_` ``toId:(long long)`_`toId`_` ``type:(BMXMessageType)`_`mtype`_` ``conversationId:(long long)`_`conversationId`_` ``timeStamp:(long long)`_`timeStamp`_

**Parameters**

| `content`        | 消息内容   |
| ---------------- | ------ |
| `msgId`          | 消息id   |
| `fromId`         | 消息发送者  |
| `toId`           | 消息接收者  |
| `mtype`          | 消息类型   |
| `conversationId` | 会话id   |
| `timeStamp`      | 服务器时间戳 |

**Discussion**

创建收到的命令消息(命令消息通过content字段或者extension字段存放命令信息)

**Declared In**

`BMXMessageObject.h`

#### `– initWithRecieveBMXMessageAttachment:msgId:fromId:toId:type:conversationId:timeStamp:`

创建接收附件消息

`- (instancetype)initWithRecieveBMXMessageAttachment:(BMXMessageAttachment *)`_`attachment`_` ``msgId:(long long)`_`msgId`_` ``fromId:(long long)`_`fromId`_` ``toId:(long long)`_`toId`_` ``type:(BMXMessageType)`_`mtype`_` ``conversationId:(long long)`_`conversationId`_` ``timeStamp:(long long)`_`timeStamp`_

**Parameters**

| `attachment`     | [BMXMessageAttachment](broken-reference) |
| ---------------- | ---------------------------------------- |
| `msgId`          | 消息id                                     |
| `fromId`         | 发送id                                     |
| `toId`           | 接收id                                     |
| `mtype`          | 消息类型                                     |
| `conversationId` | 会话id                                     |
| `timeStamp`      | 时间戳                                      |

**Return Value**

BMXMessageObject

**Declared In**

`BMXMessageObject.h`

#### `– initWithForwardMessage:fromId:toId:type:conversationId:`

创建转发消息

`- (instancetype)initWithForwardMessage:(BMXMessageObject *)`_`message`_` ``fromId:(long long)`_`fromId`_` ``toId:(long long)`_`toId`_` ``type:(BMXMessageType)`_`mtype`_` ``conversationId:(long long)`_`conversationId`_

**Parameters**

| `message`        | BMXMessageObject |
| ---------------- | ---------------- |
| `fromId`         | 发送id             |
| `toId`           | 接收id             |
| `mtype`          | 消息类型             |
| `conversationId` | 会话id             |

**Return Value**

BMXMessageObject

**Declared In**

`BMXMessageObject.h`
