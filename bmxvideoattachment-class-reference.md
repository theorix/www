# BMXVideoAttachment Class Reference

#### &#x20; `videoSize`

video大小

`@property (nonatomic) CGSize videoSize`

**Declared In**

`BMXVideoAttachment.h`

#### &#x20; `duration`

时长

`@property (nonatomic, assign) int duration`

**Declared In**

`BMXVideoAttachment.h`

#### &#x20; `thumbnailPath`

缩略图路径

`@property (nonatomic, copy) NSString *thumbnailPath`

**Declared In**

`BMXVideoAttachment.h`

#### &#x20; `thumbnailUrl`

缩略图url

`@property (nonatomic, copy) NSString *thumbnailUrl`

**Declared In**

`BMXVideoAttachment.h`

#### &#x20; `thumbnailFileLength`

thumbnail文件大小

`@property (nonatomic) long long thumbnailFileLength`

**Declared In**

`BMXVideoAttachment.h`

#### &#x20; `thumbnaildownLoadStatus`

视频下载状态

`@property (nonatomic, assign) BMXAttachmentDownloadStatus thumbnaildownLoadStatus`

**Declared In**

`BMXVideoAttachment.h`

#### `– initWithData:duration:videoSize:displayName:conversationId:`

`- (instancetype)initWithData:(NSData *)`_`aData`_` ``duration:(int)`_`duration`_` ``videoSize:(CGSize)`_`videoSize`_` ``displayName:(NSString *)`_`displayName`_` ``conversationId:(NSString *)`_`conversationId`_

#### `– initWithData:duration:videoSize:displayName:thumbnailData:conversationId:`

`- (instancetype)initWithData:(NSData *)`_`aData`_` ``duration:(int)`_`duration`_` ``videoSize:(CGSize)`_`videoSize`_` ``displayName:(NSString *)`_`displayName`_` ``thumbnailData:(NSData *)`_`thumbnailData`_` ``conversationId:(NSString *)`_`conversationId`_

#### `– initWithLocalPath:duration:size:displayName:conversationId:`

`- (instancetype)initWithLocalPath:(NSString *)`_`aLocalPath`_` ``duration:(int)`_`duration`_` ``size:(CGSize)`_`size`_` ``displayName:(NSString *)`_`aDisplayName`_` ``conversationId:(NSString *)`_`conversationId`_

#### `– initWithLocalPath:duration:size:thumbnailPath:displayName:conversationId:`

`- (instancetype)initWithLocalPath:(NSString *)`_`aLocalPath`_` ``duration:(int)`_`duration`_` ``size:(CGSize)`_`size`_` ``thumbnailPath:(NSString *)`_`thumbnailPath`_` ``displayName:(NSString *)`_`aDisplayName`_` ``conversationId:(NSString *)`_`conversationId`_
