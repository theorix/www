# floo::BMXForwardAttachment

消息转发附件

`#include <bmx_forward_attachment.h>`

Inherits from [floo::BMXMessageAttachment](broken-reference), BMXBaseObject

## Public Classes

|       | Name                                                                          |
| ----- | ----------------------------------------------------------------------------- |
| class | <p><a href="broken-reference"><strong>Message</strong></a><br>转发消息附件自定义消息</p> |

## Public Functions

|                                 | Name                                                    |
| ------------------------------- | ------------------------------------------------------- |
|                                 | <p><strong>BMXForwardAttachment</strong>()<br>构造函数</p>  |
| virtual                         | <p><strong>~BMXForwardAttachment</strong>()<br>析构函数</p> |
| virtual Type                    | <p><strong>type</strong>() const<br>附件类型</p>            |
| virtual BMXMessageAttachmentPtr | <p><strong>clone</strong>() const<br>克隆函数</p>           |

## Additional inherited members

**Public Types inherited from** [**floo::BMXMessageAttachment**](broken-reference)

|            | Name                                                                                                  |
| ---------- | ----------------------------------------------------------------------------------------------------- |
| enum class | <p><strong>Type</strong> { Image, Voice, Video, File, Location, Command, Forward}<br>附件类型</p>         |
| enum class | <p><strong>DownloadStatus</strong> { Downloaing, Successed, Failed, NotStart, Canceled}<br>附件下载状态</p> |

**Public Functions inherited from** [**floo::BMXMessageAttachment**](broken-reference)

|         | Name                                                    |
| ------- | ------------------------------------------------------- |
|         | <p><strong>BMXMessageAttachment</strong>()<br>构造函数</p>  |
| virtual | <p><strong>~BMXMessageAttachment</strong>()<br>析构函数</p> |

## Public Functions Documentation

### function BMXForwardAttachment

```cpp
inline BMXForwardAttachment()
```

构造函数

### function \~BMXForwardAttachment

```cpp
inline virtual ~BMXForwardAttachment()
```

析构函数

### function type

```cpp
inline virtual Type type() const
```

附件类型

**Return**: Type

**Reimplements**: floo::BMXMessageAttachment::type

### function clone

```cpp
virtual BMXMessageAttachmentPtr clone() const
```

克隆函数

**Return**: BMXMessageAttachmentPtr

**Reimplements**: floo::BMXMessageAttachment::clone

***

Updated on 2022-01-26 at 17:20:40 +0800
