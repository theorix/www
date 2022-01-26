# floo::BMXChatServiceListener

聊天监听者

`#include <bmx_chat_service_listener.h>`

## Public Functions

|              | Name                                                                                                                                                          |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|              | <p><strong>BMXChatServiceListener</strong>()<br>构造函数</p>                                                                                                      |
| virtual      | <p><strong>~BMXChatServiceListener</strong>()<br>析构函数</p>                                                                                                     |
| virtual void | <p><strong>onStatusChanged</strong>(BMXMessagePtr msg, BMXErrorCode error)<br>消息发送状态发生变化</p>                                                                  |
| virtual void | <p><strong>onAttachmentUploadProgressChanged</strong>(BMXMessagePtr msg, int percent)<br>附件上传进度发送变化</p>                                                       |
| virtual void | <p><strong>onRecallStatusChanged</strong>(BMXMessagePtr msg, BMXErrorCode error)<br>消息撤回状态发送变化</p>                                                            |
| virtual void | <p><strong>onReceive</strong>(const BMXMessageList &#x26; list)<br>收到消息</p>                                                                                   |
| virtual void | <p><strong>onReceiveCommandMessages</strong>(const BMXMessageList &#x26; list)<br>收到命令消息</p>                                                                  |
| virtual void | <p><strong>onReceiveSystemMessages</strong>(const BMXMessageList &#x26; list)<br>收到系统通知消息</p>                                                                 |
| virtual void | <p><strong>onReceiveReadAcks</strong>(const BMXMessageList &#x26; list)<br>收到消息已读回执</p>                                                                       |
| virtual void | <p><strong>onReceiveDeliverAcks</strong>(const BMXMessageList &#x26; list)<br>收到消息已送达回执</p>                                                                   |
| virtual void | <p><strong>onReceiveRecallMessages</strong>(const BMXMessageList &#x26; list)<br>收到撤回消息</p>                                                                   |
| virtual void | <p><strong>onReceiveReadCancels</strong>(const BMXMessageList &#x26; list)<br>收到消息已读取消（多设备其他设备同步消息已读状态变为未读）</p>                                               |
| virtual void | <p><strong>onReceiveReadAllMessages</strong>(const BMXMessageList &#x26; list)<br>收到消息全部已读（多设备同步某消息之前消息全部设置为已读）</p>                                           |
| virtual void | <p><strong>onReceiveDeleteMessages</strong>(const BMXMessageList &#x26; list)<br>收到删除消息 （多设备同步删除消息）</p>                                                       |
| virtual void | <p><strong>onReceivePlayAcks</strong>(const BMXMessageList &#x26; list)<br>收到音频/视频消息已播放回执</p>                                                                 |
| virtual void | <p><strong>onAttachmentStatusChanged</strong>(BMXMessagePtr msg, BMXErrorCode error, int percent)<br>附件下载状态发生变化</p>                                           |
| virtual void | <p><strong>onAttachmentDownloadByUrlStatusChanged</strong>(int64_t msgId, BMXErrorCode error, int percent)<br>附件下载状态发生变化</p>                                  |
| virtual void | <p><strong>onRetrieveHistoryMessages</strong>(BMXConversationPtr conversation)<br>拉取历史消息</p>                                                                  |
| virtual void | <p><strong>onLoadAllConversation</strong>()<br>已经加载完未读会话列表</p>                                                                                                |
| virtual void | <p><strong>onConversationCreate</strong>(BMXConversationPtr conversation, BMXMessagePtr msg)<br>本地创建新会话</p>                                                   |
| virtual void | <p><strong>onConversationDelete</strong>(int64_t conversationId, BMXErrorCode error)<br>删除会话</p>                                                              |
| virtual void | <p><strong>onTotalUnreadCountChanged</strong>(int unreadCount)<br>更新总未读数</p>                                                                                  |
| void         | <p><strong>registerChatService</strong>(<a href="broken-reference">BMXChatService</a> * service)<br>注册BMXChatServiceListener绑定到的BMXChatService（SDK内部自动注册）</p> |

## Protected Attributes

|                                       | Name         |
| ------------------------------------- | ------------ |
| [BMXChatService](broken-reference) \* | **mService** |

## Public Functions Documentation

### function BMXChatServiceListener

```cpp
inline BMXChatServiceListener()
```

构造函数

### function \~BMXChatServiceListener

```cpp
inline virtual ~BMXChatServiceListener()
```

析构函数

### function onStatusChanged

```cpp
inline virtual void onStatusChanged(
    BMXMessagePtr msg,
    BMXErrorCode error
)
```

消息发送状态发生变化

**Parameters**:

* **msg** 发生状态变化的消息
* **error** 状态错误码

### function onAttachmentUploadProgressChanged

```cpp
inline virtual void onAttachmentUploadProgressChanged(
    BMXMessagePtr msg,
    int percent
)
```

附件上传进度发送变化

**Parameters**:

* **msg** 上传附件的消息
* **percent** 附件上传的进度

### function onRecallStatusChanged

```cpp
inline virtual void onRecallStatusChanged(
    BMXMessagePtr msg,
    BMXErrorCode error
)
```

消息撤回状态发送变化

**Parameters**:

* **msg** 撤回状态发生变化的消息
* **error** 状态错误码

### function onReceive

```cpp
inline virtual void onReceive(
    const BMXMessageList & list
)
```

收到消息

**Parameters**:

* **list** 接收到的消息列表

### function onReceiveCommandMessages

```cpp
inline virtual void onReceiveCommandMessages(
    const BMXMessageList & list
)
```

收到命令消息

**Parameters**:

* **list** 接收到的消息列表

### function onReceiveSystemMessages

```cpp
inline virtual void onReceiveSystemMessages(
    const BMXMessageList & list
)
```

收到系统通知消息

**Parameters**:

* **list** 接收到的系统消息列表

### function onReceiveReadAcks

```cpp
inline virtual void onReceiveReadAcks(
    const BMXMessageList & list
)
```

收到消息已读回执

**Parameters**:

* **list** 接收到的已读回执消息列表

### function onReceiveDeliverAcks

```cpp
inline virtual void onReceiveDeliverAcks(
    const BMXMessageList & list
)
```

收到消息已送达回执

**Parameters**:

* **list** 接收到的已送达回执消息列表

### function onReceiveRecallMessages

```cpp
inline virtual void onReceiveRecallMessages(
    const BMXMessageList & list
)
```

收到撤回消息

**Parameters**:

* **list** 接收到的撤回消息列表

### function onReceiveReadCancels

```cpp
inline virtual void onReceiveReadCancels(
    const BMXMessageList & list
)
```

收到消息已读取消（多设备其他设备同步消息已读状态变为未读）

**Parameters**:

* **list** 接收到的消息已读取消消息列表

### function onReceiveReadAllMessages

```cpp
inline virtual void onReceiveReadAllMessages(
    const BMXMessageList & list
)
```

收到消息全部已读（多设备同步某消息之前消息全部设置为已读）

**Parameters**:

* **list** 接收到的消息全部已读消息列表

### function onReceiveDeleteMessages

```cpp
inline virtual void onReceiveDeleteMessages(
    const BMXMessageList & list
)
```

收到删除消息 （多设备同步删除消息）

**Parameters**:

* **list** 接收到的删除消息列表

### function onReceivePlayAcks

```cpp
inline virtual void onReceivePlayAcks(
    const BMXMessageList & list
)
```

收到音频/视频消息已播放回执

**Parameters**:

* **list** 接收到的音频/视频消息已播放回执消息列表

### function onAttachmentStatusChanged

```cpp
inline virtual void onAttachmentStatusChanged(
    BMXMessagePtr msg,
    BMXErrorCode error,
    int percent
)
```

附件下载状态发生变化

**Parameters**:

* **msg** 发生下载状态变化的消息
* **error** 状态错误码
* **percent** 附件下载的进度

### function onAttachmentDownloadByUrlStatusChanged

```cpp
inline virtual void onAttachmentDownloadByUrlStatusChanged(
    int64_t msgId,
    BMXErrorCode error,
    int percent
)
```

附件下载状态发生变化

**Parameters**:

* **msgId** 发生下载状态变化的消息Id
* **error** 状态错误码
* **percent** 附件下载的进度

### function onRetrieveHistoryMessages

```cpp
inline virtual void onRetrieveHistoryMessages(
    BMXConversationPtr conversation
)
```

拉取历史消息

**Parameters**:

* **conversation** 发生了拉取指历史消息的会话

### function onLoadAllConversation

```cpp
inline virtual void onLoadAllConversation()
```

已经加载完未读会话列表

### function onConversationCreate

```cpp
inline virtual void onConversationCreate(
    BMXConversationPtr conversation,
    BMXMessagePtr msg
)
```

本地创建新会话

**Parameters**:

* **conversation** 新创建的本地会话
* **msg** 会话的最新消息，存在返回不存在返回为空

### function onConversationDelete

```cpp
inline virtual void onConversationDelete(
    int64_t conversationId,
    BMXErrorCode error
)
```

删除会话

**Parameters**:

* **conversationId** 删除的本地会话id
* **error** 状态错误码

### function onTotalUnreadCountChanged

```cpp
inline virtual void onTotalUnreadCountChanged(
    int unreadCount
)
```

更新总未读数

**Parameters**:

* **unreadCount** 本地全部会话未读总数

### function registerChatService

```cpp
inline void registerChatService(
    BMXChatService * service
)
```

注册BMXChatServiceListener绑定到的BMXChatService（SDK内部自动注册）

**Parameters**:

* **service** [BMXChatService](broken-reference)

## Protected Attributes Documentation

### variable mService

```cpp
BMXChatService * mService;
```

***

Updated on 2022-01-26 at 17:20:40 +0800
