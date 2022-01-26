# floo::BMXLocationAttachment

位置消息附件

`#include <bmx_location_attachment.h>`

Inherits from [floo::BMXMessageAttachment](broken-reference), BMXBaseObject

## Public Functions

|                                 | Name                                                                                                                       |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
|                                 | <p><strong>BMXLocationAttachment</strong>(double latitude, double longitude, const std::string &#x26; address)<br>构造函数</p> |
| virtual                         | <p><strong>~BMXLocationAttachment</strong>()<br>析构函数</p>                                                                   |
| virtual Type                    | <p><strong>type</strong>() const<br>返回位置附件类型</p>                                                                           |
| virtual BMXMessageAttachmentPtr | <p><strong>clone</strong>() const<br>克隆函数</p>                                                                              |
| double                          | <p><strong>latitude</strong>() const<br>纬度</p>                                                                             |
| double                          | <p><strong>longitude</strong>() const<br>经度</p>                                                                            |
| const std::string &             | <p><strong>address</strong>() const<br>地址</p>                                                                              |

## Friends

|       | Name                                 |
| ----- | ------------------------------------ |
| class | **Encoder< BMXLocationAttachment >** |
| class | **Decoder< BMXLocationAttachment >** |

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

### function BMXLocationAttachment

```cpp
BMXLocationAttachment(
    double latitude,
    double longitude,
    const std::string & address
)
```

构造函数

**Parameters**:

* **latitude** 纬度
* **longitude** 经度
* **address** 地址名称

### function \~BMXLocationAttachment

```cpp
inline virtual ~BMXLocationAttachment()
```

析构函数

### function type

```cpp
inline virtual Type type() const
```

返回位置附件类型

**Return**: Type

**Reimplements**: floo::BMXMessageAttachment::type

### function clone

```cpp
virtual BMXMessageAttachmentPtr clone() const
```

克隆函数

**Return**: BMXMessageAttachmentPtr

**Reimplements**: floo::BMXMessageAttachment::clone

### function latitude

```cpp
double latitude() const
```

纬度

**Return**: double

### function longitude

```cpp
double longitude() const
```

经度

**Return**: double

### function address

```cpp
const std::string & address() const
```

地址

**Return**: std::string

## Friends

### friend Encoder< BMXLocationAttachment >

```cpp
friend class Encoder< BMXLocationAttachment >(
    Encoder< BMXLocationAttachment > 
);
```

### friend Decoder< BMXLocationAttachment >

```cpp
friend class Decoder< BMXLocationAttachment >(
    Decoder< BMXLocationAttachment > 
);
```

***

Updated on 2022-01-26 at 17:20:40 +0800
