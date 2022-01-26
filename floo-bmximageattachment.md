# floo::BMXImageAttachment

图片消息附件

`#include <bmx_image_attachment.h>`

Inherits from [floo::BMXFileAttachment](broken-reference), [floo::BMXMessageAttachment](broken-reference), BMXBaseObject

## Public Functions

|                                 | Name                                                                                                                                                                                 |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
|                                 | <p><strong>BMXImageAttachment</strong>(const std::string &#x26; path, const [Size] &#x26; size, const std::string &#x26; displayName ="")<br>构造函数，构建发送图片消息附件</p>                     |
|                                 | <p><strong>BMXImageAttachment</strong>(const std::string &#x26; ratelUrl, const [Size] &#x26; size, const std::string &#x26; displayName, int64_t fileLength)<br>构造函数，构建接收图片消息附件</p> |
| virtual                         | <p><strong>~BMXImageAttachment</strong>()<br>析构函数</p>                                                                                                                                |
| virtual Type                    | <p><strong>type</strong>() const<br>返回图片附件类型</p>                                                                                                                                     |
| virtual BMXMessageAttachmentPtr | <p><strong>clone</strong>() const<br>克隆函数</p>                                                                                                                                        |
| const \[Size] &                 | <p><strong>size</strong>() const<br>图片大小</p>                                                                                                                                         |
| const std::string &             | <p><strong>thumbnailUrl</strong>() const<br>远程使用缩略图URL</p>                                                                                                                           |
| void                            | <p><strong>setThumbnail</strong>(const std::string &#x26; path)<br>设置发送图片消息缩略图</p>                                                                                                   |
| const std::string &             | <p><strong>thumbnailPath</strong>() const<br>缩略图本地路径</p>                                                                                                                             |
| DownloadStatus                  | <p><strong>thumbnailDownloadStatus</strong>() const<br>缩略图下载状态</p>                                                                                                                   |

## Friends

|       | Name                              |
| ----- | --------------------------------- |
| class | **Encoder< BMXImageAttachment >** |
| class | **Decoder< BMXImageAttachment >** |

## Additional inherited members

**Public Functions inherited from** [**floo::BMXFileAttachment**](broken-reference)

|                     | Name                                                                                                                                                      |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
|                     | <p><strong>BMXFileAttachment</strong>(const std::string &#x26; path, const std::string &#x26; displayName ="")<br>构造函数，构建发送文件消息附件</p>                     |
|                     | <p><strong>BMXFileAttachment</strong>(const std::string &#x26; ratelUrl, const std::string &#x26; displayName, int64_t fileLength)<br>构造函数，构建接收文件消息附件</p> |
| virtual             | <p><strong>~BMXFileAttachment</strong>()<br>析构函数</p>                                                                                                      |
| const std::string & | <p><strong>path</strong>() const<br>本地路径</p>                                                                                                              |
| const std::string & | <p><strong>displayName</strong>() const<br>显示名</p>                                                                                                        |
| const std::string & | <p><strong>ratelUrl</strong>() const<br>远程ratel使用URL</p>                                                                                                  |
| const std::string & | <p><strong>url</strong>() const<br>远程使用URL</p>                                                                                                            |
| int64\_t            | <p><strong>fileLength</strong>() const<br>文件长度</p>                                                                                                        |
| DownloadStatus      | <p><strong>downloadStatus</strong>() const<br>附件下载状态</p>                                                                                                  |

**Protected Attributes inherited from** [**floo::BMXFileAttachment**](broken-reference)

|                | Name                |
| -------------- | ------------------- |
| std::string    | **mPath**           |
| std::string    | **mDisplayName**    |
| std::string    | **mRatelUrl**       |
| std::string    | **mUrl**            |
| int64\_t       | **mFileLength**     |
| DownloadStatus | **mDownloadStatus** |

**Friends inherited from** [**floo::BMXFileAttachment**](broken-reference)

|       | Name                             |
| ----- | -------------------------------- |
| class | **Encoder< BMXFileAttachment >** |
| class | **Decoder< BMXFileAttachment >** |

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

### function BMXImageAttachment

```cpp
BMXImageAttachment(
    const std::string & path,
    const Size & size,
    const std::string & displayName =""
)
```

构造函数，构建发送图片消息附件

**Parameters**:

* **path** 本地路径
* **size** 图片的大小，宽度和高度
* **displayName** 展示名

### function BMXImageAttachment

```cpp
BMXImageAttachment(
    const std::string & ratelUrl,
    const Size & size,
    const std::string & displayName,
    int64_t fileLength
)
```

构造函数，构建接收图片消息附件

**Parameters**:

* **url** 图片ratel服务器地址
* **size** 图片的大小，宽度和高度
* **displayName** 展示名
* **fileLength** 文件大小

### function \~BMXImageAttachment

```cpp
inline virtual ~BMXImageAttachment()
```

析构函数

### function type

```cpp
inline virtual Type type() const
```

返回图片附件类型

**Return**: Type

**Reimplements**: floo::BMXFileAttachment::type

### function clone

```cpp
virtual BMXMessageAttachmentPtr clone() const
```

克隆函数

**Return**: BMXMessageAttachmentPtr

**Reimplements**: floo::BMXFileAttachment::clone

### function size

```cpp
const Size & size() const
```

图片大小

**Return**: Size

### function thumbnailUrl

```cpp
const std::string & thumbnailUrl() const
```

远程使用缩略图URL

**Return**: std::string

### function setThumbnail

```cpp
void setThumbnail(
    const std::string & path
)
```

设置发送图片消息缩略图

**Parameters**:

* **path** 本地路径

### function thumbnailPath

```cpp
const std::string & thumbnailPath() const
```

缩略图本地路径

**Return**: std::string

### function thumbnailDownloadStatus

```cpp
DownloadStatus thumbnailDownloadStatus() const
```

缩略图下载状态

**Return**: DownloadStatus

## Friends

### friend Encoder< BMXImageAttachment >

```cpp
friend class Encoder< BMXImageAttachment >(
    Encoder< BMXImageAttachment > 
);
```

### friend Decoder< BMXImageAttachment >

```cpp
friend class Decoder< BMXImageAttachment >(
    Decoder< BMXImageAttachment > 
);
```

***

Updated on 2022-01-26 at 17:20:40 +0800
