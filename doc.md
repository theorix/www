# doc

## Modules

[groupManage](doc.md#module\_groupManage)

群管理

[rosterManage](doc.md#module\_rosterManage)

好友管理

[sysManage](doc.md#module\_sysManage)[userManage](doc.md#module\_userManage)[types](doc.md#module\_types)[flooim](doc.md#module\_flooim)

## groupManage

群管理

* [groupManage](doc.md#module\_groupManage)
  * [.asyncGetGroupInfo(group\_id, froce)](doc.md#module\_groupManage.asyncGetGroupInfo) ⇒ [`Promise.<GroupInfoAndSettings>`](doc.md#module\_types..GroupInfoAndSettings)
  * [.asyncGetJoinedGroups(froce)](doc.md#module\_groupManage.asyncGetJoinedGroups) ⇒ `Promise.<Array.<number>>`
  * [.openGroup(group\_id)](doc.md#module\_groupManage.openGroup)
  * [.getAllGroupDetail()](doc.md#module\_groupManage.getAllGroupDetail) ⇒ `Object.<number, module:types~GroupInfoAndSettings>`
  * [.asyncGetGroupMembers(group\_id)](doc.md#module\_groupManage.asyncGetGroupMembers) ⇒ `Promise.<Array.<module:types~GroupMember>>`
  * [.getGroupMembers(group\_id)](doc.md#module\_groupManage.getGroupMembers) ⇒ [`Array.<GroupMember>`](doc.md#module\_types..GroupMember)
  * [.asyncGetGroupListDetail(gids)](doc.md#module\_groupManage.asyncGetGroupListDetail) ⇒ `Promise.<Array.<module:types~BriefGroupInfoAndSettings>>`
  * [.getGruopMessage(gid)](doc.md#module\_groupManage.getGruopMessage) ⇒ [`Array.<Meta>`](doc.md#module\_types..Meta)
  * [.asyncGetInfo(params)](doc.md#module\_groupManage.asyncGetInfo) ⇒ [`Promise.<GroupInfoAndSettings>`](doc.md#module\_types..GroupInfoAndSettings)
  * [.asyncGetMemberList(param)](doc.md#module\_groupManage.asyncGetMemberList) ⇒ `Promise.<Array.<module:types~GroupMember>>`
  * [.readGroupMessage(group\_id, mid)](doc.md#groupmanage.readgroupmessage-group\_id-mid)
  * [.recallMessage(uid, mid)](doc.md#module\_groupManage.recallMessage)
  * [.getUnreadCount(gid)](doc.md#module\_groupManage.getUnreadCount) ⇒ `number`
  * [.asyncGetAdminList(params)](doc.md#module\_groupManage.asyncGetAdminList) ⇒ `Promise.<Array.<module:types~GroupMember>>`
  * [.asyncAdminAdd(params)](doc.md#module\_groupManage.asyncAdminAdd) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`
  * [.asyncAdminRemove(params)](doc.md#module\_groupManage.asyncAdminRemove) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`
  * [.asyncGetAnouncementById(params)](doc.md#module\_groupManage.asyncGetAnouncementById) ⇒ [`Promise.<GroupAnnouncement>`](doc.md#module\_types..GroupAnnouncement)
  * [.asyncAnouncementDelete(params)](doc.md#module\_groupManage.asyncAnouncementDelete) ⇒ `Promise.<boolean>`
  * [.asyncAnnouncementEdit(params)](doc.md#module\_groupManage.asyncAnnouncementEdit) ⇒ [`Promise.<GroupAnnouncement>`](doc.md#module\_types..GroupAnnouncement)
  * [.asyncGetAnnouncementList(params)](doc.md#module\_groupManage.asyncGetAnnouncementList) ⇒ `Promise.<Array.<module:types~GroupAnnouncement>>`
  * [.asyncCreate(params)](doc.md#module\_groupManage.asyncCreate) ⇒ [`Promise.<GroupInfoAndSettings>`](doc.md#module\_types..GroupInfoAndSettings)
  * [.asyncDestroy(params)](doc.md#module\_groupManage.asyncDestroy) ⇒ `Promise.<boolean>`
  * [.asyncUpdateAvatar(params)](doc.md#module\_groupManage.asyncUpdateAvatar) ⇒ `Promise.<boolean>`
  * [.asyncUpdateDescription(params)](doc.md#module\_groupManage.asyncUpdateDescription) ⇒ `Promise.<boolean>`
  * [.asyncUpdateExt(params)](doc.md#module\_groupManage.asyncUpdateExt) ⇒ `Promise.<boolean>`
  * [.asyncUpdateName(params)](doc.md#module\_groupManage.asyncUpdateName) ⇒ `Promise.<boolean>`
  * [.asyncGroupMsgMutemode(params)](doc.md#module\_groupManage.asyncGroupMsgMutemode) ⇒ `Promise.<boolean>`
  * [.asyncGroupBannedList(params)](doc.md#module\_groupManage.asyncGroupBannedList) ⇒ `Promise.<Array.<module:types~GroupMemberBanned>>`
  * [.asyncGroupBab(params)](doc.md#module\_groupManage.asyncGroupBab) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`
  * [.asyncGroupUnban(params)](doc.md#module\_groupManage.asyncGroupUnban) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`
  * [.asyncGetSettings(group\_id)](doc.md#module\_groupManage.asyncGetSettings) ⇒ [`Promise.<GroupInfoAndSettings>`](doc.md#module\_types..GroupInfoAndSettings)
  * [.asyncUpdateAllowMemberInvitation(params)](doc.md#module\_groupManage.asyncUpdateAllowMemberInvitation) ⇒ `Promise.<boolean>`
  * [.asyncUpdateAllowMemberModify(params)](doc.md#module\_groupManage.asyncUpdateAllowMemberModify) ⇒ `Promise.<boolean>`
  * [.asyncUpdateEnableReadack(params)](doc.md#module\_groupManage.asyncUpdateEnableReadack) ⇒ `Promise.<boolean>`
  * [.asyncUpdateHistoryVisible(params)](doc.md#module\_groupManage.asyncUpdateHistoryVisible) ⇒ `Promise.<boolean>`
  * [.asyncUpdateRequireadminapproval(params)](doc.md#module\_groupManage.asyncUpdateRequireadminapproval) ⇒ `Promise.<boolean>`
  * [.asyncBanAll(params)](doc.md#module\_groupManage.asyncBanAll) ⇒ [`Promise.<GroupBanAllResponse>`](doc.md#module\_types..GroupBanAllResponse)
  * [.asyncUnBanAll(params)](doc.md#module\_groupManage.asyncUnBanAll) ⇒ `Promise.<boolean>`
  * [.asyncOwnerTransfer(params)](doc.md#module\_groupManage.asyncOwnerTransfer) ⇒ [`Promise.<GroupUserRelationResponse>`](doc.md#module\_types..GroupUserRelationResponse)
  * [.asyncGetUserJoined(params)](doc.md#module\_groupManage.asyncGetUserJoined) ⇒ `Promise.<Array.<number>>`
  * [.asyncApply(params)](doc.md#module\_groupManage.asyncApply) ⇒ [`Promise.<GroupUserRelationResponse>`](doc.md#module\_types..GroupUserRelationResponse)
  * [.asyncApplyHandle(params)](doc.md#module\_groupManage.asyncApplyHandle) ⇒ [`Promise.<GroupUserRelationResponse>`](doc.md#module\_types..GroupUserRelationResponse)
  * [.asyncGroupBockedlist(params)](doc.md#module\_groupManage.asyncGroupBockedlist) ⇒ `Promise.<Array.<module:types~GroupBlockedListItem>>`
  * [.asyncGroupBlock(params)](doc.md#module\_groupManage.asyncGroupBlock) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`
  * [.asyncGroupUnblock(params)](doc.md#module\_groupManage.asyncGroupUnblock) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`
  * [.asyncKick(params)](doc.md#module\_groupManage.asyncKick) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`
  * [.asyncGetInvitationList()](doc.md#module\_groupManage.asyncGetInvitationList) ⇒ `Promise.<Array.<module:types~GroupInvitation>>`
  * [.asyncInvite(params)](doc.md#module\_groupManage.asyncInvite) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`
  * [.asyncInviteHandle(params)](doc.md#module\_groupManage.asyncInviteHandle) ⇒ `Promise.<boolean>`
  * [.asyncGetMemberDisplayName(params)](doc.md#module\_groupManage.asyncGetMemberDisplayName) ⇒ `Promise.<Array.<module:types~GroupMember>>`
  * [.asyncLeave(params)](doc.md#module\_groupManage.asyncLeave) ⇒ `Promise.<boolean>`
  * [.asyncUpdateDisplayName(params)](doc.md#module\_groupManage.asyncUpdateDisplayName) ⇒ `Promise.<boolean>`
  * [.asncGetApplicationList(params)](doc.md#module\_groupManage.asncGetApplicationList) ⇒ `Promise.<Array.<module:types~GroupApplication>>`
  * [.asyncGetFileList(params)](doc.md#module\_groupManage.asyncGetFileList) ⇒ `Promise.<Array.<module:types~GroupSharedFile>>`
  * [.asyncFileDelete(params)](doc.md#module\_groupManage.asyncFileDelete) ⇒ `Promise.<Array.<module:types~GroupSharedFileResponse>>`
  * [.asyncFileUpload(params)](doc.md#module\_groupManage.asyncFileUpload) ⇒ `Promise.<Array.<module:types~GroupSharedFile>>`

### groupManage.asyncGetGroupInfo(group\_id, froce) ⇒ [`Promise.<GroupInfoAndSettings>`](doc.md#module\_types..GroupInfoAndSettings)

获取群信息

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: [`Promise.<GroupInfoAndSettings>`](doc.md#module\_types..GroupInfoAndSettings) - 群信息

| Param     | Type      | Description                                  |
| --------- | --------- | -------------------------------------------- |
| group\_id | `number`  | 群ID                                          |
| froce     | `boolean` | 是否强制从服务器拉取： true - 从服务器拉取， false - 优先从本地存储获取 |

### groupManage.asyncGetJoinedGroups(froce) ⇒ `Promise.<Array.<number>>`

获取加入的群组

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<number>>` - 群组ID列表

| Param | Type      | Description                                  |
| ----- | --------- | -------------------------------------------- |
| froce | `boolean` | 是否强制从服务器拉取： true - 从服务器拉取， false - 优先从本地存储获取 |

### groupManage.openGroup(group\_id)

打开群组， 此方法会准备群组聊天界面的一些必备信息。

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)

| Param     | Type     | Description |
| --------- | -------- | ----------- |
| group\_id | `number` | 群组ID        |

### groupManage.getAllGroupDetail() ⇒ `Object.<number, module:types~GroupInfoAndSettings>`

获取缓存的所有群组详情

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Object.<number, module:types~GroupInfoAndSettings>` - 群组详情\


### groupManage.asyncGetGroupMembers(group\_id) ⇒ `Promise.<Array.<module:types~GroupMember>>`

获取群组成员（异步）

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupMember>>` - 群成员列表

| Param     | Type     | Description |
| --------- | -------- | ----------- |
| group\_id | `number` | 群组ID        |

### groupManage.getGroupMembers(group\_id) ⇒ [`Array.<GroupMember>`](doc.md#module\_types..GroupMember)

获取群组成员（同步）

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: [`Array.<GroupMember>`](doc.md#module\_types..GroupMember) - 群成员列表

| Param     | Type     | Description |
| --------- | -------- | ----------- |
| group\_id | `number` | 群组ID        |

### groupManage.asyncGetGroupListDetail(gids) ⇒ `Promise.<Array.<module:types~BriefGroupInfoAndSettings>>`

按id获取群组详情

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~BriefGroupInfoAndSettings>>` - 群组详情列表

| Param | Type             | Description |
| ----- | ---------------- | ----------- |
| gids  | `Array.<number>` | 群组ID列表      |

### groupManage.getGruopMessage(gid) ⇒ [`Array.<Meta>`](doc.md#module\_types..Meta)

获取群消息

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: [`Array.<Meta>`](doc.md#module\_types..Meta) - 群消息列表

| Param | Type     | Description |
| ----- | -------- | ----------- |
| gid   | `number` | 群ID         |

### groupManage.asyncGetInfo(params) ⇒ [`Promise.<GroupInfoAndSettings>`](doc.md#module\_types..GroupInfoAndSettings)

获取群组详情

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: [`Promise.<GroupInfoAndSettings>`](doc.md#module\_types..GroupInfoAndSettings) - 群组详情

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

### groupManage.asyncGetMemberList(param) ⇒ `Promise.<Array.<module:types~GroupMember>>`

获取群成员列表

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupMember>>` - 群成员列表

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| param            | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

### groupManage.readGroupMessage(group\_id, mid)

将群消息设置已读

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)

| Param     | Type     | Description |
| --------- | -------- | ----------- |
| group\_id | `number` | 群组ID        |
| mid       | `number` | 消息ID        |

### groupManage.recallMessage(uid, mid)

撤回消息

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)

| Param | Type     | Description |
| ----- | -------- | ----------- |
| uid   | `number` | 群组ID        |
| mid   | `number` | 消息ID        |

### groupManage.getUnreadCount(gid) ⇒ `number`

获取群未读消息数

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `number` - 未读消息数

| Param | Type     | Description |
| ----- | -------- | ----------- |
| gid   | `number` | 群组ID        |

### groupManage.asyncGetAdminList(params) ⇒ `Promise.<Array.<module:types~GroupMember>>`

获取群管理员列表

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupMember>>` - 群管理员列表

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

### groupManage.asyncAdminAdd(params) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`

群添加管理员

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupUserRelationResponse>>` - 结果列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.user\_list | `Array.<number>` | 群成员列表       |

### groupManage.asyncAdminRemove(params) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`

移除管理员

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupUserRelationResponse>>` - 结果列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.user\_list | `Array.<number>` | 群成员列表       |

### groupManage.asyncGetAnouncementById(params) ⇒ [`Promise.<GroupAnnouncement>`](doc.md#module\_types..GroupAnnouncement)

获取群公告详情

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: [`Promise.<GroupAnnouncement>`](doc.md#module\_types..GroupAnnouncement) - 群公告详情

| Param                   | Type             | Description |
| ----------------------- | ---------------- | ----------- |
| params                  | `object`         | 参数          |
| params.group\_id        | `number`         | 群组ID        |
| params.announcement\_id | `Array.<number>` | 公告ID        |

### groupManage.asyncAnouncementDelete(params) ⇒ `Promise.<boolean>`

删除群公告

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param                   | Type             | Description |
| ----------------------- | ---------------- | ----------- |
| params                  | `object`         | 参数          |
| params.group\_id        | `number`         | 群组ID        |
| params.announcement\_id | `Array.<number>` | 公告ID        |

### groupManage.asyncAnnouncementEdit(params) ⇒ [`Promise.<GroupAnnouncement>`](doc.md#module\_types..GroupAnnouncement)

编辑群公告

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: [`Promise.<GroupAnnouncement>`](doc.md#module\_types..GroupAnnouncement) - 群公告详情

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |
| params.title     | `string` | 公告标题        |
| params.content   | `string` | 公告内容        |

### groupManage.asyncGetAnnouncementList(params) ⇒ `Promise.<Array.<module:types~GroupAnnouncement>>`

群公告列表

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupAnnouncement>>` - 群公告详情列表

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

### groupManage.asyncCreate(params) ⇒ [`Promise.<GroupInfoAndSettings>`](doc.md#module\_types..GroupInfoAndSettings)

创建群组

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: [`Promise.<GroupInfoAndSettings>`](doc.md#module\_types..GroupInfoAndSettings) - 群详情

| Param  | Type                                                         | Description |
| ------ | ------------------------------------------------------------ | ----------- |
| params | [`GroupInfoRequest`](doc.md#module\_types..GroupInfoRequest) | 请求参数        |

### groupManage.asyncDestroy(params) ⇒ `Promise.<boolean>`

解散群组

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

### groupManage.asyncUpdateAvatar(params) ⇒ `Promise.<boolean>`

更新群头像

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |
| params.value     | `string` | 头像地址        |

### groupManage.asyncUpdateDescription(params) ⇒ `Promise.<boolean>`

更新群描述

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |
| params.value     | `string` | 群组描述        |

### groupManage.asyncUpdateExt(params) ⇒ `Promise.<boolean>`

更新群扩展信息

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |
| params.value     | `string` | 扩展信息        |

### groupManage.asyncUpdateName(params) ⇒ `Promise.<boolean>`

更新群名称

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |
| params.value     | `string` | 群名称         |

### groupManage.asyncGroupMsgMutemode(params) ⇒ `Promise.<boolean>`

设置群消息免打扰情况

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param                  | Type     | Description                                          |
| ---------------------- | -------- | ---------------------------------------------------- |
| params                 | `object` | 参数                                                   |
| params.group\_id       | `number` | 群组ID                                                 |
| params.msg\_mute\_mode | `number` | 群消息屏蔽模式: 0 - 表示不屏蔽, 1 - 表示屏蔽本地消息通知, 2 - 表示屏蔽消息，不接收消息 |

### groupManage.asyncGroupBannedList(params) ⇒ `Promise.<Array.<module:types~GroupMemberBanned>>`

获取群禁言列表

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupMemberBanned>>` - 禁言成员列表

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

### groupManage.asyncGroupBab(params) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`

禁言群成员

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupUserRelationResponse>>` - 请求结果列表

| Param  | Type                                                                         | Description |
| ------ | ---------------------------------------------------------------------------- | ----------- |
| params | [`GroupBannedMemberRequest`](doc.md#module\_types..GroupBannedMemberRequest) | 请求参数        |

### groupManage.asyncGroupUnban(params) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`

解除成员禁言

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupUserRelationResponse>>` - 请求结果列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.user\_list | `Array.<number>` | 群成员列表       |

### groupManage.asyncGetSettings(group\_id) ⇒ [`Promise.<GroupInfoAndSettings>`](doc.md#module\_types..GroupInfoAndSettings)

获取群设置

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: [`Promise.<GroupInfoAndSettings>`](doc.md#module\_types..GroupInfoAndSettings) - 群设置

| Param     | Type     | Description |
| --------- | -------- | ----------- |
| group\_id | `number` | 群ID         |

### groupManage.asyncUpdateAllowMemberInvitation(params) ⇒ `Promise.<boolean>`

设置群成员是否可以邀请

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type      | Description                             |
| ---------------- | --------- | --------------------------------------- |
| params           | `object`  | 参数                                      |
| params.group\_id | `number`  | 群组ID                                    |
| params.value     | `boolean` | 群成员邀请设置: false - 不允许邀请, true - 允许邀请(默认) |

### groupManage.asyncUpdateAllowMemberModify(params) ⇒ `Promise.<boolean>`

设置群成员是否可以修改群信息

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type      | Description                                           |
| ---------------- | --------- | ----------------------------------------------------- |
| params           | `object`  | 参数                                                    |
| params.group\_id | `number`  | 群组ID                                                  |
| params.value     | `boolean` | 群成员修改群信息设置: false - 群成员不能修改群信息(默认), true - 群成员可以修改群信息 |

### groupManage.asyncUpdateEnableReadack(params) ⇒ `Promise.<boolean>`

设置群是否开启已读模式

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type      | Description                         |
| ---------------- | --------- | ----------------------------------- |
| params           | `object`  | 参数                                  |
| params.group\_id | `number`  | 群组ID                                |
| params.value     | `boolean` | 是否开启群消息已读功能: false - 不开启, true - 开启 |

### groupManage.asyncUpdateHistoryVisible(params) ⇒ `Promise.<boolean>`

设置群历史是否可见

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type      | Description                       |
| ---------------- | --------- | --------------------------------- |
| params           | `object`  | 参数                                |
| params.group\_id | `number`  | 群组ID                              |
| params.value     | `boolean` | 设置群历史是否可见: false - 不可见, true - 可见 |

### groupManage.asyncUpdateRequireadminapproval(params) ⇒ `Promise.<boolean>`

设置入群是否需要申请

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param                  | Type      | Description                           |
| ---------------------- | --------- | ------------------------------------- |
| params                 | `object`  | 参数                                    |
| params.group\_id       | `number`  | 群组ID                                  |
| params.apply\_approval | `boolean` | 入群申请审批设置, 0:同意所有申请 1:需要管理员确认 2:拒绝所有申请 |

### groupManage.asyncBanAll(params) ⇒ [`Promise.<GroupBanAllResponse>`](doc.md#module\_types..GroupBanAllResponse)

全员禁言，只允许管理员发消息

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: [`Promise.<GroupBanAllResponse>`](doc.md#module\_types..GroupBanAllResponse) - 结果

| Param            | Type     | Description      |
| ---------------- | -------- | ---------------- |
| params           | `object` | 参数               |
| params.duration  | `number` | 禁言时长，单位为分钟,int64 |
| params.group\_id | `number` | 群id,int64        |

### groupManage.asyncUnBanAll(params) ⇒ `Promise.<boolean>`

取消全员禁言

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群id,int64   |

### groupManage.asyncOwnerTransfer(params) ⇒ [`Promise.<GroupUserRelationResponse>`](doc.md#module\_types..GroupUserRelationResponse)

更换群主

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: [`Promise.<GroupUserRelationResponse>`](doc.md#module\_types..GroupUserRelationResponse) - 结果

| Param             | Type     | Description |
| ----------------- | -------- | ----------- |
| params            | `object` | 参数          |
| params.group\_id  | `number` | 群组ID        |
| params.new\_owner | `number` | 新群主的用户ID    |

### groupManage.asyncGetUserJoined(params) ⇒ `Promise.<Array.<number>>`

获取用户的群组列表

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<number>>` - 群ID的列表

| Param  | Type     | Description |
| ------ | -------- | ----------- |
| params | `object` | 参数, 空对象     |

### groupManage.asyncApply(params) ⇒ [`Promise.<GroupUserRelationResponse>`](doc.md#module\_types..GroupUserRelationResponse)

申请加入群

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: [`Promise.<GroupUserRelationResponse>`](doc.md#module\_types..GroupUserRelationResponse) - 结果

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |
| params.reason    | `string` | 申请入群原因      |

### groupManage.asyncApplyHandle(params) ⇒ [`Promise.<GroupUserRelationResponse>`](doc.md#module\_types..GroupUserRelationResponse)

处理用户的入群申请

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: [`Promise.<GroupUserRelationResponse>`](doc.md#module\_types..GroupUserRelationResponse) - 结果

| Param            | Type      | Description           |
| ---------------- | --------- | --------------------- |
| params           | `object`  | 参数                    |
| params.group\_id | `number`  | 群组ID                  |
| params.user\_id  | `number`  | 用户ID                  |
| params.approval  | `boolean` | 审批结果：true为同意，false为拒绝 |

### groupManage.asyncGroupBockedlist(params) ⇒ `Promise.<Array.<module:types~GroupBlockedListItem>>`

获取群黑名单

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupBlockedListItem>>` - 群黑名单列表

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

### groupManage.asyncGroupBlock(params) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`

将成员加入黑名单

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupUserRelationResponse>>` - 结果列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.user\_list | `Array.<number>` | 群成员列表       |

### groupManage.asyncGroupUnblock(params) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`

解除黑名单

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupUserRelationResponse>>` - 结果列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.user\_list | `Array.<number>` | 群成员列表       |

### groupManage.asyncKick(params) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`

踢出群组

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupUserRelationResponse>>` - 结果列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.user\_list | `Array.<number>` | 群成员列表       |

### groupManage.asyncGetInvitationList() ⇒ `Promise.<Array.<module:types~GroupInvitation>>`

获取群邀请列表

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupInvitation>>` - 群邀请列表\


### groupManage.asyncInvite(params) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`

邀请成员加入群

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupUserRelationResponse>>` - 结果列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.user\_list | `Array.<number>` | 群成员列表       |

### groupManage.asyncInviteHandle(params) ⇒ `Promise.<boolean>`

处理群邀请

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type      | Description           |
| ---------------- | --------- | --------------------- |
| params           | `object`  | 参数                    |
| params.group\_id | `number`  | 群组ID                  |
| params.user\_id  | `number`  | 用户ID                  |
| params.approval  | `boolean` | 审批结果：true为同意，false为拒绝 |

### groupManage.asyncGetMemberDisplayName(params) ⇒ `Promise.<Array.<module:types~GroupMember>>`

批量获取群成员的群名片

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupMember>>` - 群成员列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.user\_list | `Array.<number>` | 群成员列表       |

### groupManage.asyncLeave(params) ⇒ `Promise.<boolean>`

退出群

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

### groupManage.asyncUpdateDisplayName(params) ⇒ `Promise.<boolean>`

修改群名片

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |
| params.value     | `string` | 新名片         |

### groupManage.asncGetApplicationList(params) ⇒ `Promise.<Array.<module:types~GroupApplication>>`

获取群申请列表

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupApplication>>` - 群申请列表

| Param              | Type             | Description |
| ------------------ | ---------------- | ----------- |
| params             | `object`         | 参数          |
| params.group\_list | `Array.<number>` | 群列表         |

### groupManage.asyncGetFileList(params) ⇒ `Promise.<Array.<module:types~GroupSharedFile>>`

获取群文件列表

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupSharedFile>>` - 群文件列表

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

### groupManage.asyncFileDelete(params) ⇒ `Promise.<Array.<module:types~GroupSharedFileResponse>>`

删除群文件

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupSharedFileResponse>>` - 结果列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.file\_list | `Array.<number>` | 文件ID列表      |

### groupManage.asyncFileUpload(params) ⇒ `Promise.<Array.<module:types~GroupSharedFile>>`

上传群文件

**Kind**: static method of [`groupManage`](doc.md#module\_groupManage)\
**Returns**: `Promise.<Array.<module:types~GroupSharedFile>>` - 群文件列表

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群id,int64   |
| params.name      | `string` | 文件名称        |
| params.size      | `number` | 文件大小,int64  |
| params.type      | `string` | 文件类型        |
| params.url       | `string` | 文件url       |

## rosterManage

好友管理

* [rosterManage](doc.md#module\_rosterManage)
  * [.asyncGetRosterIdList(force)](doc.md#module\_rosterManage.asyncGetRosterIdList) ⇒ `Promise.<Array.<number>>`
  * [.asyncGetRosterInfo(roster\_id, force)](doc.md#module\_rosterManage.asyncGetRosterInfo) ⇒ [`Promise.<RosterItem>`](doc.md#module\_types..RosterItem)
  * [.asyncRegester(opt)](doc.md#module\_rosterManage.asyncRegester) ⇒ [`Promise.<UserSettings>`](doc.md#module\_types..UserSettings)
  * [.asyncDeleteRoster(param)](doc.md#module\_rosterManage.asyncDeleteRoster) ⇒ `Promise.<boolean>`
  * [.asnycGetRosterListDetailByIds(roster\_ids)](doc.md#module\_rosterManage.asnycGetRosterListDetailByIds) ⇒ `Promise.<Array.<module:types~RosterItem>>`
  * [.getAllRosterDetail()](doc.md#module\_rosterManage.getAllRosterDetail) ⇒ [`Array.<RosterItem>`](doc.md#module\_types..RosterItem)
  * [.asyncGetUserProfile(force)](doc.md#module\_rosterManage.asyncGetUserProfile) ⇒ [`Promise.<UserProfile>`](doc.md#module\_types..UserProfile)
  * [.getRosterMessageByRid(uid)](doc.md#module\_rosterManage.getRosterMessageByRid) ⇒ [`Array.<Meta>`](doc.md#module\_types..Meta)
  * [.readRosterMessage(roster\_id, mid)](doc.md#module\_rosterManage.readRosterMessage)
  * [.recallMessage(uid, mid)](doc.md#module\_rosterManage.recallMessage)
  * [.unreadMessage(uid, mid)](doc.md#module\_rosterManage.unreadMessage)
  * [.deleteMessage(uid, mid)](doc.md#module\_rosterManage.deleteMessage)
  * [.getRosterInfo(rid)](doc.md#module\_rosterManage.getRosterInfo) ⇒ [`RosterItem`](doc.md#module\_types..RosterItem)
  * [.getUnreadCount(uid)](doc.md#module\_rosterManage.getUnreadCount) ⇒ `number`
  * [.asyncGetApplyList(params)](doc.md#module\_rosterManage.asyncGetApplyList) ⇒ `Promise.<Array.<module:types~RosterApplication>>`
  * [.asyncGetBlockedlist(params)](doc.md#module\_rosterManage.asyncGetBlockedlist) ⇒ `Promise.<Array.<number>>`
  * [.asyncBlockeAdd(params)](doc.md#module\_rosterManage.asyncBlockeAdd) ⇒ `Promise.<boolean>`
  * [.asyncBlockeRemove(params)](doc.md#module\_rosterManage.asyncBlockeRemove) ⇒ `Promise.<boolean>`
  * [.asyncApply(params)](doc.md#module\_rosterManage.asyncApply) ⇒ `Promise.<boolean>`
  * [.asyncAccept(params)](doc.md#module\_rosterManage.asyncAccept) ⇒ `Promise.<boolean>`
  * [.asyncDecline(params)](doc.md#module\_rosterManage.asyncDecline) ⇒ `Promise.<boolean>`
  * [.asyncUpdateRosterExt(params)](doc.md#module\_rosterManage.asyncUpdateRosterExt) ⇒ `Promise.<boolean>`
  * [.asyncSearchRosterByName(params)](doc.md#module\_rosterManage.asyncSearchRosterByName) ⇒ [`Promise.<RosterItem>`](doc.md#module\_types..RosterItem)
  * [.asyncSearchRosterById(params)](doc.md#module\_rosterManage.asyncSearchRosterById) ⇒ [`Promise.<RosterItem>`](doc.md#module\_types..RosterItem)

### rosterManage.asyncGetRosterIdList(force) ⇒ `Promise.<Array.<number>>`

获取好友id列表

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: `Promise.<Array.<number>>` - 用户ID列表

| Param | Type      | Description                               |
| ----- | --------- | ----------------------------------------- |
| force | `boolean` | 是否强制从服务器拉取：true - 从服务器获取， false - 从本地存储获取 |

### rosterManage.asyncGetRosterInfo(roster\_id, force) ⇒ [`Promise.<RosterItem>`](doc.md#module\_types..RosterItem)

获取好友信息

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: [`Promise.<RosterItem>`](doc.md#module\_types..RosterItem) - 好友信息

| Param      | Type      | Description                                  |
| ---------- | --------- | -------------------------------------------- |
| roster\_id | `number`  | 好友ID                                         |
| force      | `boolean` | 是否强制从服务器拉取： true - 从服务器拉取， false - 优先从本地存储获取 |

### rosterManage.asyncRegester(opt) ⇒ [`Promise.<UserSettings>`](doc.md#module\_types..UserSettings)

用户注册

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: [`Promise.<UserSettings>`](doc.md#module\_types..UserSettings) - 用户设置

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| opt          | `object` | 用户信息        |
| opt.username | `string` | 用户名         |
| opt.password | `string` | 密码          |

### rosterManage.asyncDeleteRoster(param) ⇒ `Promise.<boolean>`

删除好友

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: `Promise.<boolean>` - 请求结果

| Param          | Type     | Description |
| -------------- | -------- | ----------- |
| param          | `object` | 参数          |
| param.user\_id | `number` | 好友的用户ID     |

### rosterManage.asnycGetRosterListDetailByIds(roster\_ids) ⇒ `Promise.<Array.<module:types~RosterItem>>`

根据id列表获取用户详细信息

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: `Promise.<Array.<module:types~RosterItem>>` - 用户详细信息列表

| Param       | Type             | Description |
| ----------- | ---------------- | ----------- |
| roster\_ids | `Array.<number>` | 用户ID列表      |

### rosterManage.getAllRosterDetail() ⇒ [`Array.<RosterItem>`](doc.md#module\_types..RosterItem)

获取缓存的所有用户详细信息

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: [`Array.<RosterItem>`](doc.md#module\_types..RosterItem) - 用户详细信息列表\


### rosterManage.asyncGetUserProfile(force) ⇒ [`Promise.<UserProfile>`](doc.md#module\_types..UserProfile)

获取自己的用户信息

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: [`Promise.<UserProfile>`](doc.md#module\_types..UserProfile) - 用户信息

| Param | Type      | Description                                  |
| ----- | --------- | -------------------------------------------- |
| force | `boolean` | 是否强制从服务器拉取： true - 从服务器拉取， false - 优先从本地存储获取 |

### rosterManage.getRosterMessageByRid(uid) ⇒ [`Array.<Meta>`](doc.md#module\_types..Meta)

根据会话ID获取聊天消息

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: [`Array.<Meta>`](doc.md#module\_types..Meta) - 聊天消息列表

| Param | Type     | Description |
| ----- | -------- | ----------- |
| uid   | `number` | 会话ID        |

### rosterManage.readRosterMessage(roster\_id, mid)

修改消息状态为已读

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)

| Param      | Type     | Description |
| ---------- | -------- | ----------- |
| roster\_id | `number` | 会话ID        |
| mid        | `number` | 消息ID        |

### rosterManage.recallMessage(uid, mid)

撤回消息，只能撤回5分钟内的

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)

| Param | Type     | Description |
| ----- | -------- | ----------- |
| uid   | `number` | 会话ID        |
| mid   | `number` | 消息ID        |

### rosterManage.unreadMessage(uid, mid)

设置消息成未读

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)

| Param | Type     | Description |
| ----- | -------- | ----------- |
| uid   | `number` | 会话ID        |
| mid   | `number` | 消息ID        |

### rosterManage.deleteMessage(uid, mid)

删除消息

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)

| Param | Type     | Description |
| ----- | -------- | ----------- |
| uid   | `number` | 会话ID        |
| mid   | `number` | 消息ID        |

### rosterManage.getRosterInfo(rid) ⇒ [`RosterItem`](doc.md#module\_types..RosterItem)

获取好友信息

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: [`RosterItem`](doc.md#module\_types..RosterItem) - 好友信息

| Param | Type     | Description |
| ----- | -------- | ----------- |
| rid   | `number` | 好友ID        |

### rosterManage.getUnreadCount(uid) ⇒ `number`

获取指定会话的未读数

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: `number` - 未读数

| Param | Type     | Description |
| ----- | -------- | ----------- |
| uid   | `number` | 会话IID       |

### rosterManage.asyncGetApplyList(params) ⇒ `Promise.<Array.<module:types~RosterApplication>>`

获取好友申请列表

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: `Promise.<Array.<module:types~RosterApplication>>` - 好友申请列表

| Param         | Type     | Description           |
| ------------- | -------- | --------------------- |
| params        | `object` | 参数                    |
| params.cursor | `number` | 从哪开始获取：可以传空字符串表示从头开始取 |

### rosterManage.asyncGetBlockedlist(params) ⇒ `Promise.<Array.<number>>`

获取黑名单

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: `Promise.<Array.<number>>` - 用户ID列表

| Param  | Type     | Description |
| ------ | -------- | ----------- |
| params | `object` | 参数：空对象      |

### rosterManage.asyncBlockeAdd(params) ⇒ `Promise.<boolean>`

加入黑名单

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param           | Type     | Description |
| --------------- | -------- | ----------- |
| params          | `object` | 参数          |
| params.user\_id | `number` | 用户ID        |

### rosterManage.asyncBlockeRemove(params) ⇒ `Promise.<boolean>`

移除黑名单

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param           | Type     | Description |
| --------------- | -------- | ----------- |
| params          | `object` | 参数          |
| params.user\_id | `number` | 用户ID        |

### rosterManage.asyncApply(params) ⇒ `Promise.<boolean>`

请求加为好友

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param           | Type     | Description |
| --------------- | -------- | ----------- |
| params          | `object` | 参数          |
| params.user\_id | `number` | 用户ID        |
| params.alias    | `string` | 备注          |

### rosterManage.asyncAccept(params) ⇒ `Promise.<boolean>`

通过好友申请

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param           | Type     | Description |
| --------------- | -------- | ----------- |
| params          | `object` | 参数          |
| params.user\_id | `number` | 用户ID        |

### rosterManage.asyncDecline(params) ⇒ `Promise.<boolean>`

拒绝好友申请

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param           | Type     | Description |
| --------------- | -------- | ----------- |
| params          | `object` | 参数          |
| params.user\_id | `number` | 用户ID        |

### rosterManage.asyncUpdateRosterExt(params) ⇒ `Promise.<boolean>`

修改好友扩展字段

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param           | Type     | Description |
| --------------- | -------- | ----------- |
| params          | `object` | 参数          |
| params.user\_id | `number` | 用户ID        |
| params.ext      | `string` | 扩展字段        |

### rosterManage.asyncSearchRosterByName(params) ⇒ [`Promise.<RosterItem>`](doc.md#module\_types..RosterItem)

按名称搜索用户

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: [`Promise.<RosterItem>`](doc.md#module\_types..RosterItem) - 用户信息

| Param           | Type     | Description |
| --------------- | -------- | ----------- |
| params          | `object` | 参数          |
| params.username | `string` | 用户名         |

### rosterManage.asyncSearchRosterById(params) ⇒ [`Promise.<RosterItem>`](doc.md#module\_types..RosterItem)

按ID搜索用户

**Kind**: static method of [`rosterManage`](doc.md#module\_rosterManage)\
**Returns**: [`Promise.<RosterItem>`](doc.md#module\_types..RosterItem) - 用户信息

| Param           | Type     | Description |
| --------------- | -------- | ----------- |
| params          | `object` | 参数          |
| params.user\_id | `number` | 用户ID        |

## sysManage

* [sysManage](doc.md#module\_sysManage)
  * [.sendRosterMessage(msg)](doc.md#module\_sysManage.sendRosterMessage) ⇒ `number`
  * [.sendGroupMessage(msg)](doc.md#module\_sysManage.sendGroupMessage) ⇒ `number`
  * [.requireHistoryMessage(uid, sid, amount)](doc.md#module\_sysManage.requireHistoryMessage)
  * [.sendMentionMessage(params)](doc.md#module\_sysManage.sendMentionMessage) ⇒ `number`
  * [.sendInputStatusMessage(uid, status)](doc.md#module\_sysManage.sendInputStatusMessage) ⇒ `number`
  * [.forwardMessage(param)](doc.md#module\_sysManage.forwardMessage) ⇒ `number`
  * [.getMessageStatus(cid, mid, isGroup)](doc.md#module\_sysManage.getMessageStatus) ⇒ `string`
  * [.asyncFileUpload(param)](doc.md#module\_sysManage.asyncFileUpload) ⇒ [`Promise.<FileUploadResult>`](doc.md#module\_types..FileUploadResult)
  * [.getImage(param)](doc.md#module\_sysManage.getImage) ⇒ `string`
  * [.deleteConversation(id, other\_devices)](doc.md#module\_sysManage.deleteConversation)
  * [.asyncGetGroupAvatarUploadUrl(params)](doc.md#module\_sysManage.asyncGetGroupAvatarUploadUrl) ⇒ [`Promise.<FileUpload>`](doc.md#module\_types..FileUpload)
  * [.asyncGetFileUploadChatFileUrl(params)](doc.md#module\_sysManage.asyncGetFileUploadChatFileUrl) ⇒ [`Promise.<FileUpload>`](doc.md#module\_types..FileUpload)

### sysManage.sendRosterMessage(msg) ⇒ `number`

发送单聊消息

**Kind**: static method of [`sysManage`](doc.md#module\_sysManage)\
**Returns**: `number` - 客户端生成的消息ID

| Param          | Type                 | Description                                                                                              |
| -------------- | -------------------- | -------------------------------------------------------------------------------------------------------- |
| msg            | `object`             | 消息体                                                                                                      |
| msg.uid        | `string`             | 接收者ID                                                                                                    |
| msg.content    | `string`             | 消息内容                                                                                                     |
| msg.type       | `string`             | 消息类型： text - 文本, image - 图片， audio - 语音, video - 视频，file - 文件, location - 位置， command - 命令, forward - 转发 |
| msg.ext        | `string` \| `object` | 扩展字段                                                                                                     |
| msg.attachment | `string` \| `object` | 附件信息                                                                                                     |

### sysManage.sendGroupMessage(msg) ⇒ `number`

发送群聊消息

**Kind**: static method of [`sysManage`](doc.md#module\_sysManage)\
**Returns**: `number` - 客户端生成的消息ID

| Param          | Type                 | Description                                                                                              |
| -------------- | -------------------- | -------------------------------------------------------------------------------------------------------- |
| msg            | `object`             | 发送消息体                                                                                                    |
| msg.gid        | `string`             | 群组ID                                                                                                     |
| msg.content    | `string`             | 消息内容                                                                                                     |
| msg.type       | `string`             | 消息类型： text - 文本, image - 图片， audio - 语音, video - 视频，file - 文件, location - 位置， command - 命令, forward - 转发 |
| msg.ext        | `string` \| `object` | 扩展字段                                                                                                     |
| msg.attachment | `string` \| `object` | 附件信息                                                                                                     |
| msg.priority   | `number`             | 设置消息的扩散优先级，默认为0。0表示扩散，数字越小扩散的越多。                                                                         |

### sysManage.requireHistoryMessage(uid, sid, amount)

请求历史消息

**Kind**: static method of [`sysManage`](doc.md#module\_sysManage)

| Param  | Type     | Description                      |
| ------ | -------- | -------------------------------- |
| uid    | `number` | 会话ID                             |
| sid    | `number` | 消息ID: 从哪个消息向前拉取，传0表示从最新一条消息开始拉取。 |
| amount | `number` | 拉取的条数                            |

### sysManage.sendMentionMessage(params) ⇒ `number`

群发送@消息

**Kind**: static method of [`sysManage`](doc.md#module\_sysManage)\
**Returns**: `number` - 客户端生成的消息ID

| Param                   | Type             | Description |
| ----------------------- | ---------------- | ----------- |
| params                  | `object`         |             |
| params.gid              | `number`         | 群ID         |
| params.txt              | `string`         | 消息文本内容      |
| params.mentionAll       | `boolean`        | 是否@所有人      |
| params.mentionList      | `Array.<number>` | @的成员ID列表    |
| params.mentionedMessage | `string`         | @消息的显示内容    |
| params.mentionedMessage | `string`         | @消息的推送内容    |
| params.senderNickname   | `string`         | 发送者昵称       |

### sysManage.sendInputStatusMessage(uid, status) ⇒ `number`

发送输入状态消息

**Kind**: static method of [`sysManage`](doc.md#module\_sysManage)\
**Returns**: `number` - 客户端生成的消息ID

| Param  | Type     | Description                      |
| ------ | -------- | -------------------------------- |
| uid    | `number` | 会话ID                             |
| status | `string` | 状态： nothing - 未输入， typing - 正在输入 |

### sysManage.forwardMessage(param) ⇒ `number`

转发消息

**Kind**: static method of [`sysManage`](doc.md#module\_sysManage)\
**Returns**: `number` - 客户端生成的消息ID

| Param     | Type     | Description       |
| --------- | -------- | ----------------- |
| param     | `object` | 参数                |
| param.uid | `number` | 接收方用户ID（仅转发单聊时设置） |
| param.gid | `number` | 接收方群组ID（仅转发群聊时设置） |
| param.mid | `number` | 要转发的消息ID          |

### sysManage.getMessageStatus(cid, mid, isGroup) ⇒ `string`

获取消息的状态

**Kind**: static method of [`sysManage`](doc.md#module\_sysManage)\
**Returns**: `string` - 消息状态: unread - 未读， delivered - 已投递， read - 已读

| Param   | Type      | Default | Description |
| ------- | --------- | ------- | ----------- |
| cid     | `number`  |         | 会话ID        |
| mid     | `number`  |         | 消息ID        |
| isGroup | `boolean` | `false` | 是否是群聊       |

### sysManage.asyncFileUpload(param) ⇒ [`Promise.<FileUploadResult>`](doc.md#module\_types..FileUploadResult)

上传文件

**Kind**: static method of [`sysManage`](doc.md#module\_sysManage)\
**Returns**: [`Promise.<FileUploadResult>`](doc.md#module\_types..FileUploadResult) - 文件上传结果

| Param                 | Type                                                             | Description                                                                                                                                                                            |
| --------------------- | ---------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| param                 | `object`                                                         | 参数                                                                                                                                                                                     |
| param.group\_d        | `number`                                                         | 群组ID                                                                                                                                                                                   |
| param.toType          | `number`                                                         | 接收者类型：rosterAvatar - 用户头像， chat - 聊天文件， groupAvatar - 群头像                                                                                                                              |
| param.to\_id          | `number`                                                         | 接收者ID                                                                                                                                                                                  |
| param.file            | `File`                                                           | 文件                                                                                                                                                                                     |
| param.fileType        | `string`                                                         | 文件类型：file - 普通聊天文件, audio - 语音聊天文件(amr格式),image - 图片聊天文件, video - 视频聊天文件, audio-mp3 - 语音聊天文件(mp3格式), shareFile - 普通共享文件, shareAudio - 语音共享文件, shareImage - 图片共享文件, shareVideo - 视频共享文件 |
| param.chatType        | `number`                                                         | 聊天类型： roster - 单聊, group - 群聊                                                                                                                                                          |
| param.processCallback | [`fileUploadProgress`](doc.md#module\_types..fileUploadProgress) | 上传进度回调                                                                                                                                                                                 |

### sysManage.getImage(param) ⇒ `string`

拼装图片路径

**Kind**: static method of [`sysManage`](doc.md#module\_sysManage)\
**Returns**: `string` - 图片地址

| Param           | Type      | Description                |
| --------------- | --------- | -------------------------- |
| param           | `object`  |                            |
| param.avatar    | `string`  | 文件地址                       |
| param.type      | `string`  | 类型： roster - 用户, group - 群 |
| param.thumbnail | `boolean` | 是否缩略图：默认为true              |
| param.sdefault  | `string`  | 默认图片地址                     |

### sysManage.deleteConversation(id, other\_devices)

删除会话

**Kind**: static method of [`sysManage`](doc.md#module\_sysManage)

| Param          | Type      | Default | Description    |
| -------------- | --------- | ------- | -------------- |
| id             | `number`  |         | 会话ID           |
| other\_devices | `boolean` | `true`  | 是否同时删除其它设备上的会话 |

### sysManage.asyncGetGroupAvatarUploadUrl(params) ⇒ [`Promise.<FileUpload>`](doc.md#module\_types..FileUpload)

获取上传群头像URL

**Kind**: static method of [`sysManage`](doc.md#module\_sysManage)\
**Returns**: [`Promise.<FileUpload>`](doc.md#module\_types..FileUpload) - 文件上传信息

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

### sysManage.asyncGetFileUploadChatFileUrl(params) ⇒ [`Promise.<FileUpload>`](doc.md#module\_types..FileUpload)

获取聊天文件上传地址

**Kind**: static method of [`sysManage`](doc.md#module\_sysManage)\
**Returns**: [`Promise.<FileUpload>`](doc.md#module\_types..FileUpload) - 文件上传信息

| Param             | Type     | Description                                                                                                                                   |
| ----------------- | -------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| params            | `object` | 参数                                                                                                                                            |
| params.file\_type | `number` | 文件类型: 100 - 普通聊天文件, 101 - 语音聊天文件(amr格式),102 - 图片聊天文件, 103 - 视频聊天文件, 104 - 语音聊天文件(mp3格式)200 - 普通共享文件, 201 - 语音共享文件, 202 - 图片共享文件, 203 - 视频共享文件 |
| params.to\_type   | `number` | 会话类型： 1 - 用户，2 - 群组                                                                                                                           |
| params.to\_id     | `number` | 会话ID                                                                                                                                          |

## userManage

* [userManage](doc.md#module\_userManage)
  * [.getToken()](doc.md#module\_userManage.getToken) ⇒ `string`
  * [.getUid()](doc.md#module\_userManage.getUid) ⇒ `number`
  * [.getAppid()](doc.md#module\_userManage.getAppid) ⇒ `string`
  * [.getConversationList()](doc.md#module\_userManage.getConversationList) ⇒ [`Array.<ConversationItem>`](doc.md#module\_types..ConversationItem)
  * [.asyncUpdateAvatar(params)](doc.md#module\_userManage.asyncUpdateAvatar) ⇒ `Promise.<boolean>`
  * [.asyncUpdateNickName(params)](doc.md#module\_userManage.asyncUpdateNickName) ⇒ `Promise.<boolean>`
  * [.asyncGetProfile()](doc.md#module\_userManage.asyncGetProfile) ⇒ [`Promise.<UserProfile>`](doc.md#module\_types..UserProfile)
  * [.asyncUpdateProfile(params)](doc.md#module\_userManage.asyncUpdateProfile) ⇒ `Promise.<boolean>`
  * [.asyncGetSettings()](doc.md#module\_userManage.asyncGetSettings) ⇒ [`Promise.<UserSettings>`](doc.md#module\_types..UserSettings)
  * [.asyncUpdateSettings(settings)](doc.md#module\_userManage.asyncUpdateSettings) ⇒ `Promise.<boolean>`

### userManage.getToken() ⇒ `string`

获取登录用户的token

**Kind**: static method of [`userManage`](doc.md#module\_userManage)\
**Returns**: `string` - 用户的token\


### userManage.getUid() ⇒ `number`

获取登录用户的uid

**Kind**: static method of [`userManage`](doc.md#module\_userManage)\
**Returns**: `number` - 用户ID\


### userManage.getAppid() ⇒ `string`

获取appid

**Kind**: static method of [`userManage`](doc.md#module\_userManage)\
**Returns**: `string` - APP ID\


### userManage.getConversationList() ⇒ [`Array.<ConversationItem>`](doc.md#module\_types..ConversationItem)

获取最近会话列表

**Kind**: static method of [`userManage`](doc.md#module\_userManage)\


### userManage.asyncUpdateAvatar(params) ⇒ `Promise.<boolean>`

更新头像

**Kind**: static method of [`userManage`](doc.md#module\_userManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param         | Type     | Description |
| ------------- | -------- | ----------- |
| params        | `object` | 参数          |
| params.avatar | `string` | 头像 url      |

### userManage.asyncUpdateNickName(params) ⇒ `Promise.<boolean>`

更新昵称

**Kind**: static method of [`userManage`](doc.md#module\_userManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param             | Type     | Description |
| ----------------- | -------- | ----------- |
| params            | `object` | 参数          |
| params.nick\_name | `string` | 昵称          |

### userManage.asyncGetProfile() ⇒ [`Promise.<UserProfile>`](doc.md#module\_types..UserProfile)

获取用户profile

**Kind**: static method of [`userManage`](doc.md#module\_userManage)\
**Returns**: [`Promise.<UserProfile>`](doc.md#module\_types..UserProfile) - 用户信息\


### userManage.asyncUpdateProfile(params) ⇒ `Promise.<boolean>`

更新用户profile

**Kind**: static method of [`userManage`](doc.md#module\_userManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param                | Type     | Description   |
| -------------------- | -------- | ------------- |
| params               | `object` |               |
| params.description   | `string` | 描述信息          |
| params.nick\_name    | `string` | 昵称            |
| params.private\_info | `string` | 私有信息，仅自己可见    |
| params.public\_info  | `string` | 公开信息，好友和陌生人可见 |

### userManage.asyncGetSettings() ⇒ [`Promise.<UserSettings>`](doc.md#module\_types..UserSettings)

获取用户设置信息

**Kind**: static method of [`userManage`](doc.md#module\_userManage)\
**Returns**: [`Promise.<UserSettings>`](doc.md#module\_types..UserSettings) - 用户信息\


### userManage.asyncUpdateSettings(settings) ⇒ `Promise.<boolean>`

修改用户设置

**Kind**: static method of [`userManage`](doc.md#module\_userManage)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param    | Type                                                 | Description |
| -------- | ---------------------------------------------------- | ----------- |
| settings | [`UserSettings`](doc.md#module\_types..UserSettings) | 更新的设置       |

## types

* [types](doc.md#module\_types)
  * ["flooNotice" (res)](doc.md#event\_flooNotice)
  * ["flooError" (res)](doc.md#event\_flooError)
  * ["loginFail" (desc)](doc.md#event\_loginFail)
  * ["loginSuccess" (res)](doc.md#event\_loginSuccess)
  * ["onGroupListUpdate" (meta)](doc.md#event\_onGroupListUpdate)
  * ["onGroupMemberChanged" (groupId)](doc.md#event\_onGroupMemberChanged)
  * ["onGroupMessage" (meta)](doc.md#event\_onGroupMessage)
  * ["onInputStatusMessage" (res)](doc.md#event\_onInputStatusMessage)
  * ["onMentionMessage" (meta)](doc.md#event\_onMentionMessage)
  * ["onMessageCanceled" (res)](doc.md#event\_onMessageCanceled)
  * ["onMessageDeleted" (res)](doc.md#event\_onMessageDeleted)
  * ["onMessageRecalled" (res)](doc.md#event\_onMessageRecalled)
  * ["onMessageStatusChanged" (res)](doc.md#event\_onMessageStatusChanged)
  * ["onReceiveHistoryMsg" (res)](doc.md#event\_onReceiveHistoryMsg)
  * ["onRosterInfoUpdate" (res)](doc.md#event\_onRosterInfoUpdate)
  * ["onRosterListUpdate" (meta)](doc.md#event\_onRosterListUpdate)
  * ["onRosterMessage" (meta)](doc.md#event\_onRosterMessage)
  * ["onSendingMessageStatusChanged" (res)](doc.md#event\_onSendingMessageStatusChanged)
  * ["onUnreadChange" (cid)](doc.md#event\_onUnreadChange)
  * ["recentlistUpdate"](doc.md#event\_recentlistUpdate)
  * ["onGroupCreated" (meta)](doc.md#event\_onGroupCreated)
  * ["onGroupDestoryed" (meta)](doc.md#event\_onGroupDestoryed)
  * ["onGroupJoined" (meta)](doc.md#event\_onGroupJoined)
  * ["onGroupApplyAccepted" (meta)](doc.md#event\_onGroupApplyAccepted)
  * ["onGroupApplyDeclined" (meta)](doc.md#event\_onGroupApplyDeclined)
  * ["onGroupBaned" (meta)](doc.md#event\_onGroupBaned)
  * ["onGroupUnbaned" (meta)](doc.md#event\_onGroupUnbaned)
  * [\~RosterItem](doc.md#module\_types..RosterItem) : `object`
  * [\~UserSettings](doc.md#module\_types..UserSettings) : `object`
  * [\~UserProfile](doc.md#module\_types..UserProfile) : `object`
  * [\~Meta](doc.md#module\_types..Meta) : `object`
  * [\~RosterApplication](doc.md#module\_types..RosterApplication) : `object`
  * [\~GroupInfoAndSettings](doc.md#module\_types..GroupInfoAndSettings) : `object`
  * [\~BriefGroupInfoAndSettings](doc.md#module\_types..BriefGroupInfoAndSettings) : `object`
  * [\~GroupMember](doc.md#module\_types..GroupMember) : `object`
  * [\~GroupMemberBanned](doc.md#module\_types..GroupMemberBanned) : `object`
  * [\~GroupUserRelationResponse](doc.md#module\_types..GroupUserRelationResponse) : `object`
  * [\~GroupAnnouncement](doc.md#module\_types..GroupAnnouncement) : `object`
  * [\~GroupInfoRequest](doc.md#module\_types..GroupInfoRequest) : `object`
  * [\~GroupBannedMemberRequest](doc.md#module\_types..GroupBannedMemberRequest) : `object`
  * [\~GroupBlockedListItem](doc.md#module\_types..GroupBlockedListItem) : `object`
  * [\~GroupInvitation](doc.md#module\_types..GroupInvitation) : `object`
  * [\~GroupApplication](doc.md#module\_types..GroupApplication) : `object`
  * [\~GroupSharedFile](doc.md#module\_types..GroupSharedFile) : `object`
  * [\~GroupSharedFileResponse](doc.md#module\_types..GroupSharedFileResponse) : `object`
  * [\~GroupBanAllResponse](doc.md#module\_types..GroupBanAllResponse) : `object`
  * [\~FileUpload](doc.md#module\_types..FileUpload) : `object`
  * [\~FileUploadResult](doc.md#module\_types..FileUploadResult) : `object`
  * [\~fileUploadProgress](doc.md#module\_types..fileUploadProgress) : `function`
  * [\~ConversationItem](doc.md#module\_types..ConversationItem) : `object`
  * [\~UserProfile](doc.md#module\_types..UserProfile) : `object`
  * [\~UserSettings](doc.md#module\_types..UserSettings) : `object`
  * [\~Event](doc.md#module\_types..Event) : `string`
  * [\~EventCallback](doc.md#module\_types..EventCallback) : `function`

### "flooNotice" (res)

Floo通知

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| res          | `object` | 结果          |
| res.category | `string` | 类别          |
| res.desc     | `string` | 描述          |

**Example**

```js
{category: 'loginMessage',desc: 'socket connecting...'} // 开始建连接
{category: 'loginMessage',desc: 'socket connect success...'} // 连接成功
{category: 'loginMessage',desc: 'logining socket service...'} // 开始登录
{category: 'loginMessage',desc: 'login socket failure ......'} // 登录失败
{category: 'loginMessage',desc: 'login socket success.....'} // 登录成功
{category: 'loginMessage', desc: 'getting token...' } //获取token
{category: 'loginMessage',desc: 'token sucecc, getting roster lists..'} // 获取token成功，开始获取好友列表
{category: 'loginMessage',desc: 'get roster list failure:' + ex.message} // 获取好友列表失败
{category: 'action', desc: 'relogin' } // 需要自动登录
{category: 'action', desc: 'relogin_manually' }  // 需要手动登录
{category: 'conversation_deleted',desc: { id, source:'user_operation' }} // 会话被删除。ID：会话ID， source: 来源
{category: 'userNotice', desc:'PASSWORD_CHANGED'} // 用户密码改变
{category: 'userNotice', desc:'FROZEN'} // 用户账户被封禁
{category: 'userNotice', desc:'REMOVED'} // 用户被删除
{category: 'userNotice', desc:'KICK_BY_SAME_DEVICE'} // 当前设备被相同设备踢下线
{category: 'userNotice', desc:'KICKED_BY_OTHER_DEVICE'} // 当前设备被其它设备踢下线
{category: 'userNotice', desc:'INFO_UPDATED'} // 用户信息改变：profile或setting
{category: 'userNotice', desc:'DEVICE_LOGIN'} // 用户其它设备上线
{category: 'userNotice', desc:'DEVICE_LOGOUT'} // 用户其它设备下线
{category: 'userNotice', desc:'DEVICE_ADDED'} // 新设备通知
{category: 'userNotice', desc:'DEVICE_REMOVED'} // 设备被移除的通知
{category: 'userNotice', desc:'CLUSTER_CHANGED'} // 用户所在集群改变 需要重新登录
```

### "flooError" (res)

Floo错误

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| res          | `object` |             |
| res.category | `string` | 类别          |
| res.desc     | `string` | 描述          |

**Example**

```js
{category: 'USER_BANNED', desc:'用户被禁言'}
{category: 'USER_FROZEN', desc:'用户被冻结，请联系App管理员。'}
{category: 'APP_FROZEN', desc:'APP 被冻结，请登陆美信拓扑控制台查看详情。'}
{category: 'LICENSE', desc:'无效 LICENSE，请确认服务已按时付费。'}
{category: 'LICENSE', desc:'超出 LICENSE 用户数限制，请购买更高规格服务。'}
{category: 'DNS_FAILED', desc: dnsServer } // DNS错误: 无法访问
```

### "loginFail" (desc)

登录失败

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param | Type     | Description |
| ----- | -------- | ----------- |
| desc  | `string` | 失败原因        |

### "loginSuccess" (res)

登录成功

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param | Type     | Description |
| ----- | -------- | ----------- |
| res   | `object` | 空对象         |

### "onGroupListUpdate" (meta)

群列表更新

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param | Type                                                | Description |
| ----- | --------------------------------------------------- | ----------- |
| meta  | [`Meta`](doc.md#module\_types..Meta) \| `undefined` | 通知消息内容      |

### "onGroupMemberChanged" (groupId)

群成员列表更新

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param   | Type     | Description |
| ------- | -------- | ----------- |
| groupId | `number` | 群ID         |

### "onGroupMessage" (meta)

收到群消息

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param | Type                                 | Description |
| ----- | ------------------------------------ | ----------- |
| meta  | [`Meta`](doc.md#module\_types..Meta) | 消息内容        |

### "onInputStatusMessage" (res)

对方正在输入

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param    | Type     | Description |
| -------- | -------- | ----------- |
| res      | `object` |             |
| res.ext  | `string` | 扩展字段        |
| res.from | `string` | 发送者用户ID     |
| res.to   | `string` | 接收者用户ID     |

### "onMentionMessage" (meta)

收到群组@消息

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param | Type                                 | Description |
| ----- | ------------------------------------ | ----------- |
| meta  | [`Meta`](doc.md#module\_types..Meta) | 消息内容        |

### "onMessageCanceled" (res)

消息被取消已读

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param   | Type     | Description |
| ------- | -------- | ----------- |
| res     | `object` |             |
| res.uid | `string` | 会话ID        |
| res.mid | `string` | 消息ID        |

### "onMessageDeleted" (res)

消息被删除

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param   | Type     | Description |
| ------- | -------- | ----------- |
| res     | `object` |             |
| res.uid | `string` | 会话ID        |
| res.mid | `string` | 消息ID        |

### "onMessageRecalled" (res)

消息被撤回

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param   | Type     | Description |
| ------- | -------- | ----------- |
| res     | `object` |             |
| res.uid | `string` | 会话ID        |
| res.mid | `string` | 消息ID        |

### "onMessageStatusChanged" (res)

消息状态变更：撤回/删除/已读

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param   | Type     | Description |
| ------- | -------- | ----------- |
| res     | `object` |             |
| res.uid | `string` | 会话ID        |
| res.mid | `string` | 消息ID        |

### "onReceiveHistoryMsg" (res)

收到历史消息

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param    | Type     | Description |
| -------- | -------- | ----------- |
| res      | `object` |             |
| res.next | `number` | 下次取历史消息的key |

### "onRosterInfoUpdate" (res)

好友信息变更

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param         | Type             | Description |
| ------------- | ---------------- | ----------- |
| res           | `object`         |             |
| res.rosterIds | `Array.<number>` | 好友的用户ID列表   |

### "onRosterListUpdate" (meta)

好友列表变更

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param | Type                                 | Description |
| ----- | ------------------------------------ | ----------- |
| meta  | [`Meta`](doc.md#module\_types..Meta) | 好友通知的消息内容   |

### "onRosterMessage" (meta)

收到单聊消息

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param | Type                                 | Description |
| ----- | ------------------------------------ | ----------- |
| meta  | [`Meta`](doc.md#module\_types..Meta) | 消息内容        |

### "onSendingMessageStatusChanged" (res)

消息发送状态变更

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param       | Type     | Description       |
| ----------- | -------- | ----------------- |
| res         | `object` |                   |
| res.status: | `number` | 发送状态，取值为sending   |
| res.mid:    | `number` | 客户端生成的client\_mid |

### "onUnreadChange" (cid)

未读数改变

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param | Type     | Description |
| ----- | -------- | ----------- |
| cid   | `number` | 会话ID        |

### "recentlistUpdate"

最近会话更新

**Kind**: event emitted by [`types`](doc.md#module\_types)\


### "onGroupCreated" (meta)

群组创建通知

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param | Type                                 | Description |
| ----- | ------------------------------------ | ----------- |
| meta  | [`Meta`](doc.md#module\_types..Meta) | 群通知的消息内容    |

### "onGroupDestoryed" (meta)

群组解散通知

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param | Type                                 | Description |
| ----- | ------------------------------------ | ----------- |
| meta  | [`Meta`](doc.md#module\_types..Meta) | 群通知的消息内容    |

### "onGroupJoined" (meta)

成员入群通知

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param | Type                                 | Description |
| ----- | ------------------------------------ | ----------- |
| meta  | [`Meta`](doc.md#module\_types..Meta) | 群通知的消息内容    |

### "onGroupApplyAccepted" (meta)

群申请被通过

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param | Type                                 | Description |
| ----- | ------------------------------------ | ----------- |
| meta  | [`Meta`](doc.md#module\_types..Meta) | 群通知的消息内容    |

### "onGroupApplyDeclined" (meta)

群申请被拒绝

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param | Type                                 | Description |
| ----- | ------------------------------------ | ----------- |
| meta  | [`Meta`](doc.md#module\_types..Meta) | 群通知的消息内容    |

### "onGroupBaned" (meta)

被群禁言

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param | Type                                 | Description |
| ----- | ------------------------------------ | ----------- |
| meta  | [`Meta`](doc.md#module\_types..Meta) | 群通知的消息内容    |

### "onGroupUnbaned" (meta)

被群取消禁言

**Kind**: event emitted by [`types`](doc.md#module\_types)

| Param | Type                                 | Description |
| ----- | ------------------------------------ | ----------- |
| meta  | [`Meta`](doc.md#module\_types..Meta) | 群通知的消息内容    |

### types\~RosterItem : `object`

好友信息

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name               | Type      | Description                                                                       |
| ------------------ | --------- | --------------------------------------------------------------------------------- |
| alias              | `string`  | 别名                                                                                |
| auth\_mode         | `number`  | 验证方式, 0 - 无需验证，任何人可以加为好友, 1 - 需要同意方可加为好友, 2 - 需要回答问题正确方可加为好友, 3 - 拒绝所有加好友申请,int32 |
| auth\_question     | `string`  | 验证问题                                                                              |
| avatar             | `string`  | 头像                                                                                |
| description        | `string`  | 描述信息                                                                              |
| ext                | `string`  | 扩展信息                                                                              |
| mute\_notification | `boolean` | 是否接收消息提醒                                                                          |
| nick\_name         | `string`  | 昵称或名称                                                                             |
| public\_info       | `string`  | 公开信息，好友和陌生人可见                                                                     |
| relation           | `number`  | 关系: 0 - 好友，1 - 被删除，2 - 陌生人, int32                                                 |
| user\_id           | `number`  | 好友用户ID,int64                                                                      |
| username           | `string`  | 用户名                                                                               |

### types\~UserSettings : `object`

用户设置信息

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name                  | Type      | Description                                                                       |
| --------------------- | --------- | --------------------------------------------------------------------------------- |
| auth\_answer          | `string`  | 验证问题答案                                                                            |
| auth\_mode            | `number`  | 验证方式, 0 - 无需验证，任何人可以加为好友, 1 - 需要同意方可加为好友, 2 - 需要回答问题正确方可加为好友, 3 - 拒绝所有加好友申请,int32 |
| auth\_question        | `string`  | 验证问题                                                                              |
| auto\_download        | `boolean` | 是否自动下载                                                                            |
| group\_confirm        | `boolean` | 邀请入群时是否需要用户确认: true - 需要用户同意才可加入， false - 自动同意邀请                                  |
| id                    | `number`  | 用户ID, int64                                                                       |
| no\_push              | `boolean` | 是否关闭推送消息                                                                          |
| no\_push\_detail      | `boolean` | 是否推送详情                                                                            |
| no\_push\_end\_hour   | `number`  | 推送免打扰结束时间,int32                                                                   |
| no\_push\_start\_hour | `number`  | 推送免打扰开始时间,int32                                                                   |
| no\_sounds            | `boolean` | 收到消息时是否静音                                                                         |
| push\_nick\_name      | `string`  | 推送昵称                                                                              |
| push\_token           | `string`  | 推送token                                                                           |
| silence\_end\_time    | `number`  | 推送不提醒结束时间,int32                                                                   |
| silence\_start\_time  | `number`  | 推送不提醒开始时间,int32                                                                   |
| user\_id              | `number`  | 用户ID,int64                                                                        |
| vibratory             | `boolean` | 收到消息时否振动                                                                          |

### types\~UserProfile : `object`

用户信息

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name          | Type     | Description   |
| ------------- | -------- | ------------- |
| avatar        | `string` | 头像 url        |
| description   | `string` | 描述信息          |
| email         | `string` | 邮箱            |
| mobile        | `string` | 手机号码          |
| nick\_name    | `string` | 昵称            |
| private\_info | `string` | 私有信息，仅自己可见    |
| public\_info  | `string` | 公开信息，好友和陌生人可见 |
| user\_id      | `number` | 用户ID,int64    |
| username      | `string` | 用户名           |

### types\~Meta : `object`

消息体

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name      | Type                 | Description                                                                                              |
| --------- | -------------------- | -------------------------------------------------------------------------------------------------------- |
| id        | `string`             | 消息ID                                                                                                     |
| from      | `string`             | 发送者                                                                                                      |
| to        | `string`             | 接收者                                                                                                      |
| content   | `string`             | 消息内容                                                                                                     |
| type      | `string`             | 消息类型： text - 文本, image - 图片， audio - 语音, video - 视频，file - 文件, location - 位置， command - 命令, forward - 转发 |
| ext       | `string` \| `object` | 扩展字段                                                                                                     |
| config    | `string` \| `object` | SDK扩展字段                                                                                                  |
| attach    | `string` \| `object` | 附件信息                                                                                                     |
| status    | `number`             | 消息状态： 0 - 未读, 1 - 已投递, 2 - 已读                                                                            |
| timestamp | `string`             | 消息发送时间戳（毫秒）                                                                                              |
| toType    | `string`             | 接收者类型： roster - 好友， group - 群组                                                                           |

### types\~RosterApplication : `object`

加好友申请列表项

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name          | Type     | Description                         |
| ------------- | -------- | ----------------------------------- |
| expired\_time | `number` | 过期时间,int64                          |
| reason        | `string` | 申请描述                                |
| status        | `number` | 状态： 0 - 等待确认， 1 - 接受， 2 - 拒绝。 int32 |
| user\_id      | `number` | 发起加好友申请的用户ID,int64                  |

### types\~GroupInfoAndSettings : `object`

群信息

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name              | Type      | Description                                                                |
| ----------------- | --------- | -------------------------------------------------------------------------- |
| apply\_approval   | `number`  | 入群申请审批设置, 0:同意所有申请 1:需要管理员确认 2:拒绝所有申请                                      |
| avatar            | `string`  | 群头像                                                                        |
| ban\_expire\_time | `number`  | 全员禁言过期时间（秒），禁言期间只允许管理员发消息， 为0或小于当前时间表示不禁言, -1表示永久禁言                        |
| created\_at       | `number`  | 创建时间                                                                       |
| description       | `string`  | 群描述                                                                        |
| ext               | `string`  | 群扩展信息                                                                      |
| group\_id         | `number`  | 群id,int64                                                                  |
| history\_visible  | `boolean` | 新成员可见历史聊天记录设置                                                              |
| member\_invite    | `boolean` | 群成员邀请设置: false - 不允许邀请, true - 允许邀请(默认)                                    |
| member\_modify    | `boolean` | 群成员修改群信息设置: false - 群成员不能修改群信息(默认), true - 群成员可以修改群信息                      |
| msg\_mute\_mode   | `number`  | 群消息屏蔽模式: 0 - 表示不屏蔽, 1 - 表示屏蔽本地消息通知, 2 - 表示屏蔽消息，不接收消息                       |
| msg\_push\_mode   | `number`  | 群消息推送模式：0 - 接收所有推送，1 - 不接受推送，2 - 接收管理员和@消息推送， 3 - 只接收管理员消息推送， 4 - 只接收@消息推送 |
| name              | `string`  | 群名称                                                                        |
| owner\_id         | `number`  | 群主id,int64                                                                 |
| read\_ack         | `boolean` | 群消息已读功能设置                                                                  |
| status            | `number`  | 群状态, 0：正常, 1：已解散                                                           |
| type              | `number`  | 群类型: 1表示公开群，0表示私有群, 2表示聊天室                                                 |
| updated\_at       | `number`  | 更新时间,int64                                                                 |
| count             | `number`  | 群成员数                                                                       |
| capacity          | `number`  | 群容量                                                                        |

### types\~BriefGroupInfoAndSettings : `object`

群简要信息及用户设置

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name            | Type     | Description                                                                |
| --------------- | -------- | -------------------------------------------------------------------------- |
| apply\_approval | `number` | 入群申请审批设置, 0:同意所有申请 1:需要管理员确认 2:拒绝所有申请                                      |
| avatar          | `string` | 群头像                                                                        |
| capacity        | `number` | 群容量                                                                        |
| count           | `number` | 群成员数                                                                       |
| group\_id       | `number` | 群id,int64                                                                  |
| msg\_mute\_mode | `number` | 群消息屏蔽模式: 0 - 表示不屏蔽, 1 - 表示屏蔽本地消息通知, 2 - 表示屏蔽消息，不接收消息                       |
| msg\_push\_mode | `number` | 群消息推送模式：0 - 接收所有推送，1 - 不接受推送，2 - 接收管理员和@消息推送， 3 - 只接收管理员消息推送， 4 - 只接收@消息推送 |
| name            | `string` | 群名称                                                                        |
| owner           | `number` | 群主id,int64                                                                 |
| status          | `number` | 群状态, 0：正常, 1：已解散,int32                                                     |
| type            | `number` | 群类型: 1表示公开群，0表示私有群, 2表示聊天室。int32                                           |

### types\~GroupMember : `object`

群成员格式

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name          | Type     | Description  |
| ------------- | -------- | ------------ |
| display\_name | `string` | 成员群名片        |
| join\_time    | `number` | 成员入群时间,int64 |
| user\_id      | `number` | 用户id,int64   |
| avatar        | `string` | 头像地址         |

### types\~GroupMemberBanned : `object`

禁言成员

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name          | Type     | Description  |
| ------------- | -------- | ------------ |
| display\_name | `string` | 成员群名片        |
| join\_time    | `number` | 成员入群时间,int64 |
| user\_id      | `number` | 用户id,int64   |
| avatar        | `string` | 头像地址         |
| expired\_time | `number` | 禁言过期时间       |

### types\~GroupUserRelationResponse : `object`

群用户请求结果

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name     | Type     | Description |
| -------- | -------- | ----------- |
| reason   | `string` | 原因          |
| result   | `string` | 结果          |
| user\_id | `number` | 用户ID，int64  |

### types\~GroupAnnouncement : `object`

群公告内容

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name        | Type     | Description  |
| ----------- | -------- | ------------ |
| author      | `number` | 公告发布者,int64  |
| content     | `string` | 公告内容         |
| created\_at | `number` | 公告发布时间,int64 |
| group\_id   | `number` | 群id,int64    |
| id          | `number` | 公告id,int64   |
| title       | `string` | 公告标题         |

### types\~GroupInfoRequest : `object`

创建群

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name        | Type             | Description                     |
| ----------- | ---------------- | ------------------------------- |
| avatar      | `string`         | 群头像                             |
| description | `string`         | 群描述                             |
| name        | `string`         | 群名称                             |
| type        | `number`         | 群类型 1表示公开群，0表示私有群, 2表示聊天室,int32 |
| user\_list  | `Array.<number>` | 邀请入群的用户id列表                     |

### types\~GroupBannedMemberRequest : `object`

禁言请求

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name       | Type             | Description      |
| ---------- | ---------------- | ---------------- |
| duration   | `number`         | 禁言时长，单位为分钟,int64 |
| group\_id  | `number`         | 群id,int64        |
| user\_list | `Array.<number>` | 用户id列表           |

### types\~GroupBlockedListItem : `object`

群组黑名单

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name       | Type     | Description |
| ---------- | -------- | ----------- |
| user\_id   | `number` | 用户id,int64  |
| group\_id  | `number` | 群id,int64   |
| create\_at | `string` | 创建时间        |

### types\~GroupInvitation : `object`

群组邀请信息

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name         | Type     | Description                   |
| ------------ | -------- | ----------------------------- |
| group\_id    | `number` | 群ID                           |
| inviter\_id  | `number` | 邀请者ID                         |
| invitee\_id  | `number` | 被邀请者ID                        |
| reason       | `string` | 原因                            |
| status       | `number` | 状态： 0 - 待处理，1 - 用户同意，2 - 用户拒绝 |
| expire\_time | `number` | 过期时间                          |
| create\_at   | `string` | 创建时间                          |

### types\~GroupApplication : `object`

群申请信息

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name          | Type     | Description               |
| ------------- | -------- | ------------------------- |
| group\_id     | `number` | 群ID                       |
| applicant\_id | `number` | 申请者ID                     |
| reason        | `string` | 原因                        |
| expire\_time  | `number` | 过期时间                      |
| status        | `number` | 状态： 0 - 待处理，1 - 同意，2 - 拒绝 |

### types\~GroupSharedFile : `object`

群共享文件返回格式

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name        | Type     | Description   |
| ----------- | -------- | ------------- |
| created\_at | `number` | int64         |
| file\_id    | `number` | 共享文件id,int64  |
| group\_id   | `number` | 群id,int64     |
| name        | `string` | 共享文件名称        |
| size        | `number` | 共享文件大小,int64  |
| type        | `string` | 共享文件类型        |
| updated\_at | `number` | int64         |
| uploader    | `number` | 共享文件上传者,int64 |
| url         | `string` | 共享文件url       |

### types\~GroupSharedFileResponse : `object`

删除群共享文件结果

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name     | Type     | Description |
| -------- | -------- | ----------- |
| file\_id | `number` | 文件ID        |
| reason   | `string` | 原因          |
| result   | `string` | 结果          |

### types\~GroupBanAllResponse : `object`

全员禁言结果

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name              | Type     | Description    |
| ----------------- | -------- | -------------- |
| ban\_expire\_time | `number` | 全员禁言过期时间,int64 |

### types\~FileUpload : `object`

文件上传信息

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name             | Type                      | Description |
| ---------------- | ------------------------- | ----------- |
| download\_url    | `string`                  | 下载地址        |
| oss\_body\_param | `object.<string, string>` | 额外参数        |
| upload\_url      | `string`                  | 上传地址        |

### types\~FileUploadResult : `object`

文件上传结果

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name | Type     | Description |
| ---- | -------- | ----------- |
| url  | `string` | 下载地址        |

### types\~fileUploadProgress : `function`

文件上传进度回调

**Kind**: inner typedef of [`types`](doc.md#module\_types)

| Param      | Type     | Description |
| ---------- | -------- | ----------- |
| res        | `object` | 进度          |
| res.loaded | `number` | 已下载字节数      |
| res.total  | `number` | 总字节数        |

### types\~ConversationItem : `object`

会话信息

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name      | Type     | Description                   |
| --------- | -------- | ----------------------------- |
| id        | `number` | 会话ID                          |
| content   | `string` | 消息内容                          |
| timestamp | `string` | 消息发送时间戳（毫秒）                   |
| type      | `string` | 会话类型： roster - 单聊， group - 群聊 |

### types\~UserProfile : `object`

用户信息

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name          | Type     | Description   |
| ------------- | -------- | ------------- |
| avatar        | `string` | 头像 url        |
| description   | `string` | 描述信息          |
| email         | `string` | 邮箱            |
| mobile        | `string` | 手机号码          |
| nick\_name    | `string` | 昵称            |
| private\_info | `string` | 私有信息，仅自己可见    |
| public\_info  | `string` | 公开信息，好友和陌生人可见 |
| user\_id      | `number` | 用户ID,int64    |
| username      | `string` | 用户名           |

### types\~UserSettings : `object`

用户设置信息

**Kind**: inner typedef of [`types`](doc.md#module\_types)\
**Properties**

| Name                  | Type      | Description                                                                       |
| --------------------- | --------- | --------------------------------------------------------------------------------- |
| auth\_answer          | `string`  | 验证问题答案                                                                            |
| auth\_mode            | `number`  | 验证方式, 0 - 无需验证，任何人可以加为好友, 1 - 需要同意方可加为好友, 2 - 需要回答问题正确方可加为好友, 3 - 拒绝所有加好友申请,int32 |
| auth\_question        | `string`  | 验证问题                                                                              |
| auto\_download        | `boolean` | 是否自动下载                                                                            |
| group\_confirm        | `boolean` | 邀请入群时是否需要用户确认: true - 需要用户同意才可加入， false - 自动同意邀请                                  |
| id                    | `number`  | 设置ID                                                                              |
| no\_push              | `boolean` | 是否关闭推送消息                                                                          |
| no\_push\_detail      | `boolean` | 是否推送详情                                                                            |
| no\_push\_end\_hour   | `number`  | 推送免打扰结束时间,int32                                                                   |
| no\_push\_start\_hour | `number`  | 推送免打扰开始时间,int32                                                                   |
| no\_sounds            | `boolean` | 收到消息时是否静音                                                                         |
| push\_nick\_name      | `string`  | 推送昵称                                                                              |
| push\_token           | `string`  | 推送token                                                                           |
| silence\_end\_time    | `number`  | 推送不提醒结束时间,int32                                                                   |
| silence\_start\_time  | `number`  | 推送不提醒开始时间,int32                                                                   |
| user\_id              | `number`  | 用户ID,int64                                                                        |
| vibratory             | `boolean` | 收到消息时否振动                                                                          |

### types\~Event : `string`

监听事件名称

**Kind**: inner typedef of [`types`](doc.md#module\_types)\


### types\~EventCallback : `function`

监听事件回调

**Kind**: inner typedef of [`types`](doc.md#module\_types)

| Param | Type                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | Description |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------- |
| res   | [`flooNotice`](doc.md#event\_flooNotice) \| [`flooError`](doc.md#event\_flooError) \| [`loginFail`](doc.md#event\_loginFail) \| [`loginSuccess`](doc.md#event\_loginSuccess) \| [`onGroupListUpdate`](doc.md#event\_onGroupListUpdate) \| [`onGroupMemberChanged`](doc.md#event\_onGroupMemberChanged) \| [`onGroupMessage`](doc.md#event\_onGroupMessage) \| [`onInputStatusMessage`](doc.md#event\_onInputStatusMessage) \| [`onMentionMessage`](doc.md#event\_onMentionMessage) \| [`onMessageCanceled`](doc.md#event\_onMessageCanceled) \| [`onMessageDeleted`](doc.md#event\_onMessageDeleted) \| [`onMessageRecalled`](doc.md#event\_onMessageRecalled) \| [`onMessageStatusChanged`](doc.md#event\_onMessageStatusChanged) \| [`onReceiveHistoryMsg`](doc.md#event\_onReceiveHistoryMsg) \| [`onRosterInfoUpdate`](doc.md#event\_onRosterInfoUpdate) \| [`onRosterListUpdate`](doc.md#event\_onRosterListUpdate) \| [`onRosterMessage`](doc.md#event\_onRosterMessage) \| [`onSendingMessageStatusChanged`](doc.md#event\_onSendingMessageStatusChanged) \| [`onUnreadChange`](doc.md#event\_onUnreadChange) \| [`recentlistUpdate`](doc.md#event\_recentlistUpdate) \| [`onGroupCreated`](doc.md#event\_onGroupCreated) \| [`onGroupDestoryed`](doc.md#event\_onGroupDestoryed) \| [`onGroupJoined`](doc.md#event\_onGroupJoined) \| [`onGroupApplyAccepted`](doc.md#event\_onGroupApplyAccepted) \| [`onGroupApplyDeclined`](doc.md#event\_onGroupApplyDeclined) \| [`onGroupBaned`](doc.md#event\_onGroupBaned) \| [`onGroupUnbaned`](doc.md#event\_onGroupUnbaned) | 事件结果        |

## flooim

* [flooim](doc.md#module\_flooim)
  * [.flooim(config)](doc.md#module\_flooim.flooim) ⇒ `object`
  * [.login(opt)](doc.md#module\_flooim.login)
  * [.qrlogin(opt)](doc.md#module\_flooim.qrlogin)
  * [.tokenLogin(opt)](doc.md#module\_flooim.tokenLogin)
  * [.idLogin(opt)](doc.md#module\_flooim.idLogin)
  * [.isLogin()](doc.md#module\_flooim.isLogin) ⇒ `boolean`
  * [.on(options, ext)](doc.md#module\_flooim.on)
  * [.off(options, ext)](doc.md#module\_flooim.off)
  * [.logout()](doc.md#module\_flooim.logout)

### flooim.flooim(config) ⇒ `object`

初始化SDK

**Kind**: static method of [`flooim`](doc.md#module\_flooim)\
**Returns**: `object` - flooim对象

| Param            | Type                    | Description                                                      |
| ---------------- | ----------------------- | ---------------------------------------------------------------- |
| config           | `object`                | SDK初始化设置                                                         |
| config.appid     | `string`                | APPID                                                            |
| config.ws        | `boolean`               | 连接地址前缀是否为ws/wss: true - 连接地址前缀为ws或wss, false - 连接地址前缀为http/https |
| config.autoLogin | `boolean`               | 是否自动登录                                                           |
| config.dnsServer | `string` \| `undefined` | DNS服务器地址， 可以不设置，默认为 https://dns.maximtop.com/v2/app\_dns         |

**Example**

```js
const config = {
// dnsServer: "https://dns.maximtop.com/v2/app_dns",
appid: "YOUR_APP_ID",
ws: false,
autoLogin: true
};
import flooim from 'floo-2.0.0';
const im = flooim(config);
```

### flooim.login(opt)

登录

**Kind**: static method of [`flooim`](doc.md#module\_flooim)

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| opt          | `object` |             |
| opt.name     | `string` | 用户名         |
| opt.password | `string` | 密码          |

### flooim.qrlogin(opt)

二维码登录

**Kind**: static method of [`flooim`](doc.md#module\_flooim)

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| opt          | `object` |             |
| opt.user\_id | `number` | 用户ID        |
| opt.password | `string` | 密码          |

### flooim.tokenLogin(opt)

token登录

**Kind**: static method of [`flooim`](doc.md#module\_flooim)

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| opt          | `object` |             |
| opt.user\_id | `number` | 用户ID        |
| opt.token    | `string` | Token       |

### flooim.idLogin(opt)

使用用户ID和密码登录

**Kind**: static method of [`flooim`](doc.md#module\_flooim)

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| opt          | `object` |             |
| opt.user\_id | `number` | 用户ID        |
| opt.password | `string` | 密码          |

### flooim.isLogin() ⇒ `boolean`

是否已登录

**Kind**: static method of [`flooim`](doc.md#module\_flooim)\
**Returns**: `boolean` - 是否已登录\


### flooim.on(options, ext)

事件监听

**Kind**: static method of [`flooim`](doc.md#module\_flooim)

| Param   | Type                                                                                                      | Description             |
| ------- | --------------------------------------------------------------------------------------------------------- | ----------------------- |
| options | [`Event`](doc.md#module\_types..Event) \| `Object.<module:types`~~`Event, module:types`~~`EventCallback>` | 可以为事件名，也可以为事件名和事件回调     |
| ext     | [`EventCallback`](doc.md#module\_types..EventCallback) \| `undefined`                                     | 事件回调，只有options为事件名时需要设置 |

**Example**

```js
const im = flooim(config);
im.on('event', (ret) => {
   //do something with ret
 })
 // or
im.on({
   eventName: (ret) => {
     //do something with ret
   },
   ...
 })
```

### flooim.off(options, ext)

取消监听

**Kind**: static method of [`flooim`](doc.md#module\_flooim)

| Param   | Type                                                                                                      | Description             |
| ------- | --------------------------------------------------------------------------------------------------------- | ----------------------- |
| options | [`Event`](doc.md#module\_types..Event) \| `Object.<module:types`~~`Event, module:types`~~`EventCallback>` | 可以为事件名，也可以为事件名和事件回调     |
| ext     | [`EventCallback`](doc.md#module\_types..EventCallback) \| `undefined`                                     | 事件回调，只有options为事件名时需要设置 |

**Example**

```js
const im = flooim(config);
 im.off('events', (ret) => {
   //do something with ret
 })
 // or
 im.off({
   eventName: (ret) => {
     //do something with ret
   },
 ...
 })
```

### flooim.logout()

退出账户

**Kind**: static method of [`flooim`](doc.md#module\_flooim)
