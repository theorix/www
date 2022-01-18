# BMXImageAttachment Class Reference

#### &#x20; `thumbnailPath`

`@property (nonatomic, copy) NSString *thumbnailPath`

#### &#x20; `thumbnailFileLength`

`@property (nonatomic, assign) long long thumbnailFileLength`

#### &#x20; `thumbnailSize`

`@property (nonatomic) CGSize thumbnailSize`

#### &#x20; `pictureSize`

`@property (nonatomic) CGSize pictureSize`

#### &#x20; `thumbnailDownLoadStatus`

`@property (nonatomic, assign) BMXAttachmentDownloadStatus thumbnailDownLoadStatus`

#### `– initWithData:thumbnailData:imageSize:conversationId:`

`- (instancetype)initWithData:(NSData *)`_`aData`_` ``thumbnailData:(NSData *)`_`aThumbnailData`_` ``imageSize:(CGSize)`_`imageSize`_` ``conversationId:(NSString *)`_`conversationId`_

#### `– initWithLocalPath:thumbnailPath:size:displayName:conversationId:`

`- (instancetype)initWithLocalPath:(NSString *)`_`aLocalPath`_` ``thumbnailPath:(NSString *)`_`aThumbnailPath`_` ``size:(CGSize)`_`size`_` ``displayName:(NSString *)`_`aDisplayName`_` ``conversationId:(NSString *)`_`conversationId`_

#### `– setReceiveThumbnailUrl:thumbnailSize:fileLength:`

设置接收图片消息缩略图

`- (void)setReceiveThumbnailUrl:(NSString *)`_`url`_` ``thumbnailSize:(CGSize)`_`thumbnailSize`_` ``fileLength:(long long)`_`fileLength`_

**Declared In**

`BMXImageAttachment.h`

#### `– setsendThumbnailPath:`

设置发送图片消息缩略图

`- (void)setsendThumbnailPath:(NSString *)`_`path`_

**Declared In**

`BMXImageAttachment.h`
