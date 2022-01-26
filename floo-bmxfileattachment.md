# floo::BMXFileAttachment

消息文件附件

`#include <bmx_file_attachment.h>`

Inherits from [floo::BMXMessageAttachment](broken-reference), BMXBaseObject

Inherited by [floo::BMXImageAttachment](broken-reference), floo::BMXVideoAttachment, floo::BMXVoiceAttachment

## Public Functions

|                                 | Name                                                                                                                                                      |
| ------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
|                                 | <p><strong>BMXFileAttachment</strong>(const std::string &#x26; path, const std::string &#x26; displayName ="")<br>构造函数，构建发送文件消息附件</p>                     |
|                                 | <p><strong>BMXFileAttachment</strong>(const std::string &#x26; ratelUrl, const std::string &#x26; displayName, int64_t fileLength)<br>构造函数，构建接收文件消息附件</p> |
| virtual                         | <p><strong>~BMXFileAttachment</strong>()<br>析构函数</p>                                                                                                      |
| virtual Type                    | <p><strong>type</strong>() const<br>返回文件类型</p>                                                                                                            |
| virtual BMXMessageAttachmentPtr | <p><strong>clone</strong>() const<br>克隆函数</p>                                                                                                             |
| const std::string &             | <p><strong>path</strong>() const<br>本地路径</p>                                                                                                              |
| const std::string &             | <p><strong>displayName</strong>() const<br>显示名</p>                                                                                                        |
| const std::string &             | <p><strong>ratelUrl</strong>() const<br>远程ratel使用URL</p>                                                                                                  |
| const std::string &             | <p><strong>url</strong>() const<br>远程使用URL</p>                                                                                                            |
| int64\_t                        | <p><strong>fileLength</strong>() const<br>文件长度</p>                                                                                                        |
| DownloadStatus                  | <p><strong>downloadStatus</strong>() const<br>附件下载状态</p>                                                                                                  |

## Protected Attributes

|                | Name                |
| -------------- | ------------------- |
| std::string    | **mPath**           |
| std::string    | **mDisplayName**    |
| std::string    | **mRatelUrl**       |
| std::string    | **mUrl**            |
| int64\_t       | **mFileLength**     |
| DownloadStatus | **mDownloadStatus** |

## Friends

|       | Name                             |
| ----- | -------------------------------- |
| class | **Encoder< BMXFileAttachment >** |
| class | **Decoder< BMXFileAttachment >** |

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

### function BMXFileAttachment

```cpp
BMXFileAttachment(
    const std::string & path,
    const std::string & displayName =""
)
```

构造函数，构建发送文件消息附件

**Parameters**:

* **path** 文件的本地路径
* **displayName** 文件展示名

### function BMXFileAttachment

```cpp
BMXFileAttachment(
    const std::string & ratelUrl,
    const std::string & displayName,
    int64_t fileLength
)
```

构造函数，构建接收文件消息附件

**Parameters**:

* **ratelUrl** ratel文件服务器地址
* **displayName** 文件展示名
* **fileLength** 文件大小

### function \~BMXFileAttachment

```cpp
inline virtual ~BMXFileAttachment()
```

析构函数

### function type

```cpp
inline virtual Type type() const
```

返回文件类型

**Return**: Type

**Reimplements**: floo::BMXMessageAttachment::type

**Reimplemented by**: floo::BMXImageAttachment::type, floo::BMXVideoAttachment::type, floo::BMXVoiceAttachment::type

### function clone

```cpp
virtual BMXMessageAttachmentPtr clone() const
```

克隆函数

**Return**: BMXMessageAttachmentPtr

**Reimplements**: floo::BMXMessageAttachment::clone

**Reimplemented by**: floo::BMXImageAttachment::clone, floo::BMXVideoAttachment::clone, floo::BMXVoiceAttachment::clone

### function path

```cpp
const std::string & path() const
```

本地路径

**Return**: std::string

### function displayName

```cpp
const std::string & displayName() const
```

显示名

**Return**: std::string

### function ratelUrl

```cpp
const std::string & ratelUrl() const
```

远程ratel使用URL

**Return**: std::string

### function url

```cpp
const std::string & url() const
```

远程使用URL

**Return**: std::string

### function fileLength

```cpp
int64_t fileLength() const
```

文件长度

**Return**: std::string

### function downloadStatus

```cpp
DownloadStatus downloadStatus() const
```

附件下载状态

**Return**: DownloadStatus

## Protected Attributes Documentation

### variable mPath

```cpp
std::string mPath;
```

### variable mDisplayName

```cpp
std::string mDisplayName;
```

### variable mRatelUrl

```cpp
std::string mRatelUrl;
```

### variable mUrl

```cpp
std::string mUrl;
```

### variable mFileLength

```cpp
int64_t mFileLength;
```

### variable mDownloadStatus

```cpp
DownloadStatus mDownloadStatus;
```

## Friends

### friend Encoder< BMXFileAttachment >

```cpp
friend class Encoder< BMXFileAttachment >(
    Encoder< BMXFileAttachment > 
);
```

### friend Decoder< BMXFileAttachment >

```cpp
friend class Decoder< BMXFileAttachment >(
    Decoder< BMXFileAttachment > 
);
```

***

Updated on 2022-01-26 at 17:20:40 +0800
