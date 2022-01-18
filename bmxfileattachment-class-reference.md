# BMXFileAttachment Class Reference

#### &#x20; `path`

本地路径

`@property (nonatomic, copy) NSString *path`

**Declared In**

`BMXFileAttachment.h`

#### &#x20; `displayName`

显示名称

`@property (nonatomic, copy) NSString *displayName`

**Declared In**

`BMXFileAttachment.h`

#### &#x20; `url`

文件url

`@property (nonatomic, copy) NSString *url`

**Declared In**

`BMXFileAttachment.h`

#### &#x20; `fileLength`

文件大小

`@property (nonatomic, assign) long long fileLength`

**Declared In**

`BMXFileAttachment.h`

#### &#x20; `downLoadStatus`

下载状态

`@property (nonatomic, assign) BMXAttachmentDownloadStatus downLoadStatus`

**Declared In**

`BMXFileAttachment.h`

#### `– initWithData:displayName:conversationId:`

初始化文件BMXFileAttachment

`- (instancetype)initWithData:(NSData *)`_`aData`_` ``displayName:(NSString *)`_`displayName`_` ``conversationId:(NSString *)`_`conversationId`_

**Parameters**

| `aData`          | 文件数据 |
| ---------------- | ---- |
| `displayName`    | 文件名称 |
| `conversationId` | 会话id |

**Return Value**

BMXFileAttachment

**Discussion**

初始化文件BMXFileAttachment

**Declared In**

`BMXFileAttachment.h`

#### `– initWithPath:displayName:conversationId:`

初始化文件BMXFileAttachment

`- (instancetype)initWithPath:(NSString *)`_`path`_` ``displayName:(NSString *)`_`displayName`_` ``conversationId:(NSString *)`_`conversationId`_

**Parameters**

| `path`           | 文件路径 |
| ---------------- | ---- |
| `displayName`    | 文件名称 |
| `conversationId` | 会话id |

**Discussion**

初始化文件BMXFileAttachment

**Declared In**

`BMXFileAttachment.h`
