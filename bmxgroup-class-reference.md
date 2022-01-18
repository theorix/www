# BMXGroup Class Reference

#### &#x20; `groupId`

群Id

`@property (nonatomic, assign, readonly) long long groupId`

#### &#x20; `groupType`

`@property (nonatomic, assign, readonly) BMXGroupType groupType`

#### &#x20; `myNickName`

在群里的昵称

`@property (nonatomic, copy, readonly) NSString *myNickName`

#### &#x20; `name`

群名称

`@property (nonatomic, copy, readonly) NSString *name`

#### &#x20; `groupDescription`

群描述

`@property (nonatomic, copy, readonly) NSString *groupDescription`

#### &#x20; `avatarUrl`

群头像

`@property (nonatomic, copy, readonly) NSString *avatarUrl`

#### &#x20; `avatarPath`

群头像下载后的本地路径

`@property (nonatomic, copy, readonly) NSString *avatarPath`

#### &#x20; `avatarThumbnailUrl`

群头像缩略图

`@property (nonatomic, copy, readonly) NSString *avatarThumbnailUrl`

#### &#x20; `avatarThumbnailPath`

群头像缩略图下载后的本地路径

`@property (nonatomic, copy, readonly) NSString *avatarThumbnailPath`

**Discussion**

群头像缩略图下载后的本地路径

#### &#x20; `creatTime`

群创建时间

`@property (nonatomic, readonly) long long creatTime`

#### &#x20; `jsonextension`

群扩展信息

`@property (nonatomic, copy, readonly) NSString *jsonextension`

#### &#x20; `shareFile`

`@property (nonatomic, strong, readonly) BMXGroupSharedFile *shareFile`

#### &#x20; `ownerId`

群成员

`@property (nonatomic, assign, readonly) NSInteger ownerId`

#### &#x20; `annountment`

`@property (nonatomic, strong) BMXGroupAnnounment *annountment`

#### &#x20; `capactiy`

最大人数

`@property (nonatomic, assign, readonly) NSInteger capactiy`

#### &#x20; `membersCount`

群成员数量，包含Owner，admins 和members

`@property (nonatomic, assign, readonly) NSInteger membersCount`

**Discussion**

群成员数量，包含Owner，admins 和members

#### &#x20; `adminsCount`

群管理员数量

`@property (nonatomic, assign, readonly) NSInteger adminsCount`

#### &#x20; `sharedFilesCount`

群共享文件数量

`@property (nonatomic, assign, readonly) NSInteger sharedFilesCount`

#### &#x20; `msgPushMode`

群消息通知类型

`@property (nonatomic, assign, readonly) BMXGroupMsgPushMode msgPushMode`

#### &#x20; `modifyMode`

群信息修改模式

`@property (nonatomic, assign, readonly) BMXGroupModifyMode modifyMode`

#### &#x20; `joinAuthMode`

入群审批模式

`@property (nonatomic, assign, readonly) BMXGroupJoinAuthMode joinAuthMode`

#### &#x20; `inviteMode`

入群邀请模式

`@property (nonatomic, assign, readonly) BMXGroupInviteMode inviteMode`

#### &#x20; `enableReadAck`

是否开启群消息已读功能

`@property (nonatomic, assign) BOOL enableReadAck`

#### &#x20; `historyVisible`

是否可以加载显示历史聊天记录

`@property (nonatomic, assign) BOOL historyVisible`

**Discussion**

是否可以加载显示历史聊天记录

#### &#x20; `msgMuteMode`

群消息屏蔽模式

`@property (nonatomic, assign) BMXGroupMsgMuteMode msgMuteMode`

#### &#x20; `groupStatus`

当前群组的状态。（Normal 正常， Destroyed 以销毁）

`@property (nonatomic, assign) BMXGroupStatus groupStatus`

**Discussion**

当前群组的状态。（Normal 正常， Destroyed 以销毁）

#### &#x20; `isMember`

`@property (nonatomic, assign, readonly) BOOL isMember`

#### &#x20; `roleType`

`@property (nonatomic, assign) BMXGroupMemberRoleType roleType`
