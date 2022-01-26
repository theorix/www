# floo::BMXForwardAttachment::Message

转发消息附件自定义消息

`#include <bmx_forward_attachment.h>`

## Public Functions

|         | Name                                                                |
| ------- | ------------------------------------------------------------------- |
|         | **Message**(std::shared\_ptr< [BMXMessage](broken-reference) > msg) |
| virtual | **\~Message**()                                                     |

## Public Attributes

|                         | Name                |
| ----------------------- | ------------------- |
| int64\_t                | **msgId**           |
| int64\_t                | **fromId**          |
| int64\_t                | **clientTimestamp** |
| int64\_t                | **serverTimestamp** |
| std::string             | **content**         |
| Type                    | **contentType**     |
| BMXMessageAttachmentPtr | **attachment**      |
| JSON                    | **extension**       |

## Public Functions Documentation

### function Message

```cpp
Message(
    std::shared_ptr< BMXMessage > msg
)
```

### function \~Message

```cpp
inline virtual ~Message()
```

## Public Attributes Documentation

### variable msgId

```cpp
int64_t msgId;
```

### variable fromId

```cpp
int64_t fromId;
```

### variable clientTimestamp

```cpp
int64_t clientTimestamp;
```

### variable serverTimestamp

```cpp
int64_t serverTimestamp;
```

### variable content

```cpp
std::string content;
```

### variable contentType

```cpp
Type contentType;
```

### variable attachment

```cpp
BMXMessageAttachmentPtr attachment;
```

### variable extension

```cpp
JSON extension;
```

***

Updated on 2022-01-26 at 17:20:40 +0800
