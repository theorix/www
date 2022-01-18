# BMXConversation Class Reference

| Inherits from | NSObject          |
| ------------- | ----------------- |
| Declared in   | BMXConversation.h |

#### &#x20; `conversationId`

会话Id

`@property (nonatomic, assign, readonly) long long conversationId`

**Declared In**

`BMXConversation.h`

#### &#x20; `type`

会话类型

`@property (nonatomic, assign, readonly) BMXConversationType type`

**Declared In**

`BMXConversation.h`

#### &#x20; `lastMessage`

最新消息

`@property (nonatomic, strong, readonly) BMXMessageObject *lastMessage`

**Declared In**

`BMXConversation.h`

#### &#x20; `unreadNumber`

未读消息数量

`@property (nonatomic, assign, readonly) NSInteger unreadNumber`

**Declared In**

`BMXConversation.h`

#### &#x20; `messageCount`

会话中所有消息数量

`@property (nonatomic, assign, readonly) NSInteger messageCount`

**Declared In**

`BMXConversation.h`

#### &#x20; `isMuteNotication`

是否提醒用户消息,不提醒的情况下会话总未读数不会统计该会话计数。

`@property (nonatomic, assign) BOOL isMuteNotication`

**Discussion**

是否提醒用户消息,不提醒的情况下会话总未读数不会统计该会话计数。

**Declared In**

`BMXConversation.h`

#### &#x20; `extensionJson`

扩展信息

`@property (nonatomic, copy) NSString *extensionJson`

**Declared In**

`BMXConversation.h`

#### &#x20; `editMessage`

编辑消息

`@property (nonatomic, copy) NSString *editMessage`

**Declared In**

`BMXConversation.h`

#### `– setMessagePlayedStatus:status:completion:`

设置消息播放状态（只对语音/视频消息有效）

`- (void)setMessagePlayedStatus:(BMXMessageObject *)`_`message`_` ``status:(bool)`_`status`_` ``completion:(void ( ^ ) ( BMXMessageObject *aMessage , BMXError *error ))`_`aCompletionBlock`_

**Parameters**

| `message`          | message |
| ------------------ | ------- |
| `status`           | 播放状态    |
| `aCompletionBlock` | Result  |

**Discussion**

设置消息播放状态（只对语音/视频消息有效）

**Declared In**

`BMXConversation.h`

#### `– setMessageReadStatus:status:completion:`

设置消息未读状态，更新未读消息数, 本地

`- (void)setMessageReadStatus:(BMXMessageObject *)`_`message`_` ``status:(BOOL)`_`status`_` ``completion:(void ( ^ ) ( BMXError *error ))`_`aCompletionBlock`_

**Parameters**

| `message`          | message |
| ------------------ | ------- |
| `status`           | 是否已读    |
| `aCompletionBlock` | Result  |

**Discussion**

设置消息未读状态，更新未读消息数, 本地

**Declared In**

`BMXConversation.h`

#### `– setAllMessagesReadCompletion:`

把所有消息设置为已读，更新未读消息数

`- (void)setAllMessagesReadCompletion:(void ( ^ ) ( BMXError *error ))`_`aCompletionBlock`_

**Discussion**

把所有消息设置为已读，更新未读消息数

**Declared In**

`BMXConversation.h`

#### `– updateMessageExtension:completion:`

更新一条数据库存储消息的扩展字段信息

`- (void)updateMessageExtension:(BMXMessageObject *)`_`message`_` ``completion:(void ( ^ ) ( BMXError *error ))`_`aCompletionBlock`_

**Parameters**

| `message`          | 需要更改扩展信息的消息此时msg部分已经更新扩展字椴信息 |
| ------------------ | ---------------------------- |
| `aCompletionBlock` | 更新结果                         |

**Discussion**

更新一条数据库存储消息的扩展字段信息

**Declared In**

`BMXConversation.h`

#### `– insertMessage:completion:`

插入一条消息

`- (void)insertMessage:(BMXMessageObject *)`_`msg`_` ``completion:(void ( ^ ) ( BMXError *error ))`_`aCompletionBlock`_

**Parameters**

| `msg`              | message |
| ------------------ | ------- |
| `aCompletionBlock` | Result  |

**Declared In**

`BMXConversation.h`

#### `– loadMessage:completion:`

读取一条消息

`- (void)loadMessage:(long long)`_`msgId`_` ``completion:(void ( ^ ) ( BMXMessageObject *message ))`_`aCompletionBlock`_

**Parameters**

| `msgId`            | msgId  |
| ------------------ | ------ |
| `aCompletionBlock` | Result |

**Declared In**

`BMXConversation.h`

#### `– removeAllMessagescompletion:`

删除会话中的所有消息

`- (void)removeAllMessagescompletion:(void ( ^ ) ( BMXError *error ))`_`aCompletionBlock`_

**Parameters**

| `aCompletionBlock` | Result |
| ------------------ | ------ |

**Declared In**

`BMXConversation.h`

#### `– loadMessageFromMessageId:size:completion:`

加载消息，从参考消息向前加载，如果不指定则从最新消息开始

`- (void)loadMessageFromMessageId:(long long)`_`reMsgId`_` ``size:(NSUInteger)`_`size`_` ``completion:(void ( ^ ) ( NSArray *messageList , BMXError *error ))`_`aCompletionBlock`_

**Parameters**

| `reMsgId`          | 参考消息Id             |
| ------------------ | ------------------ |
| `size`             | size               |
| `aCompletionBlock` | Result：MessageList |

**Discussion**

加载消息，从参考消息向前加载，如果不指定则从最新消息开始

**Declared In**

`BMXConversation.h`

#### `– searchMessagesByKeyWords:refTime:size:directionType:completion:`

搜索消息，如果不指定则从最新消息开始

`- (void)searchMessagesByKeyWords:(NSString *)`_`keywords`_` ``refTime:(NSTimeInterval)`_`refTime`_` ``size:(NSUInteger)`_`size`_` ``directionType:(BMXMessageDirection)`_`directionType`_` ``completion:(void ( ^ ) ( NSArray<BMXMessageObject*> *messageList , BMXError *error ))`_`aCompletionBlock`_

**Discussion**

搜索消息，如果不指定则从最新消息开始

**Declared In**

`BMXConversation.h`

#### `– searchMessagesBycontentType:refTime:size:directionType:completion:`

按照类型搜索消息，如果不指定则从最新消息开始

`- (void)searchMessagesBycontentType:(BMXContentType)`_`contentType`_` ``refTime:(NSTimeInterval)`_`refTime`_` ``size:(NSUInteger)`_`size`_` ``directionType:(BMXMessageDirection)`_`directionType`_` ``completion:(void ( ^ ) ( NSArray<BMXMessageObject*> *messageList , BMXError *error ))`_`aCompletionBlock`_

**Discussion**

按照类型搜索消息，如果不指定则从最新消息开始

**Declared In**

`BMXConversation.h`
