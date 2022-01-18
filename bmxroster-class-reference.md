# BMXRoster Class Reference

#### &#x20; `rosterId`

好友Id

`@property (nonatomic, assign, readonly) long long rosterId`

#### &#x20; `userName`

好友名

`@property (nonatomic, copy, readonly) NSString *userName`

#### &#x20; `nickName`

好友昵称

`@property (nonatomic, copy, readonly) NSString *nickName`

#### &#x20; `avatarUrl`

好友头像

`@property (nonatomic, copy, readonly) NSString *avatarUrl`

#### &#x20; `avatarPath`

好友头像本地存储路径

`@property (nonatomic, copy, readonly) NSString *avatarPath`

#### &#x20; `avatarThumbnailPath`

好友头像缩略图本地存储路径

`@property (nonatomic, copy, readonly) NSString *avatarThumbnailPath`

#### &#x20; `json_PublicInfo`

扩展信息，用户设置的好友可以看到的信息，比如地址，个性签名等

`@property (nonatomic, copy, readonly) NSString *json_PublicInfo`

**Discussion**

扩展信息，用户设置的好友可以看到的信息，比如地址，个性签名等

#### &#x20; `json_alias`

用户对好友添加的备注等信息

`@property (nonatomic, copy, readonly) NSString *json_alias`

#### &#x20; `json_ext`

用户的服务器扩展信息

`@property (nonatomic, copy, readonly) NSString *json_ext`

#### &#x20; `json_localExt`

用户的本地扩展信息

`@property (nonatomic, copy, readonly) NSString *json_localExt`

#### &#x20; `isMuteNotification`

是否提醒用户消息

`@property (nonatomic, assign, readonly) BOOL isMuteNotification`

#### &#x20; `rosterRelation`

联系人关系

`@property (nonatomic, assign, readonly) BMXRosterRelation rosterRelation`
