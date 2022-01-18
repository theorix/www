# BMXVoiceAttachment Class Reference

#### &#x20; `duration`

时长

`@property (nonatomic, assign) int duration`

**Declared In**

`BMXVoiceAttachment.h`

#### `– initWithPath:displayName:duration:conversationId:`

`- (instancetype)initWithPath:(NSString *)`_`path`_` ``displayName:(NSString *)`_`displayName`_` ``duration:(NSInteger)`_`duration`_` ``conversationId:(NSString *)`_`conversationId`_

**Parameters**

| `path`        | 音频路径 |
| ------------- | ---- |
| `displayName` | 显示   |
| `duration`    | 时长   |

**Declared In**

`BMXVoiceAttachment.h`

#### `– initWithData:displayName:fileLength:duration:conversationId:`

`- (instancetype)initWithData:(NSData *)`_`aData`_` ``displayName:(NSString *)`_`displayName`_` ``fileLength:(NSInteger)`_`fileLength`_` ``duration:(NSInteger)`_`duration`_` ``conversationId:(NSString *)`_`conversationId`_

**Parameters**

| `aData`          | 音频Data |
| ---------------- | ------ |
| `displayName`    | 显示名称   |
| `duration`       | 时长     |
| `conversationId` | 会话Id   |

**Declared In**

`BMXVoiceAttachment.h`
