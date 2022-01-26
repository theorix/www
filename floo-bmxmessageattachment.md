# floo::BMXMessageAttachment

消息附件

`#include <bmx_message_attachment.h>`

Inherits from BMXBaseObject

Inherited by [floo::BMXFileAttachment](broken-reference), [floo::BMXForwardAttachment](broken-reference), [floo::BMXLocationAttachment](broken-reference)

## Public Types

|            | Name                                                                                                  |
| ---------- | ----------------------------------------------------------------------------------------------------- |
| enum class | <p><strong>Type</strong> { Image = 1, Voice, Video, File, Location, Command, Forward}<br>附件类型</p>     |
| enum class | <p><strong>DownloadStatus</strong> { Downloaing, Successed, Failed, NotStart, Canceled}<br>附件下载状态</p> |

## Public Functions

|                                                                      | Name                                                    |
| -------------------------------------------------------------------- | ------------------------------------------------------- |
|                                                                      | <p><strong>BMXMessageAttachment</strong>()<br>构造函数</p>  |
| virtual                                                              | <p><strong>~BMXMessageAttachment</strong>()<br>析构函数</p> |
| virtual Type                                                         | <p><strong>type</strong>() const =0<br>附件类型</p>         |
| virtual std::shared\_ptr< [BMXMessageAttachment](broken-reference) > | <p><strong>clone</strong>() const =0<br>复制附件</p>        |

## Public Types Documentation

### enum Type

| Enumerator | Value | Description |
| ---------- | ----- | ----------- |
| Image      | 1     | 图片          |
| Voice      |       | 语音          |
| Video      |       | 视频片段        |
| File       |       | 文件          |
| Location   |       | 位置          |
| Command    |       | 命令消息        |
| Forward    |       | 转发消息        |

附件类型

### enum DownloadStatus

| Enumerator | Value | Description |
| ---------- | ----- | ----------- |
| Downloaing |       | 下载中         |
| Successed  |       | 下载成功        |
| Failed     |       | 下载失败        |
| NotStart   |       | 下载尚未开始      |
| Canceled   |       | 下载被取消       |

附件下载状态

## Public Functions Documentation

### function BMXMessageAttachment

```cpp
inline BMXMessageAttachment()
```

构造函数

### function \~BMXMessageAttachment

```cpp
inline virtual ~BMXMessageAttachment()
```

析构函数

### function type

```cpp
virtual Type type() const =0
```

附件类型

**Return**: Type

**Reimplemented by**: floo::BMXFileAttachment::type, floo::BMXForwardAttachment::type, floo::BMXImageAttachment::type, floo::BMXLocationAttachment::type, floo::BMXVideoAttachment::type, floo::BMXVoiceAttachment::type

### function clone

```cpp
virtual std::shared_ptr< BMXMessageAttachment > clone() const =0
```

复制附件

**Return**: BMXMessageAttachmentPtr

**Reimplemented by**: floo::BMXFileAttachment::clone, floo::BMXForwardAttachment::clone, floo::BMXImageAttachment::clone, floo::BMXLocationAttachment::clone, floo::BMXVideoAttachment::clone, floo::BMXVoiceAttachment::clone

***

Updated on 2022-01-26 at 17:20:40 +0800
