# doc.md

### Modules

[groupManage](broken-reference)

群管理

[rosterManage](broken-reference)

好友管理

[sysManage](broken-reference)[userManage](broken-reference)[types](broken-reference)[flooim](broken-reference)

### groupManage <a href="#module_groupmanage" id="module_groupmanage"></a>

群管理

* [groupManage](broken-reference)
  * [.asyncGetGroupInfo(group\_id, froce)](broken-reference) ⇒ [`Promise.<GroupInfoAndSettings>`](broken-reference)
  * [.asyncGetJoinedGroups(froce)](broken-reference) ⇒ `Promise.<Array.<number>>`
  * [.openGroup(group\_id)](broken-reference)
  * [.getAllGroupDetail()](broken-reference) ⇒ `Object.<number, module:types~GroupInfoAndSettings>`
  * [.asyncGetGroupMembers(group\_id)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupMember>>`
  * [.getGroupMembers(group\_id)](broken-reference) ⇒ [`Array.<GroupMember>`](broken-reference)
  * [.asyncGetGroupListDetail(gids)](broken-reference) ⇒ `Promise.<Array.<module:types~BriefGroupInfoAndSettings>>`
  * [.getGruopMessage(gid)](broken-reference) ⇒ [`Array.<Meta>`](broken-reference)
  * [.asyncGetInfo(params)](broken-reference) ⇒ [`Promise.<GroupInfoAndSettings>`](broken-reference)
  * [.asyncGetMemberList(param)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupMember>>`
  * [.readGroupMessage(group\_id, mid)](broken-reference)
  * [.recallMessage(uid, mid)](broken-reference)
  * [.getUnreadCount(gid)](broken-reference) ⇒ `number`
  * [.asyncGetAdminList(params)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupMember>>`
  * [.asyncAdminAdd(params)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`
  * [.asyncAdminRemove(params)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`
  * [.asyncGetAnouncementById(params)](broken-reference) ⇒ [`Promise.<GroupAnnouncement>`](broken-reference)
  * [.asyncAnouncementDelete(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncAnnouncementEdit(params)](broken-reference) ⇒ [`Promise.<GroupAnnouncement>`](broken-reference)
  * [.asyncGetAnnouncementList(params)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupAnnouncement>>`
  * [.asyncCreate(params)](broken-reference) ⇒ [`Promise.<GroupInfoAndSettings>`](broken-reference)
  * [.asyncDestroy(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncUpdateAvatar(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncUpdateDescription(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncUpdateExt(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncUpdateName(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncGroupMsgMutemode(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncGroupBannedList(params)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupMemberBanned>>`
  * [.asyncGroupBab(params)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`
  * [.asyncGroupUnban(params)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`
  * [.asyncGetSettings(group\_id)](broken-reference) ⇒ [`Promise.<GroupInfoAndSettings>`](broken-reference)
  * [.asyncUpdateAllowMemberInvitation(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncUpdateAllowMemberModify(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncUpdateEnableReadack(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncUpdateHistoryVisible(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncUpdateRequireadminapproval(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncBanAll(params)](broken-reference) ⇒ [`Promise.<GroupBanAllResponse>`](broken-reference)
  * [.asyncUnBanAll(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncOwnerTransfer(params)](broken-reference) ⇒ [`Promise.<GroupUserRelationResponse>`](broken-reference)
  * [.asyncGetUserJoined(params)](broken-reference) ⇒ `Promise.<Array.<number>>`
  * [.asyncApply(params)](broken-reference) ⇒ [`Promise.<GroupUserRelationResponse>`](broken-reference)
  * [.asyncApplyHandle(params)](broken-reference) ⇒ [`Promise.<GroupUserRelationResponse>`](broken-reference)
  * [.asyncGroupBockedlist(params)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupBlockedListItem>>`
  * [.asyncGroupBlock(params)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`
  * [.asyncGroupUnblock(params)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`
  * [.asyncKick(params)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`
  * [.asyncGetInvitationList()](broken-reference) ⇒ `Promise.<Array.<module:types~GroupInvitation>>`
  * [.asyncInvite(params)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>`
  * [.asyncInviteHandle(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncGetMemberDisplayName(params)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupMember>>`
  * [.asyncLeave(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncUpdateDisplayName(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asncGetApplicationList(params)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupApplication>>`
  * [.asyncGetFileList(params)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupSharedFile>>`
  * [.asyncFileDelete(params)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupSharedFileResponse>>`
  * [.asyncFileUpload(params)](broken-reference) ⇒ `Promise.<Array.<module:types~GroupSharedFile>>`

#### groupManage.asyncGetGroupInfo(group\_id, froce) ⇒ [`Promise.<GroupInfoAndSettings>`](broken-reference) <a href="#module_groupmanage.asyncgetgroupinfo" id="module_groupmanage.asyncgetgroupinfo"></a>

获取群信息

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: [`Promise.<GroupInfoAndSettings>`](broken-reference) - 群信息

| Param     | Type      | Description                                  |
| --------- | --------- | -------------------------------------------- |
| group\_id | `number`  | 群ID                                          |
| froce     | `boolean` | 是否强制从服务器拉取： true - 从服务器拉取， false - 优先从本地存储获取 |

#### groupManage.asyncGetJoinedGroups(froce) ⇒ `Promise.<Array.<number>>` <a href="#module_groupmanage.asyncgetjoinedgroups" id="module_groupmanage.asyncgetjoinedgroups"></a>

获取加入的群组

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<number>>` - 群组ID列表

| Param | Type      | Description                                  |
| ----- | --------- | -------------------------------------------- |
| froce | `boolean` | 是否强制从服务器拉取： true - 从服务器拉取， false - 优先从本地存储获取 |

#### groupManage.openGroup(group\_id) <a href="#module_groupmanage.opengroup" id="module_groupmanage.opengroup"></a>

打开群组， 此方法会准备群组聊天界面的一些必备信息。

**Kind**: static method of [`groupManage`](broken-reference)

| Param     | Type     | Description |
| --------- | -------- | ----------- |
| group\_id | `number` | 群组ID        |

#### groupManage.getAllGroupDetail() ⇒ `Object.<number, module:types~GroupInfoAndSettings>` <a href="#module_groupmanage.getallgroupdetail" id="module_groupmanage.getallgroupdetail"></a>

获取缓存的所有群组详情

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Object.<number, module:types~GroupInfoAndSettings>` - 群组详情

#### groupManage.asyncGetGroupMembers(group\_id) ⇒ `Promise.<Array.<module:types~GroupMember>>` <a href="#module_groupmanage.asyncgetgroupmembers" id="module_groupmanage.asyncgetgroupmembers"></a>

获取群组成员（异步）

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupMember>>` - 群成员列表

| Param     | Type     | Description |
| --------- | -------- | ----------- |
| group\_id | `number` | 群组ID        |

#### groupManage.getGroupMembers(group\_id) ⇒ [`Array.<GroupMember>`](broken-reference) <a href="#module_groupmanage.getgroupmembers" id="module_groupmanage.getgroupmembers"></a>

获取群组成员（同步）

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: [`Array.<GroupMember>`](broken-reference) - 群成员列表

| Param     | Type     | Description |
| --------- | -------- | ----------- |
| group\_id | `number` | 群组ID        |

#### groupManage.asyncGetGroupListDetail(gids) ⇒ `Promise.<Array.<module:types~BriefGroupInfoAndSettings>>` <a href="#module_groupmanage.asyncgetgrouplistdetail" id="module_groupmanage.asyncgetgrouplistdetail"></a>

按id获取群组详情

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~BriefGroupInfoAndSettings>>` - 群组详情列表

| Param | Type             | Description |
| ----- | ---------------- | ----------- |
| gids  | `Array.<number>` | 群组ID列表      |

#### groupManage.getGruopMessage(gid) ⇒ [`Array.<Meta>`](broken-reference) <a href="#module_groupmanage.getgruopmessage" id="module_groupmanage.getgruopmessage"></a>

获取群消息

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: [`Array.<Meta>`](broken-reference) - 群消息列表

| Param | Type     | Description |
| ----- | -------- | ----------- |
| gid   | `number` | 群ID         |

#### groupManage.asyncGetInfo(params) ⇒ [`Promise.<GroupInfoAndSettings>`](broken-reference) <a href="#module_groupmanage.asyncgetinfo" id="module_groupmanage.asyncgetinfo"></a>

获取群组详情

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: [`Promise.<GroupInfoAndSettings>`](broken-reference) - 群组详情

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

#### groupManage.asyncGetMemberList(param) ⇒ `Promise.<Array.<module:types~GroupMember>>` <a href="#module_groupmanage.asyncgetmemberlist" id="module_groupmanage.asyncgetmemberlist"></a>

获取群成员列表

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupMember>>` - 群成员列表

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| param            | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

#### groupManage.readGroupMessage(group\_id, mid) <a href="#module_groupmanage.readgroupmessage" id="module_groupmanage.readgroupmessage"></a>

将群消息设置已读

**Kind**: static method of [`groupManage`](broken-reference)

| Param     | Type     | Description |
| --------- | -------- | ----------- |
| group\_id | `number` | 群组ID        |
| mid       | `number` | 消息ID        |

#### groupManage.recallMessage(uid, mid) <a href="#module_groupmanage.recallmessage" id="module_groupmanage.recallmessage"></a>

撤回消息

**Kind**: static method of [`groupManage`](broken-reference)

| Param | Type     | Description |
| ----- | -------- | ----------- |
| uid   | `number` | 群组ID        |
| mid   | `number` | 消息ID        |

#### groupManage.getUnreadCount(gid) ⇒ `number` <a href="#module_groupmanage.getunreadcount" id="module_groupmanage.getunreadcount"></a>

获取群未读消息数

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `number` - 未读消息数

| Param | Type     | Description |
| ----- | -------- | ----------- |
| gid   | `number` | 群组ID        |

#### groupManage.asyncGetAdminList(params) ⇒ `Promise.<Array.<module:types~GroupMember>>` <a href="#module_groupmanage.asyncgetadminlist" id="module_groupmanage.asyncgetadminlist"></a>

获取群管理员列表

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupMember>>` - 群管理员列表

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

#### groupManage.asyncAdminAdd(params) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>` <a href="#module_groupmanage.asyncadminadd" id="module_groupmanage.asyncadminadd"></a>

群添加管理员

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupUserRelationResponse>>` - 结果列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.user\_list | `Array.<number>` | 群成员列表       |

#### groupManage.asyncAdminRemove(params) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>` <a href="#module_groupmanage.asyncadminremove" id="module_groupmanage.asyncadminremove"></a>

移除管理员

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupUserRelationResponse>>` - 结果列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.user\_list | `Array.<number>` | 群成员列表       |

#### groupManage.asyncGetAnouncementById(params) ⇒ [`Promise.<GroupAnnouncement>`](broken-reference) <a href="#module_groupmanage.asyncgetanouncementbyid" id="module_groupmanage.asyncgetanouncementbyid"></a>

获取群公告详情

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: [`Promise.<GroupAnnouncement>`](broken-reference) - 群公告详情

| Param                   | Type             | Description |
| ----------------------- | ---------------- | ----------- |
| params                  | `object`         | 参数          |
| params.group\_id        | `number`         | 群组ID        |
| params.announcement\_id | `Array.<number>` | 公告ID        |

#### groupManage.asyncAnouncementDelete(params) ⇒ `Promise.<boolean>` <a href="#module_groupmanage.asyncanouncementdelete" id="module_groupmanage.asyncanouncementdelete"></a>

删除群公告

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param                   | Type             | Description |
| ----------------------- | ---------------- | ----------- |
| params                  | `object`         | 参数          |
| params.group\_id        | `number`         | 群组ID        |
| params.announcement\_id | `Array.<number>` | 公告ID        |

#### groupManage.asyncAnnouncementEdit(params) ⇒ [`Promise.<GroupAnnouncement>`](broken-reference) <a href="#module_groupmanage.asyncannouncementedit" id="module_groupmanage.asyncannouncementedit"></a>

编辑群公告

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: [`Promise.<GroupAnnouncement>`](broken-reference) - 群公告详情

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |
| params.title     | `string` | 公告标题        |
| params.content   | `string` | 公告内容        |

#### groupManage.asyncGetAnnouncementList(params) ⇒ `Promise.<Array.<module:types~GroupAnnouncement>>` <a href="#module_groupmanage.asyncgetannouncementlist" id="module_groupmanage.asyncgetannouncementlist"></a>

群公告列表

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupAnnouncement>>` - 群公告详情列表

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

#### groupManage.asyncCreate(params) ⇒ [`Promise.<GroupInfoAndSettings>`](broken-reference) <a href="#module_groupmanage.asynccreate" id="module_groupmanage.asynccreate"></a>

创建群组

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: [`Promise.<GroupInfoAndSettings>`](broken-reference) - 群详情

| Param  | Type                                   | Description |
| ------ | -------------------------------------- | ----------- |
| params | [`GroupInfoRequest`](broken-reference) | 请求参数        |

#### groupManage.asyncDestroy(params) ⇒ `Promise.<boolean>` <a href="#module_groupmanage.asyncdestroy" id="module_groupmanage.asyncdestroy"></a>

解散群组

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

#### groupManage.asyncUpdateAvatar(params) ⇒ `Promise.<boolean>` <a href="#module_groupmanage.asyncupdateavatar" id="module_groupmanage.asyncupdateavatar"></a>

更新群头像

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |
| params.value     | `string` | 头像地址        |

#### groupManage.asyncUpdateDescription(params) ⇒ `Promise.<boolean>` <a href="#module_groupmanage.asyncupdatedescription" id="module_groupmanage.asyncupdatedescription"></a>

更新群描述

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |
| params.value     | `string` | 群组描述        |

#### groupManage.asyncUpdateExt(params) ⇒ `Promise.<boolean>` <a href="#module_groupmanage.asyncupdateext" id="module_groupmanage.asyncupdateext"></a>

更新群扩展信息

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |
| params.value     | `string` | 扩展信息        |

#### groupManage.asyncUpdateName(params) ⇒ `Promise.<boolean>` <a href="#module_groupmanage.asyncupdatename" id="module_groupmanage.asyncupdatename"></a>

更新群名称

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |
| params.value     | `string` | 群名称         |

#### groupManage.asyncGroupMsgMutemode(params) ⇒ `Promise.<boolean>` <a href="#module_groupmanage.asyncgroupmsgmutemode" id="module_groupmanage.asyncgroupmsgmutemode"></a>

设置群消息免打扰情况

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param                  | Type     | Description                                          |
| ---------------------- | -------- | ---------------------------------------------------- |
| params                 | `object` | 参数                                                   |
| params.group\_id       | `number` | 群组ID                                                 |
| params.msg\_mute\_mode | `number` | 群消息屏蔽模式: 0 - 表示不屏蔽, 1 - 表示屏蔽本地消息通知, 2 - 表示屏蔽消息，不接收消息 |

#### groupManage.asyncGroupBannedList(params) ⇒ `Promise.<Array.<module:types~GroupMemberBanned>>` <a href="#module_groupmanage.asyncgroupbannedlist" id="module_groupmanage.asyncgroupbannedlist"></a>

获取群禁言列表

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupMemberBanned>>` - 禁言成员列表

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

#### groupManage.asyncGroupBab(params) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>` <a href="#module_groupmanage.asyncgroupbab" id="module_groupmanage.asyncgroupbab"></a>

禁言群成员

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupUserRelationResponse>>` - 请求结果列表

| Param  | Type                                           | Description |
| ------ | ---------------------------------------------- | ----------- |
| params | [`GroupBannedMemberRequest`](broken-reference) | 请求参数        |

#### groupManage.asyncGroupUnban(params) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>` <a href="#module_groupmanage.asyncgroupunban" id="module_groupmanage.asyncgroupunban"></a>

解除成员禁言

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupUserRelationResponse>>` - 请求结果列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.user\_list | `Array.<number>` | 群成员列表       |

#### groupManage.asyncGetSettings(group\_id) ⇒ [`Promise.<GroupInfoAndSettings>`](broken-reference) <a href="#module_groupmanage.asyncgetsettings" id="module_groupmanage.asyncgetsettings"></a>

获取群设置

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: [`Promise.<GroupInfoAndSettings>`](broken-reference) - 群设置

| Param     | Type     | Description |
| --------- | -------- | ----------- |
| group\_id | `number` | 群ID         |

#### groupManage.asyncUpdateAllowMemberInvitation(params) ⇒ `Promise.<boolean>` <a href="#module_groupmanage.asyncupdateallowmemberinvitation" id="module_groupmanage.asyncupdateallowmemberinvitation"></a>

设置群成员是否可以邀请

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type      | Description                             |
| ---------------- | --------- | --------------------------------------- |
| params           | `object`  | 参数                                      |
| params.group\_id | `number`  | 群组ID                                    |
| params.value     | `boolean` | 群成员邀请设置: false - 不允许邀请, true - 允许邀请(默认) |

#### groupManage.asyncUpdateAllowMemberModify(params) ⇒ `Promise.<boolean>` <a href="#module_groupmanage.asyncupdateallowmembermodify" id="module_groupmanage.asyncupdateallowmembermodify"></a>

设置群成员是否可以修改群信息

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type      | Description                                           |
| ---------------- | --------- | ----------------------------------------------------- |
| params           | `object`  | 参数                                                    |
| params.group\_id | `number`  | 群组ID                                                  |
| params.value     | `boolean` | 群成员修改群信息设置: false - 群成员不能修改群信息(默认), true - 群成员可以修改群信息 |

#### groupManage.asyncUpdateEnableReadack(params) ⇒ `Promise.<boolean>` <a href="#module_groupmanage.asyncupdateenablereadack" id="module_groupmanage.asyncupdateenablereadack"></a>

设置群是否开启已读模式

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type      | Description                         |
| ---------------- | --------- | ----------------------------------- |
| params           | `object`  | 参数                                  |
| params.group\_id | `number`  | 群组ID                                |
| params.value     | `boolean` | 是否开启群消息已读功能: false - 不开启, true - 开启 |

#### groupManage.asyncUpdateHistoryVisible(params) ⇒ `Promise.<boolean>` <a href="#module_groupmanage.asyncupdatehistoryvisible" id="module_groupmanage.asyncupdatehistoryvisible"></a>

设置群历史是否可见

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type      | Description                       |
| ---------------- | --------- | --------------------------------- |
| params           | `object`  | 参数                                |
| params.group\_id | `number`  | 群组ID                              |
| params.value     | `boolean` | 设置群历史是否可见: false - 不可见, true - 可见 |

#### groupManage.asyncUpdateRequireadminapproval(params) ⇒ `Promise.<boolean>` <a href="#module_groupmanage.asyncupdaterequireadminapproval" id="module_groupmanage.asyncupdaterequireadminapproval"></a>

设置入群是否需要申请

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param                  | Type      | Description                           |
| ---------------------- | --------- | ------------------------------------- |
| params                 | `object`  | 参数                                    |
| params.group\_id       | `number`  | 群组ID                                  |
| params.apply\_approval | `boolean` | 入群申请审批设置, 0:同意所有申请 1:需要管理员确认 2:拒绝所有申请 |

#### groupManage.asyncBanAll(params) ⇒ [`Promise.<GroupBanAllResponse>`](broken-reference) <a href="#module_groupmanage.asyncbanall" id="module_groupmanage.asyncbanall"></a>

全员禁言，只允许管理员发消息

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: [`Promise.<GroupBanAllResponse>`](broken-reference) - 结果

| Param            | Type     | Description      |
| ---------------- | -------- | ---------------- |
| params           | `object` | 参数               |
| params.duration  | `number` | 禁言时长，单位为分钟,int64 |
| params.group\_id | `number` | 群id,int64        |

#### groupManage.asyncUnBanAll(params) ⇒ `Promise.<boolean>` <a href="#module_groupmanage.asyncunbanall" id="module_groupmanage.asyncunbanall"></a>

取消全员禁言

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群id,int64   |

#### groupManage.asyncOwnerTransfer(params) ⇒ [`Promise.<GroupUserRelationResponse>`](broken-reference) <a href="#module_groupmanage.asyncownertransfer" id="module_groupmanage.asyncownertransfer"></a>

更换群主

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: [`Promise.<GroupUserRelationResponse>`](broken-reference) - 结果

| Param             | Type     | Description |
| ----------------- | -------- | ----------- |
| params            | `object` | 参数          |
| params.group\_id  | `number` | 群组ID        |
| params.new\_owner | `number` | 新群主的用户ID    |

#### groupManage.asyncGetUserJoined(params) ⇒ `Promise.<Array.<number>>` <a href="#module_groupmanage.asyncgetuserjoined" id="module_groupmanage.asyncgetuserjoined"></a>

获取用户的群组列表

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<number>>` - 群ID的列表

| Param  | Type     | Description |
| ------ | -------- | ----------- |
| params | `object` | 参数, 空对象     |

#### groupManage.asyncApply(params) ⇒ [`Promise.<GroupUserRelationResponse>`](broken-reference) <a href="#module_groupmanage.asyncapply" id="module_groupmanage.asyncapply"></a>

申请加入群

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: [`Promise.<GroupUserRelationResponse>`](broken-reference) - 结果

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |
| params.reason    | `string` | 申请入群原因      |

#### groupManage.asyncApplyHandle(params) ⇒ [`Promise.<GroupUserRelationResponse>`](broken-reference) <a href="#module_groupmanage.asyncapplyhandle" id="module_groupmanage.asyncapplyhandle"></a>

处理用户的入群申请

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: [`Promise.<GroupUserRelationResponse>`](broken-reference) - 结果

| Param            | Type      | Description           |
| ---------------- | --------- | --------------------- |
| params           | `object`  | 参数                    |
| params.group\_id | `number`  | 群组ID                  |
| params.user\_id  | `number`  | 用户ID                  |
| params.approval  | `boolean` | 审批结果：true为同意，false为拒绝 |

#### groupManage.asyncGroupBockedlist(params) ⇒ `Promise.<Array.<module:types~GroupBlockedListItem>>` <a href="#module_groupmanage.asyncgroupbockedlist" id="module_groupmanage.asyncgroupbockedlist"></a>

获取群黑名单

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupBlockedListItem>>` - 群黑名单列表

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

#### groupManage.asyncGroupBlock(params) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>` <a href="#module_groupmanage.asyncgroupblock" id="module_groupmanage.asyncgroupblock"></a>

将成员加入黑名单

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupUserRelationResponse>>` - 结果列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.user\_list | `Array.<number>` | 群成员列表       |

#### groupManage.asyncGroupUnblock(params) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>` <a href="#module_groupmanage.asyncgroupunblock" id="module_groupmanage.asyncgroupunblock"></a>

解除黑名单

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupUserRelationResponse>>` - 结果列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.user\_list | `Array.<number>` | 群成员列表       |

#### groupManage.asyncKick(params) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>` <a href="#module_groupmanage.asynckick" id="module_groupmanage.asynckick"></a>

踢出群组

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupUserRelationResponse>>` - 结果列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.user\_list | `Array.<number>` | 群成员列表       |

#### groupManage.asyncGetInvitationList() ⇒ `Promise.<Array.<module:types~GroupInvitation>>` <a href="#module_groupmanage.asyncgetinvitationlist" id="module_groupmanage.asyncgetinvitationlist"></a>

获取群邀请列表

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupInvitation>>` - 群邀请列表

#### groupManage.asyncInvite(params) ⇒ `Promise.<Array.<module:types~GroupUserRelationResponse>>` <a href="#module_groupmanage.asyncinvite" id="module_groupmanage.asyncinvite"></a>

邀请成员加入群

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupUserRelationResponse>>` - 结果列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.user\_list | `Array.<number>` | 群成员列表       |

#### groupManage.asyncInviteHandle(params) ⇒ `Promise.<boolean>` <a href="#module_groupmanage.asyncinvitehandle" id="module_groupmanage.asyncinvitehandle"></a>

处理群邀请

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type      | Description           |
| ---------------- | --------- | --------------------- |
| params           | `object`  | 参数                    |
| params.group\_id | `number`  | 群组ID                  |
| params.user\_id  | `number`  | 用户ID                  |
| params.approval  | `boolean` | 审批结果：true为同意，false为拒绝 |

#### groupManage.asyncGetMemberDisplayName(params) ⇒ `Promise.<Array.<module:types~GroupMember>>` <a href="#module_groupmanage.asyncgetmemberdisplayname" id="module_groupmanage.asyncgetmemberdisplayname"></a>

批量获取群成员的群名片

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupMember>>` - 群成员列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.user\_list | `Array.<number>` | 群成员列表       |

#### groupManage.asyncLeave(params) ⇒ `Promise.<boolean>` <a href="#module_groupmanage.asyncleave" id="module_groupmanage.asyncleave"></a>

退出群

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

#### groupManage.asyncUpdateDisplayName(params) ⇒ `Promise.<boolean>` <a href="#module_groupmanage.asyncupdatedisplayname" id="module_groupmanage.asyncupdatedisplayname"></a>

修改群名片

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |
| params.value     | `string` | 新名片         |

#### groupManage.asncGetApplicationList(params) ⇒ `Promise.<Array.<module:types~GroupApplication>>` <a href="#module_groupmanage.asncgetapplicationlist" id="module_groupmanage.asncgetapplicationlist"></a>

获取群申请列表

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupApplication>>` - 群申请列表

| Param              | Type             | Description |
| ------------------ | ---------------- | ----------- |
| params             | `object`         | 参数          |
| params.group\_list | `Array.<number>` | 群列表         |

#### groupManage.asyncGetFileList(params) ⇒ `Promise.<Array.<module:types~GroupSharedFile>>` <a href="#module_groupmanage.asyncgetfilelist" id="module_groupmanage.asyncgetfilelist"></a>

获取群文件列表

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupSharedFile>>` - 群文件列表

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

#### groupManage.asyncFileDelete(params) ⇒ `Promise.<Array.<module:types~GroupSharedFileResponse>>` <a href="#module_groupmanage.asyncfiledelete" id="module_groupmanage.asyncfiledelete"></a>

删除群文件

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupSharedFileResponse>>` - 结果列表

| Param             | Type             | Description |
| ----------------- | ---------------- | ----------- |
| params            | `object`         | 参数          |
| params.group\_id  | `number`         | 群组ID        |
| params.file\_list | `Array.<number>` | 文件ID列表      |

#### groupManage.asyncFileUpload(params) ⇒ `Promise.<Array.<module:types~GroupSharedFile>>` <a href="#module_groupmanage.asyncfileupload" id="module_groupmanage.asyncfileupload"></a>

上传群文件

**Kind**: static method of [`groupManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~GroupSharedFile>>` - 群文件列表

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群id,int64   |
| params.name      | `string` | 文件名称        |
| params.size      | `number` | 文件大小,int64  |
| params.type      | `string` | 文件类型        |
| params.url       | `string` | 文件url       |

### rosterManage <a href="#module_rostermanage" id="module_rostermanage"></a>

好友管理

* [rosterManage](broken-reference)
  * [.asyncGetRosterIdList(force)](broken-reference) ⇒ `Promise.<Array.<number>>`
  * [.asyncGetRosterInfo(roster\_id, force)](broken-reference) ⇒ [`Promise.<RosterItem>`](broken-reference)
  * [.asyncRegester(opt)](broken-reference) ⇒ [`Promise.<UserSettings>`](broken-reference)
  * [.asyncDeleteRoster(param)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asnycGetRosterListDetailByIds(roster\_ids)](broken-reference) ⇒ `Promise.<Array.<module:types~RosterItem>>`
  * [.getAllRosterDetail()](broken-reference) ⇒ [`Array.<RosterItem>`](broken-reference)
  * [.asyncGetUserProfile(force)](broken-reference) ⇒ [`Promise.<UserProfile>`](broken-reference)
  * [.getRosterMessageByRid(uid)](broken-reference) ⇒ [`Array.<Meta>`](broken-reference)
  * [.readRosterMessage(roster\_id, mid)](broken-reference)
  * [.recallMessage(uid, mid)](broken-reference)
  * [.unreadMessage(uid, mid)](broken-reference)
  * [.deleteMessage(uid, mid)](broken-reference)
  * [.getRosterInfo(rid)](broken-reference) ⇒ [`RosterItem`](broken-reference)
  * [.getUnreadCount(uid)](broken-reference) ⇒ `number`
  * [.asyncGetApplyList(params)](broken-reference) ⇒ `Promise.<Array.<module:types~RosterApplication>>`
  * [.asyncGetBlockedlist(params)](broken-reference) ⇒ `Promise.<Array.<number>>`
  * [.asyncBlockeAdd(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncBlockeRemove(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncApply(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncAccept(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncDecline(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncUpdateRosterExt(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncSearchRosterByName(params)](broken-reference) ⇒ [`Promise.<RosterItem>`](broken-reference)
  * [.asyncSearchRosterById(params)](broken-reference) ⇒ [`Promise.<RosterItem>`](broken-reference)

#### rosterManage.asyncGetRosterIdList(force) ⇒ `Promise.<Array.<number>>` <a href="#module_rostermanage.asyncgetrosteridlist" id="module_rostermanage.asyncgetrosteridlist"></a>

获取好友id列表

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: `Promise.<Array.<number>>` - 用户ID列表

| Param | Type      | Description                               |
| ----- | --------- | ----------------------------------------- |
| force | `boolean` | 是否强制从服务器拉取：true - 从服务器获取， false - 从本地存储获取 |

#### rosterManage.asyncGetRosterInfo(roster\_id, force) ⇒ [`Promise.<RosterItem>`](broken-reference) <a href="#module_rostermanage.asyncgetrosterinfo" id="module_rostermanage.asyncgetrosterinfo"></a>

获取好友信息

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: [`Promise.<RosterItem>`](broken-reference) - 好友信息

| Param      | Type      | Description                                  |
| ---------- | --------- | -------------------------------------------- |
| roster\_id | `number`  | 好友ID                                         |
| force      | `boolean` | 是否强制从服务器拉取： true - 从服务器拉取， false - 优先从本地存储获取 |

#### rosterManage.asyncRegester(opt) ⇒ [`Promise.<UserSettings>`](broken-reference) <a href="#module_rostermanage.asyncregester" id="module_rostermanage.asyncregester"></a>

用户注册

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: [`Promise.<UserSettings>`](broken-reference) - 用户设置

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| opt          | `object` | 用户信息        |
| opt.username | `string` | 用户名         |
| opt.password | `string` | 密码          |

#### rosterManage.asyncDeleteRoster(param) ⇒ `Promise.<boolean>` <a href="#module_rostermanage.asyncdeleteroster" id="module_rostermanage.asyncdeleteroster"></a>

删除好友

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 请求结果

| Param          | Type     | Description |
| -------------- | -------- | ----------- |
| param          | `object` | 参数          |
| param.user\_id | `number` | 好友的用户ID     |

#### rosterManage.asnycGetRosterListDetailByIds(roster\_ids) ⇒ `Promise.<Array.<module:types~RosterItem>>` <a href="#module_rostermanage.asnycgetrosterlistdetailbyids" id="module_rostermanage.asnycgetrosterlistdetailbyids"></a>

根据id列表获取用户详细信息

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~RosterItem>>` - 用户详细信息列表

| Param       | Type             | Description |
| ----------- | ---------------- | ----------- |
| roster\_ids | `Array.<number>` | 用户ID列表      |

#### rosterManage.getAllRosterDetail() ⇒ [`Array.<RosterItem>`](broken-reference) <a href="#module_rostermanage.getallrosterdetail" id="module_rostermanage.getallrosterdetail"></a>

获取缓存的所有用户详细信息

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: [`Array.<RosterItem>`](broken-reference) - 用户详细信息列表

#### rosterManage.asyncGetUserProfile(force) ⇒ [`Promise.<UserProfile>`](broken-reference) <a href="#module_rostermanage.asyncgetuserprofile" id="module_rostermanage.asyncgetuserprofile"></a>

获取自己的用户信息

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: [`Promise.<UserProfile>`](broken-reference) - 用户信息

| Param | Type      | Description                                  |
| ----- | --------- | -------------------------------------------- |
| force | `boolean` | 是否强制从服务器拉取： true - 从服务器拉取， false - 优先从本地存储获取 |

#### rosterManage.getRosterMessageByRid(uid) ⇒ [`Array.<Meta>`](broken-reference) <a href="#module_rostermanage.getrostermessagebyrid" id="module_rostermanage.getrostermessagebyrid"></a>

根据会话ID获取聊天消息

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: [`Array.<Meta>`](broken-reference) - 聊天消息列表

| Param | Type     | Description |
| ----- | -------- | ----------- |
| uid   | `number` | 会话ID        |

#### rosterManage.readRosterMessage(roster\_id, mid) <a href="#module_rostermanage.readrostermessage" id="module_rostermanage.readrostermessage"></a>

修改消息状态为已读

**Kind**: static method of [`rosterManage`](broken-reference)

| Param      | Type     | Description |
| ---------- | -------- | ----------- |
| roster\_id | `number` | 会话ID        |
| mid        | `number` | 消息ID        |

#### rosterManage.recallMessage(uid, mid) <a href="#module_rostermanage.recallmessage" id="module_rostermanage.recallmessage"></a>

撤回消息，只能撤回5分钟内的

**Kind**: static method of [`rosterManage`](broken-reference)

| Param | Type     | Description |
| ----- | -------- | ----------- |
| uid   | `number` | 会话ID        |
| mid   | `number` | 消息ID        |

#### rosterManage.unreadMessage(uid, mid) <a href="#module_rostermanage.unreadmessage" id="module_rostermanage.unreadmessage"></a>

设置消息成未读

**Kind**: static method of [`rosterManage`](broken-reference)

| Param | Type     | Description |
| ----- | -------- | ----------- |
| uid   | `number` | 会话ID        |
| mid   | `number` | 消息ID        |

#### rosterManage.deleteMessage(uid, mid) <a href="#module_rostermanage.deletemessage" id="module_rostermanage.deletemessage"></a>

删除消息

**Kind**: static method of [`rosterManage`](broken-reference)

| Param | Type     | Description |
| ----- | -------- | ----------- |
| uid   | `number` | 会话ID        |
| mid   | `number` | 消息ID        |

#### rosterManage.getRosterInfo(rid) ⇒ [`RosterItem`](broken-reference) <a href="#module_rostermanage.getrosterinfo" id="module_rostermanage.getrosterinfo"></a>

获取好友信息

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: [`RosterItem`](broken-reference) - 好友信息

| Param | Type     | Description |
| ----- | -------- | ----------- |
| rid   | `number` | 好友ID        |

#### rosterManage.getUnreadCount(uid) ⇒ `number` <a href="#module_rostermanage.getunreadcount" id="module_rostermanage.getunreadcount"></a>

获取指定会话的未读数

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: `number` - 未读数

| Param | Type     | Description |
| ----- | -------- | ----------- |
| uid   | `number` | 会话IID       |

#### rosterManage.asyncGetApplyList(params) ⇒ `Promise.<Array.<module:types~RosterApplication>>` <a href="#module_rostermanage.asyncgetapplylist" id="module_rostermanage.asyncgetapplylist"></a>

获取好友申请列表

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: `Promise.<Array.<module:types~RosterApplication>>` - 好友申请列表

| Param         | Type     | Description           |
| ------------- | -------- | --------------------- |
| params        | `object` | 参数                    |
| params.cursor | `number` | 从哪开始获取：可以传空字符串表示从头开始取 |

#### rosterManage.asyncGetBlockedlist(params) ⇒ `Promise.<Array.<number>>` <a href="#module_rostermanage.asyncgetblockedlist" id="module_rostermanage.asyncgetblockedlist"></a>

获取黑名单

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: `Promise.<Array.<number>>` - 用户ID列表

| Param  | Type     | Description |
| ------ | -------- | ----------- |
| params | `object` | 参数：空对象      |

#### rosterManage.asyncBlockeAdd(params) ⇒ `Promise.<boolean>` <a href="#module_rostermanage.asyncblockeadd" id="module_rostermanage.asyncblockeadd"></a>

加入黑名单

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param           | Type     | Description |
| --------------- | -------- | ----------- |
| params          | `object` | 参数          |
| params.user\_id | `number` | 用户ID        |

#### rosterManage.asyncBlockeRemove(params) ⇒ `Promise.<boolean>` <a href="#module_rostermanage.asyncblockeremove" id="module_rostermanage.asyncblockeremove"></a>

移除黑名单

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param           | Type     | Description |
| --------------- | -------- | ----------- |
| params          | `object` | 参数          |
| params.user\_id | `number` | 用户ID        |

#### rosterManage.asyncApply(params) ⇒ `Promise.<boolean>` <a href="#module_rostermanage.asyncapply" id="module_rostermanage.asyncapply"></a>

请求加为好友

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param           | Type     | Description |
| --------------- | -------- | ----------- |
| params          | `object` | 参数          |
| params.user\_id | `number` | 用户ID        |
| params.alias    | `string` | 备注          |

#### rosterManage.asyncAccept(params) ⇒ `Promise.<boolean>` <a href="#module_rostermanage.asyncaccept" id="module_rostermanage.asyncaccept"></a>

通过好友申请

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param           | Type     | Description |
| --------------- | -------- | ----------- |
| params          | `object` | 参数          |
| params.user\_id | `number` | 用户ID        |

#### rosterManage.asyncDecline(params) ⇒ `Promise.<boolean>` <a href="#module_rostermanage.asyncdecline" id="module_rostermanage.asyncdecline"></a>

拒绝好友申请

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param           | Type     | Description |
| --------------- | -------- | ----------- |
| params          | `object` | 参数          |
| params.user\_id | `number` | 用户ID        |

#### rosterManage.asyncUpdateRosterExt(params) ⇒ `Promise.<boolean>` <a href="#module_rostermanage.asyncupdaterosterext" id="module_rostermanage.asyncupdaterosterext"></a>

修改好友扩展字段

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param           | Type     | Description |
| --------------- | -------- | ----------- |
| params          | `object` | 参数          |
| params.user\_id | `number` | 用户ID        |
| params.ext      | `string` | 扩展字段        |

#### rosterManage.asyncSearchRosterByName(params) ⇒ [`Promise.<RosterItem>`](broken-reference) <a href="#module_rostermanage.asyncsearchrosterbyname" id="module_rostermanage.asyncsearchrosterbyname"></a>

按名称搜索用户

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: [`Promise.<RosterItem>`](broken-reference) - 用户信息

| Param           | Type     | Description |
| --------------- | -------- | ----------- |
| params          | `object` | 参数          |
| params.username | `string` | 用户名         |

#### rosterManage.asyncSearchRosterById(params) ⇒ [`Promise.<RosterItem>`](broken-reference) <a href="#module_rostermanage.asyncsearchrosterbyid" id="module_rostermanage.asyncsearchrosterbyid"></a>

按ID搜索用户

**Kind**: static method of [`rosterManage`](broken-reference)\
**Returns**: [`Promise.<RosterItem>`](broken-reference) - 用户信息

| Param           | Type     | Description |
| --------------- | -------- | ----------- |
| params          | `object` | 参数          |
| params.user\_id | `number` | 用户ID        |

### sysManage <a href="#module_sysmanage" id="module_sysmanage"></a>

* [sysManage](broken-reference)
  * [.sendRosterMessage(msg)](broken-reference) ⇒ `number`
  * [.sendGroupMessage(msg)](broken-reference) ⇒ `number`
  * [.requireHistoryMessage(uid, sid, amount)](broken-reference)
  * [.sendMentionMessage(params)](broken-reference) ⇒ `number`
  * [.sendInputStatusMessage(uid, status)](broken-reference) ⇒ `number`
  * [.forwardMessage(param)](broken-reference) ⇒ `number`
  * [.getMessageStatus(cid, mid, isGroup)](broken-reference) ⇒ `string`
  * [.asyncFileUpload(param)](broken-reference) ⇒ [`Promise.<FileUploadResult>`](broken-reference)
  * [.getImage(param)](broken-reference) ⇒ `string`
  * [.deleteConversation(id, other\_devices)](broken-reference)
  * [.asyncGetGroupAvatarUploadUrl(params)](broken-reference) ⇒ [`Promise.<FileUpload>`](broken-reference)
  * [.asyncGetFileUploadChatFileUrl(params)](broken-reference) ⇒ [`Promise.<FileUpload>`](broken-reference)

#### sysManage.sendRosterMessage(msg) ⇒ `number` <a href="#module_sysmanage.sendrostermessage" id="module_sysmanage.sendrostermessage"></a>

发送单聊消息

**Kind**: static method of [`sysManage`](broken-reference)\
**Returns**: `number` - 客户端生成的消息ID

| Param          | Type                 | Description                                                                                              |
| -------------- | -------------------- | -------------------------------------------------------------------------------------------------------- |
| msg            | `object`             | 消息体                                                                                                      |
| msg.uid        | `string`             | 接收者ID                                                                                                    |
| msg.content    | `string`             | 消息内容                                                                                                     |
| msg.type       | `string`             | 消息类型： text - 文本, image - 图片， audio - 语音, video - 视频，file - 文件, location - 位置， command - 命令, forward - 转发 |
| msg.ext        | `string` \| `object` | 扩展字段                                                                                                     |
| msg.attachment | `string` \| `object` | 附件信息                                                                                                     |

#### sysManage.sendGroupMessage(msg) ⇒ `number` <a href="#module_sysmanage.sendgroupmessage" id="module_sysmanage.sendgroupmessage"></a>

发送群聊消息

**Kind**: static method of [`sysManage`](broken-reference)\
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

#### sysManage.requireHistoryMessage(uid, sid, amount) <a href="#module_sysmanage.requirehistorymessage" id="module_sysmanage.requirehistorymessage"></a>

请求历史消息

**Kind**: static method of [`sysManage`](broken-reference)

| Param  | Type     | Description                      |
| ------ | -------- | -------------------------------- |
| uid    | `number` | 会话ID                             |
| sid    | `number` | 消息ID: 从哪个消息向前拉取，传0表示从最新一条消息开始拉取。 |
| amount | `number` | 拉取的条数                            |

#### sysManage.sendMentionMessage(params) ⇒ `number` <a href="#module_sysmanage.sendmentionmessage" id="module_sysmanage.sendmentionmessage"></a>

群发送@消息

**Kind**: static method of [`sysManage`](broken-reference)\
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

#### sysManage.sendInputStatusMessage(uid, status) ⇒ `number` <a href="#module_sysmanage.sendinputstatusmessage" id="module_sysmanage.sendinputstatusmessage"></a>

发送输入状态消息

**Kind**: static method of [`sysManage`](broken-reference)\
**Returns**: `number` - 客户端生成的消息ID

| Param  | Type     | Description                      |
| ------ | -------- | -------------------------------- |
| uid    | `number` | 会话ID                             |
| status | `string` | 状态： nothing - 未输入， typing - 正在输入 |

#### sysManage.forwardMessage(param) ⇒ `number` <a href="#module_sysmanage.forwardmessage" id="module_sysmanage.forwardmessage"></a>

转发消息

**Kind**: static method of [`sysManage`](broken-reference)\
**Returns**: `number` - 客户端生成的消息ID

| Param     | Type     | Description       |
| --------- | -------- | ----------------- |
| param     | `object` | 参数                |
| param.uid | `number` | 接收方用户ID（仅转发单聊时设置） |
| param.gid | `number` | 接收方群组ID（仅转发群聊时设置） |
| param.mid | `number` | 要转发的消息ID          |

#### sysManage.getMessageStatus(cid, mid, isGroup) ⇒ `string` <a href="#module_sysmanage.getmessagestatus" id="module_sysmanage.getmessagestatus"></a>

获取消息的状态

**Kind**: static method of [`sysManage`](broken-reference)\
**Returns**: `string` - 消息状态: unread - 未读， delivered - 已投递， read - 已读

| Param   | Type      | Default | Description |
| ------- | --------- | ------- | ----------- |
| cid     | `number`  |         | 会话ID        |
| mid     | `number`  |         | 消息ID        |
| isGroup | `boolean` | `false` | 是否是群聊       |

#### sysManage.asyncFileUpload(param) ⇒ [`Promise.<FileUploadResult>`](broken-reference) <a href="#module_sysmanage.asyncfileupload" id="module_sysmanage.asyncfileupload"></a>

上传文件

**Kind**: static method of [`sysManage`](broken-reference)\
**Returns**: [`Promise.<FileUploadResult>`](broken-reference) - 文件上传结果

| Param                 | Type                                     | Description                                                                                                                                                                            |
| --------------------- | ---------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| param                 | `object`                                 | 参数                                                                                                                                                                                     |
| param.group\_d        | `number`                                 | 群组ID                                                                                                                                                                                   |
| param.toType          | `number`                                 | 接收者类型：rosterAvatar - 用户头像， chat - 聊天文件， groupAvatar - 群头像                                                                                                                              |
| param.to\_id          | `number`                                 | 接收者ID                                                                                                                                                                                  |
| param.file            | `File`                                   | 文件                                                                                                                                                                                     |
| param.fileType        | `string`                                 | 文件类型：file - 普通聊天文件, audio - 语音聊天文件(amr格式),image - 图片聊天文件, video - 视频聊天文件, audio-mp3 - 语音聊天文件(mp3格式), shareFile - 普通共享文件, shareAudio - 语音共享文件, shareImage - 图片共享文件, shareVideo - 视频共享文件 |
| param.chatType        | `number`                                 | 聊天类型： roster - 单聊, group - 群聊                                                                                                                                                          |
| param.processCallback | [`fileUploadProgress`](broken-reference) | 上传进度回调                                                                                                                                                                                 |

#### sysManage.getImage(param) ⇒ `string` <a href="#module_sysmanage.getimage" id="module_sysmanage.getimage"></a>

拼装图片路径

**Kind**: static method of [`sysManage`](broken-reference)\
**Returns**: `string` - 图片地址

| Param           | Type      | Description                |
| --------------- | --------- | -------------------------- |
| param           | `object`  |                            |
| param.avatar    | `string`  | 文件地址                       |
| param.type      | `string`  | 类型： roster - 用户, group - 群 |
| param.thumbnail | `boolean` | 是否缩略图：默认为true              |
| param.sdefault  | `string`  | 默认图片地址                     |

#### sysManage.deleteConversation(id, other\_devices) <a href="#module_sysmanage.deleteconversation" id="module_sysmanage.deleteconversation"></a>

删除会话

**Kind**: static method of [`sysManage`](broken-reference)

| Param          | Type      | Default | Description    |
| -------------- | --------- | ------- | -------------- |
| id             | `number`  |         | 会话ID           |
| other\_devices | `boolean` | `true`  | 是否同时删除其它设备上的会话 |

#### sysManage.asyncGetGroupAvatarUploadUrl(params) ⇒ [`Promise.<FileUpload>`](broken-reference) <a href="#module_sysmanage.asyncgetgroupavataruploadurl" id="module_sysmanage.asyncgetgroupavataruploadurl"></a>

获取上传群头像URL

**Kind**: static method of [`sysManage`](broken-reference)\
**Returns**: [`Promise.<FileUpload>`](broken-reference) - 文件上传信息

| Param            | Type     | Description |
| ---------------- | -------- | ----------- |
| params           | `object` | 参数          |
| params.group\_id | `number` | 群组ID        |

#### sysManage.asyncGetFileUploadChatFileUrl(params) ⇒ [`Promise.<FileUpload>`](broken-reference) <a href="#module_sysmanage.asyncgetfileuploadchatfileurl" id="module_sysmanage.asyncgetfileuploadchatfileurl"></a>

获取聊天文件上传地址

**Kind**: static method of [`sysManage`](broken-reference)\
**Returns**: [`Promise.<FileUpload>`](broken-reference) - 文件上传信息

| Param             | Type     | Description                                                                                                                                   |
| ----------------- | -------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| params            | `object` | 参数                                                                                                                                            |
| params.file\_type | `number` | 文件类型: 100 - 普通聊天文件, 101 - 语音聊天文件(amr格式),102 - 图片聊天文件, 103 - 视频聊天文件, 104 - 语音聊天文件(mp3格式)200 - 普通共享文件, 201 - 语音共享文件, 202 - 图片共享文件, 203 - 视频共享文件 |
| params.to\_type   | `number` | 会话类型： 1 - 用户，2 - 群组                                                                                                                           |
| params.to\_id     | `number` | 会话ID                                                                                                                                          |

### userManage <a href="#module_usermanage" id="module_usermanage"></a>

* [userManage](broken-reference)
  * [.getToken()](broken-reference) ⇒ `string`
  * [.getUid()](broken-reference) ⇒ `number`
  * [.getAppid()](broken-reference) ⇒ `string`
  * [.getConversationList()](broken-reference) ⇒ [`Array.<ConversationItem>`](broken-reference)
  * [.asyncUpdateAvatar(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncUpdateNickName(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncGetProfile()](broken-reference) ⇒ [`Promise.<UserProfile>`](broken-reference)
  * [.asyncUpdateProfile(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncGetSettings()](broken-reference) ⇒ [`Promise.<UserSettings>`](broken-reference)
  * [.asyncUpdateSettings(settings)](broken-reference) ⇒ `Promise.<boolean>`

#### userManage.getToken() ⇒ `string` <a href="#module_usermanage.gettoken" id="module_usermanage.gettoken"></a>

获取登录用户的token

**Kind**: static method of [`userManage`](broken-reference)\
**Returns**: `string` - 用户的token

#### userManage.getUid() ⇒ `number` <a href="#module_usermanage.getuid" id="module_usermanage.getuid"></a>

获取登录用户的uid

**Kind**: static method of [`userManage`](broken-reference)\
**Returns**: `number` - 用户ID

#### userManage.getAppid() ⇒ `string` <a href="#module_usermanage.getappid" id="module_usermanage.getappid"></a>

获取appid

**Kind**: static method of [`userManage`](broken-reference)\
**Returns**: `string` - APP ID

#### userManage.getConversationList() ⇒ [`Array.<ConversationItem>`](broken-reference) <a href="#module_usermanage.getconversationlist" id="module_usermanage.getconversationlist"></a>

获取最近会话列表

**Kind**: static method of [`userManage`](broken-reference)

#### userManage.asyncUpdateAvatar(params) ⇒ `Promise.<boolean>` <a href="#module_usermanage.asyncupdateavatar" id="module_usermanage.asyncupdateavatar"></a>

更新头像

**Kind**: static method of [`userManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param         | Type     | Description |
| ------------- | -------- | ----------- |
| params        | `object` | 参数          |
| params.avatar | `string` | 头像 url      |

#### userManage.asyncUpdateNickName(params) ⇒ `Promise.<boolean>` <a href="#module_usermanage.asyncupdatenickname" id="module_usermanage.asyncupdatenickname"></a>

更新昵称

**Kind**: static method of [`userManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param             | Type     | Description |
| ----------------- | -------- | ----------- |
| params            | `object` | 参数          |
| params.nick\_name | `string` | 昵称          |

#### userManage.asyncGetProfile() ⇒ [`Promise.<UserProfile>`](broken-reference) <a href="#module_usermanage.asyncgetprofile" id="module_usermanage.asyncgetprofile"></a>

获取用户profile

**Kind**: static method of [`userManage`](broken-reference)\
**Returns**: [`Promise.<UserProfile>`](broken-reference) - 用户信息

#### userManage.asyncUpdateProfile(params) ⇒ `Promise.<boolean>` <a href="#module_usermanage.asyncupdateprofile" id="module_usermanage.asyncupdateprofile"></a>

更新用户profile

**Kind**: static method of [`userManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param                | Type     | Description   |
| -------------------- | -------- | ------------- |
| params               | `object` |               |
| params.description   | `string` | 描述信息          |
| params.nick\_name    | `string` | 昵称            |
| params.private\_info | `string` | 私有信息，仅自己可见    |
| params.public\_info  | `string` | 公开信息，好友和陌生人可见 |

#### userManage.asyncGetSettings() ⇒ [`Promise.<UserSettings>`](broken-reference) <a href="#module_usermanage.asyncgetsettings" id="module_usermanage.asyncgetsettings"></a>

获取用户设置信息

**Kind**: static method of [`userManage`](broken-reference)\
**Returns**: [`Promise.<UserSettings>`](broken-reference) - 用户信息

#### userManage.asyncUpdateSettings(settings) ⇒ `Promise.<boolean>` <a href="#module_usermanage.asyncupdatesettings" id="module_usermanage.asyncupdatesettings"></a>

修改用户设置

**Kind**: static method of [`userManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param    | Type                               | Description |
| -------- | ---------------------------------- | ----------- |
| settings | [`UserSettings`](broken-reference) | 更新的设置       |

### types <a href="#module_types" id="module_types"></a>

* [types](broken-reference)
  * ["flooNotice" (res)](broken-reference)
  * ["flooError" (res)](broken-reference)
  * ["loginFail" (desc)](broken-reference)
  * ["loginSuccess" (res)](broken-reference)
  * ["onGroupListUpdate" (meta)](broken-reference)
  * ["onGroupMemberChanged" (groupId)](broken-reference)
  * ["onGroupMessage" (meta)](broken-reference)
  * ["onInputStatusMessage" (res)](broken-reference)
  * ["onMentionMessage" (meta)](broken-reference)
  * ["onMessageCanceled" (res)](broken-reference)
  * ["onMessageDeleted" (res)](broken-reference)
  * ["onMessageRecalled" (res)](broken-reference)
  * ["onMessageStatusChanged" (res)](broken-reference)
  * ["onReceiveHistoryMsg" (res)](broken-reference)
  * ["onRosterInfoUpdate" (res)](broken-reference)
  * ["onRosterListUpdate" (meta)](broken-reference)
  * ["onRosterMessage" (meta)](broken-reference)
  * ["onSendingMessageStatusChanged" (res)](broken-reference)
  * ["onUnreadChange" (cid)](broken-reference)
  * ["recentlistUpdate"](broken-reference)
  * ["onGroupCreated" (meta)](broken-reference)
  * ["onGroupDestoryed" (meta)](broken-reference)
  * ["onGroupJoined" (meta)](broken-reference)
  * ["onGroupApplyAccepted" (meta)](broken-reference)
  * ["onGroupApplyDeclined" (meta)](broken-reference)
  * ["onGroupBaned" (meta)](broken-reference)
  * ["onGroupUnbaned" (meta)](broken-reference)
  * [\~RosterItem](broken-reference) : `object`
  * [\~UserSettings](broken-reference) : `object`
  * [\~UserProfile](broken-reference) : `object`
  * [\~Meta](broken-reference) : `object`
  * [\~RosterApplication](broken-reference) : `object`
  * [\~GroupInfoAndSettings](broken-reference) : `object`
  * [\~BriefGroupInfoAndSettings](broken-reference) : `object`
  * [\~GroupMember](broken-reference) : `object`
  * [\~GroupMemberBanned](broken-reference) : `object`
  * [\~GroupUserRelationResponse](broken-reference) : `object`
  * [\~GroupAnnouncement](broken-reference) : `object`
  * [\~GroupInfoRequest](broken-reference) : `object`
  * [\~GroupBannedMemberRequest](broken-reference) : `object`
  * [\~GroupBlockedListItem](broken-reference) : `object`
  * [\~GroupInvitation](broken-reference) : `object`
  * [\~GroupApplication](broken-reference) : `object`
  * [\~GroupSharedFile](broken-reference) : `object`
  * [\~GroupSharedFileResponse](broken-reference) : `object`
  * [\~GroupBanAllResponse](broken-reference) : `object`
  * [\~FileUpload](broken-reference) : `object`
  * [\~FileUploadResult](broken-reference) : `object`
  * [\~fileUploadProgress](broken-reference) : `function`
  * [\~ConversationItem](broken-reference) : `object`
  * [\~UserProfile](broken-reference) : `object`
  * [\~UserSettings](broken-reference) : `object`
  * [\~Event](broken-reference) : `string`
  * [\~EventCallback](broken-reference) : `function`

#### "flooNotice" (res) <a href="#event_floonotice" id="event_floonotice"></a>

Floo通知

**Kind**: event emitted by [`types`](broken-reference)

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

#### "flooError" (res) <a href="#event_flooerror" id="event_flooerror"></a>

Floo错误

**Kind**: event emitted by [`types`](broken-reference)

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

#### "loginFail" (desc) <a href="#event_loginfail" id="event_loginfail"></a>

登录失败

**Kind**: event emitted by [`types`](broken-reference)

| Param | Type     | Description |
| ----- | -------- | ----------- |
| desc  | `string` | 失败原因        |

#### "loginSuccess" (res) <a href="#event_loginsuccess" id="event_loginsuccess"></a>

登录成功

**Kind**: event emitted by [`types`](broken-reference)

| Param | Type     | Description |
| ----- | -------- | ----------- |
| res   | `object` | 空对象         |

#### "onGroupListUpdate" (meta) <a href="#event_ongrouplistupdate" id="event_ongrouplistupdate"></a>

群列表更新

**Kind**: event emitted by [`types`](broken-reference)

| Param | Type                                      | Description |
| ----- | ----------------------------------------- | ----------- |
| meta  | [`Meta`](broken-reference) \| `undefined` | 通知消息内容      |

#### "onGroupMemberChanged" (groupId) <a href="#event_ongroupmemberchanged" id="event_ongroupmemberchanged"></a>

群成员列表更新

**Kind**: event emitted by [`types`](broken-reference)

| Param   | Type     | Description |
| ------- | -------- | ----------- |
| groupId | `number` | 群ID         |

#### "onGroupMessage" (meta) <a href="#event_ongroupmessage" id="event_ongroupmessage"></a>

收到群消息

**Kind**: event emitted by [`types`](broken-reference)

| Param | Type                       | Description |
| ----- | -------------------------- | ----------- |
| meta  | [`Meta`](broken-reference) | 消息内容        |

#### "onInputStatusMessage" (res) <a href="#event_oninputstatusmessage" id="event_oninputstatusmessage"></a>

对方正在输入

**Kind**: event emitted by [`types`](broken-reference)

| Param    | Type     | Description |
| -------- | -------- | ----------- |
| res      | `object` |             |
| res.ext  | `string` | 扩展字段        |
| res.from | `string` | 发送者用户ID     |
| res.to   | `string` | 接收者用户ID     |

#### "onMentionMessage" (meta) <a href="#event_onmentionmessage" id="event_onmentionmessage"></a>

收到群组@消息

**Kind**: event emitted by [`types`](broken-reference)

| Param | Type                       | Description |
| ----- | -------------------------- | ----------- |
| meta  | [`Meta`](broken-reference) | 消息内容        |

#### "onMessageCanceled" (res) <a href="#event_onmessagecanceled" id="event_onmessagecanceled"></a>

消息被取消已读

**Kind**: event emitted by [`types`](broken-reference)

| Param   | Type     | Description |
| ------- | -------- | ----------- |
| res     | `object` |             |
| res.uid | `string` | 会话ID        |
| res.mid | `string` | 消息ID        |

#### "onMessageDeleted" (res) <a href="#event_onmessagedeleted" id="event_onmessagedeleted"></a>

消息被删除

**Kind**: event emitted by [`types`](broken-reference)

| Param   | Type     | Description |
| ------- | -------- | ----------- |
| res     | `object` |             |
| res.uid | `string` | 会话ID        |
| res.mid | `string` | 消息ID        |

#### "onMessageRecalled" (res) <a href="#event_onmessagerecalled" id="event_onmessagerecalled"></a>

消息被撤回

**Kind**: event emitted by [`types`](broken-reference)

| Param   | Type     | Description |
| ------- | -------- | ----------- |
| res     | `object` |             |
| res.uid | `string` | 会话ID        |
| res.mid | `string` | 消息ID        |

#### "onMessageStatusChanged" (res) <a href="#event_onmessagestatuschanged" id="event_onmessagestatuschanged"></a>

消息状态变更：撤回/删除/已读

**Kind**: event emitted by [`types`](broken-reference)

| Param   | Type     | Description |
| ------- | -------- | ----------- |
| res     | `object` |             |
| res.uid | `string` | 会话ID        |
| res.mid | `string` | 消息ID        |

#### "onReceiveHistoryMsg" (res) <a href="#event_onreceivehistorymsg" id="event_onreceivehistorymsg"></a>

收到历史消息

**Kind**: event emitted by [`types`](broken-reference)

| Param    | Type     | Description |
| -------- | -------- | ----------- |
| res      | `object` |             |
| res.next | `number` | 下次取历史消息的key |

#### "onRosterInfoUpdate" (res) <a href="#event_onrosterinfoupdate" id="event_onrosterinfoupdate"></a>

好友信息变更

**Kind**: event emitted by [`types`](broken-reference)

| Param         | Type             | Description |
| ------------- | ---------------- | ----------- |
| res           | `object`         |             |
| res.rosterIds | `Array.<number>` | 好友的用户ID列表   |

#### "onRosterListUpdate" (meta) <a href="#event_onrosterlistupdate" id="event_onrosterlistupdate"></a>

好友列表变更

**Kind**: event emitted by [`types`](broken-reference)

| Param | Type                       | Description |
| ----- | -------------------------- | ----------- |
| meta  | [`Meta`](broken-reference) | 好友通知的消息内容   |

#### "onRosterMessage" (meta) <a href="#event_onrostermessage" id="event_onrostermessage"></a>

收到单聊消息

**Kind**: event emitted by [`types`](broken-reference)

| Param | Type                       | Description |
| ----- | -------------------------- | ----------- |
| meta  | [`Meta`](broken-reference) | 消息内容        |

#### "onSendingMessageStatusChanged" (res) <a href="#event_onsendingmessagestatuschanged" id="event_onsendingmessagestatuschanged"></a>

消息发送状态变更

**Kind**: event emitted by [`types`](broken-reference)

| Param       | Type     | Description       |
| ----------- | -------- | ----------------- |
| res         | `object` |                   |
| res.status: | `number` | 发送状态，取值为sending   |
| res.mid:    | `number` | 客户端生成的client\_mid |

#### "onUnreadChange" (cid) <a href="#event_onunreadchange" id="event_onunreadchange"></a>

未读数改变

**Kind**: event emitted by [`types`](broken-reference)

| Param | Type     | Description |
| ----- | -------- | ----------- |
| cid   | `number` | 会话ID        |

#### "recentlistUpdate" <a href="#event_recentlistupdate" id="event_recentlistupdate"></a>

最近会话更新

**Kind**: event emitted by [`types`](broken-reference)

#### "onGroupCreated" (meta) <a href="#event_ongroupcreated" id="event_ongroupcreated"></a>

群组创建通知

**Kind**: event emitted by [`types`](broken-reference)

| Param | Type                       | Description |
| ----- | -------------------------- | ----------- |
| meta  | [`Meta`](broken-reference) | 群通知的消息内容    |

#### "onGroupDestoryed" (meta) <a href="#event_ongroupdestoryed" id="event_ongroupdestoryed"></a>

群组解散通知

**Kind**: event emitted by [`types`](broken-reference)

| Param | Type                       | Description |
| ----- | -------------------------- | ----------- |
| meta  | [`Meta`](broken-reference) | 群通知的消息内容    |

#### "onGroupJoined" (meta) <a href="#event_ongroupjoined" id="event_ongroupjoined"></a>

成员入群通知

**Kind**: event emitted by [`types`](broken-reference)

| Param | Type                       | Description |
| ----- | -------------------------- | ----------- |
| meta  | [`Meta`](broken-reference) | 群通知的消息内容    |

#### "onGroupApplyAccepted" (meta) <a href="#event_ongroupapplyaccepted" id="event_ongroupapplyaccepted"></a>

群申请被通过

**Kind**: event emitted by [`types`](broken-reference)

| Param | Type                       | Description |
| ----- | -------------------------- | ----------- |
| meta  | [`Meta`](broken-reference) | 群通知的消息内容    |

#### "onGroupApplyDeclined" (meta) <a href="#event_ongroupapplydeclined" id="event_ongroupapplydeclined"></a>

群申请被拒绝

**Kind**: event emitted by [`types`](broken-reference)

| Param | Type                       | Description |
| ----- | -------------------------- | ----------- |
| meta  | [`Meta`](broken-reference) | 群通知的消息内容    |

#### "onGroupBaned" (meta) <a href="#event_ongroupbaned" id="event_ongroupbaned"></a>

被群禁言

**Kind**: event emitted by [`types`](broken-reference)

| Param | Type                       | Description |
| ----- | -------------------------- | ----------- |
| meta  | [`Meta`](broken-reference) | 群通知的消息内容    |

#### "onGroupUnbaned" (meta) <a href="#event_ongroupunbaned" id="event_ongroupunbaned"></a>

被群取消禁言

**Kind**: event emitted by [`types`](broken-reference)

| Param | Type                       | Description |
| ----- | -------------------------- | ----------- |
| meta  | [`Meta`](broken-reference) | 群通知的消息内容    |

#### types\~RosterItem : `object` <a href="#module_types..rosteritem" id="module_types..rosteritem"></a>

好友信息

**Kind**: inner typedef of [`types`](broken-reference)\
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

#### types\~UserSettings : `object` <a href="#module_types..usersettings" id="module_types..usersettings"></a>

用户设置信息

**Kind**: inner typedef of [`types`](broken-reference)\
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

#### types\~UserProfile : `object` <a href="#module_types..userprofile" id="module_types..userprofile"></a>

用户信息

**Kind**: inner typedef of [`types`](broken-reference)\
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

#### types\~Meta : `object` <a href="#module_types..meta" id="module_types..meta"></a>

消息体

**Kind**: inner typedef of [`types`](broken-reference)\
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

#### types\~RosterApplication : `object` <a href="#module_types..rosterapplication" id="module_types..rosterapplication"></a>

加好友申请列表项

**Kind**: inner typedef of [`types`](broken-reference)\
**Properties**

| Name          | Type     | Description                         |
| ------------- | -------- | ----------------------------------- |
| expired\_time | `number` | 过期时间,int64                          |
| reason        | `string` | 申请描述                                |
| status        | `number` | 状态： 0 - 等待确认， 1 - 接受， 2 - 拒绝。 int32 |
| user\_id      | `number` | 发起加好友申请的用户ID,int64                  |

#### types\~GroupInfoAndSettings : `object` <a href="#module_types..groupinfoandsettings" id="module_types..groupinfoandsettings"></a>

群信息

**Kind**: inner typedef of [`types`](broken-reference)\
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

#### types\~BriefGroupInfoAndSettings : `object` <a href="#module_types..briefgroupinfoandsettings" id="module_types..briefgroupinfoandsettings"></a>

群简要信息及用户设置

**Kind**: inner typedef of [`types`](broken-reference)\
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

#### types\~GroupMember : `object` <a href="#module_types..groupmember" id="module_types..groupmember"></a>

群成员格式

**Kind**: inner typedef of [`types`](broken-reference)\
**Properties**

| Name          | Type     | Description  |
| ------------- | -------- | ------------ |
| display\_name | `string` | 成员群名片        |
| join\_time    | `number` | 成员入群时间,int64 |
| user\_id      | `number` | 用户id,int64   |
| avatar        | `string` | 头像地址         |

#### types\~GroupMemberBanned : `object` <a href="#module_types..groupmemberbanned" id="module_types..groupmemberbanned"></a>

禁言成员

**Kind**: inner typedef of [`types`](broken-reference)\
**Properties**

| Name          | Type     | Description  |
| ------------- | -------- | ------------ |
| display\_name | `string` | 成员群名片        |
| join\_time    | `number` | 成员入群时间,int64 |
| user\_id      | `number` | 用户id,int64   |
| avatar        | `string` | 头像地址         |
| expired\_time | `number` | 禁言过期时间       |

#### types\~GroupUserRelationResponse : `object` <a href="#module_types..groupuserrelationresponse" id="module_types..groupuserrelationresponse"></a>

群用户请求结果

**Kind**: inner typedef of [`types`](broken-reference)\
**Properties**

| Name     | Type     | Description |
| -------- | -------- | ----------- |
| reason   | `string` | 原因          |
| result   | `string` | 结果          |
| user\_id | `number` | 用户ID，int64  |

#### types\~GroupAnnouncement : `object` <a href="#module_types..groupannouncement" id="module_types..groupannouncement"></a>

群公告内容

**Kind**: inner typedef of [`types`](broken-reference)\
**Properties**

| Name        | Type     | Description  |
| ----------- | -------- | ------------ |
| author      | `number` | 公告发布者,int64  |
| content     | `string` | 公告内容         |
| created\_at | `number` | 公告发布时间,int64 |
| group\_id   | `number` | 群id,int64    |
| id          | `number` | 公告id,int64   |
| title       | `string` | 公告标题         |

#### types\~GroupInfoRequest : `object` <a href="#module_types..groupinforequest" id="module_types..groupinforequest"></a>

创建群

**Kind**: inner typedef of [`types`](broken-reference)\
**Properties**

| Name        | Type             | Description                     |
| ----------- | ---------------- | ------------------------------- |
| avatar      | `string`         | 群头像                             |
| description | `string`         | 群描述                             |
| name        | `string`         | 群名称                             |
| type        | `number`         | 群类型 1表示公开群，0表示私有群, 2表示聊天室,int32 |
| user\_list  | `Array.<number>` | 邀请入群的用户id列表                     |

#### types\~GroupBannedMemberRequest : `object` <a href="#module_types..groupbannedmemberrequest" id="module_types..groupbannedmemberrequest"></a>

禁言请求

**Kind**: inner typedef of [`types`](broken-reference)\
**Properties**

| Name       | Type             | Description      |
| ---------- | ---------------- | ---------------- |
| duration   | `number`         | 禁言时长，单位为分钟,int64 |
| group\_id  | `number`         | 群id,int64        |
| user\_list | `Array.<number>` | 用户id列表           |

#### types\~GroupBlockedListItem : `object` <a href="#module_types..groupblockedlistitem" id="module_types..groupblockedlistitem"></a>

群组黑名单

**Kind**: inner typedef of [`types`](broken-reference)\
**Properties**

| Name       | Type     | Description |
| ---------- | -------- | ----------- |
| user\_id   | `number` | 用户id,int64  |
| group\_id  | `number` | 群id,int64   |
| create\_at | `string` | 创建时间        |

#### types\~GroupInvitation : `object` <a href="#module_types..groupinvitation" id="module_types..groupinvitation"></a>

群组邀请信息

**Kind**: inner typedef of [`types`](broken-reference)\
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

#### types\~GroupApplication : `object` <a href="#module_types..groupapplication" id="module_types..groupapplication"></a>

群申请信息

**Kind**: inner typedef of [`types`](broken-reference)\
**Properties**

| Name          | Type     | Description               |
| ------------- | -------- | ------------------------- |
| group\_id     | `number` | 群ID                       |
| applicant\_id | `number` | 申请者ID                     |
| reason        | `string` | 原因                        |
| expire\_time  | `number` | 过期时间                      |
| status        | `number` | 状态： 0 - 待处理，1 - 同意，2 - 拒绝 |

#### types\~GroupSharedFile : `object` <a href="#module_types..groupsharedfile" id="module_types..groupsharedfile"></a>

群共享文件返回格式

**Kind**: inner typedef of [`types`](broken-reference)\
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

#### types\~GroupSharedFileResponse : `object` <a href="#module_types..groupsharedfileresponse" id="module_types..groupsharedfileresponse"></a>

删除群共享文件结果

**Kind**: inner typedef of [`types`](broken-reference)\
**Properties**

| Name     | Type     | Description |
| -------- | -------- | ----------- |
| file\_id | `number` | 文件ID        |
| reason   | `string` | 原因          |
| result   | `string` | 结果          |

#### types\~GroupBanAllResponse : `object` <a href="#module_types..groupbanallresponse" id="module_types..groupbanallresponse"></a>

全员禁言结果

**Kind**: inner typedef of [`types`](broken-reference)\
**Properties**

| Name              | Type     | Description    |
| ----------------- | -------- | -------------- |
| ban\_expire\_time | `number` | 全员禁言过期时间,int64 |

#### types\~FileUpload : `object` <a href="#module_types..fileupload" id="module_types..fileupload"></a>

文件上传信息

**Kind**: inner typedef of [`types`](broken-reference)\
**Properties**

| Name             | Type                      | Description |
| ---------------- | ------------------------- | ----------- |
| download\_url    | `string`                  | 下载地址        |
| oss\_body\_param | `object.<string, string>` | 额外参数        |
| upload\_url      | `string`                  | 上传地址        |

#### types\~FileUploadResult : `object` <a href="#module_types..fileuploadresult" id="module_types..fileuploadresult"></a>

文件上传结果

**Kind**: inner typedef of [`types`](broken-reference)\
**Properties**

| Name | Type     | Description |
| ---- | -------- | ----------- |
| url  | `string` | 下载地址        |

#### types\~fileUploadProgress : `function` <a href="#module_types..fileuploadprogress" id="module_types..fileuploadprogress"></a>

文件上传进度回调

**Kind**: inner typedef of [`types`](broken-reference)

| Param      | Type     | Description |
| ---------- | -------- | ----------- |
| res        | `object` | 进度          |
| res.loaded | `number` | 已下载字节数      |
| res.total  | `number` | 总字节数        |

#### types\~ConversationItem : `object` <a href="#module_types..conversationitem" id="module_types..conversationitem"></a>

会话信息

**Kind**: inner typedef of [`types`](broken-reference)\
**Properties**

| Name      | Type     | Description                   |
| --------- | -------- | ----------------------------- |
| id        | `number` | 会话ID                          |
| content   | `string` | 消息内容                          |
| timestamp | `string` | 消息发送时间戳（毫秒）                   |
| type      | `string` | 会话类型： roster - 单聊， group - 群聊 |

#### types\~UserProfile : `object` <a href="#module_types..userprofile" id="module_types..userprofile"></a>

用户信息

**Kind**: inner typedef of [`types`](broken-reference)\
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

#### types\~UserSettings : `object` <a href="#module_types..usersettings" id="module_types..usersettings"></a>

用户设置信息

**Kind**: inner typedef of [`types`](broken-reference)\
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

#### types\~Event : `string` <a href="#module_types..event" id="module_types..event"></a>

监听事件名称

**Kind**: inner typedef of [`types`](broken-reference)

#### types\~EventCallback : `function` <a href="#module_types..eventcallback" id="module_types..eventcallback"></a>

监听事件回调

**Kind**: inner typedef of [`types`](broken-reference)

| Param | Type                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Description |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- |
| res   | [`flooNotice`](broken-reference) \| [`flooError`](broken-reference) \| [`loginFail`](broken-reference) \| [`loginSuccess`](broken-reference) \| [`onGroupListUpdate`](broken-reference) \| [`onGroupMemberChanged`](broken-reference) \| [`onGroupMessage`](broken-reference) \| [`onInputStatusMessage`](broken-reference) \| [`onMentionMessage`](broken-reference) \| [`onMessageCanceled`](broken-reference) \| [`onMessageDeleted`](broken-reference) \| [`onMessageRecalled`](broken-reference) \| [`onMessageStatusChanged`](broken-reference) \| [`onReceiveHistoryMsg`](broken-reference) \| [`onRosterInfoUpdate`](broken-reference) \| [`onRosterListUpdate`](broken-reference) \| [`onRosterMessage`](broken-reference) \| [`onSendingMessageStatusChanged`](broken-reference) \| [`onUnreadChange`](broken-reference) \| [`recentlistUpdate`](broken-reference) \| [`onGroupCreated`](broken-reference) \| [`onGroupDestoryed`](broken-reference) \| [`onGroupJoined`](broken-reference) \| [`onGroupApplyAccepted`](broken-reference) \| [`onGroupApplyDeclined`](broken-reference) \| [`onGroupBaned`](broken-reference) \| [`onGroupUnbaned`](broken-reference) | 事件结果        |

### flooim <a href="#module_flooim" id="module_flooim"></a>

* [flooim](broken-reference)
  * [.flooim(config)](broken-reference) ⇒ `object`
  * [.login(opt)](broken-reference)
  * [.qrlogin(opt)](broken-reference)
  * [.tokenLogin(opt)](broken-reference)
  * [.idLogin(opt)](broken-reference)
  * [.isLogin()](broken-reference) ⇒ `boolean`
  * [.on(options, ext)](broken-reference)
  * [.off(options, ext)](broken-reference)
  * [.logout()](broken-reference)

#### flooim.flooim(config) ⇒ `object` <a href="#module_flooim.flooim" id="module_flooim.flooim"></a>

初始化SDK

**Kind**: static method of [`flooim`](broken-reference)\
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

#### flooim.login(opt) <a href="#module_flooim.login" id="module_flooim.login"></a>

登录

**Kind**: static method of [`flooim`](broken-reference)

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| opt          | `object` |             |
| opt.name     | `string` | 用户名         |
| opt.password | `string` | 密码          |

#### flooim.qrlogin(opt) <a href="#module_flooim.qrlogin" id="module_flooim.qrlogin"></a>

二维码登录

**Kind**: static method of [`flooim`](broken-reference)

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| opt          | `object` |             |
| opt.user\_id | `number` | 用户ID        |
| opt.password | `string` | 密码          |

#### flooim.tokenLogin(opt) <a href="#module_flooim.tokenlogin" id="module_flooim.tokenlogin"></a>

token登录

**Kind**: static method of [`flooim`](broken-reference)

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| opt          | `object` |             |
| opt.user\_id | `number` | 用户ID        |
| opt.token    | `string` | Token       |

#### flooim.idLogin(opt) <a href="#module_flooim.idlogin" id="module_flooim.idlogin"></a>

使用用户ID和密码登录

**Kind**: static method of [`flooim`](broken-reference)

| Param        | Type     | Description |
| ------------ | -------- | ----------- |
| opt          | `object` |             |
| opt.user\_id | `number` | 用户ID        |
| opt.password | `string` | 密码          |

#### flooim.isLogin() ⇒ `boolean` <a href="#module_flooim.islogin" id="module_flooim.islogin"></a>

是否已登录

**Kind**: static method of [`flooim`](broken-reference)\
**Returns**: `boolean` - 是否已登录

#### flooim.on(options, ext) <a href="#module_flooim.on" id="module_flooim.on"></a>

事件监听

**Kind**: static method of [`flooim`](broken-reference)

| Param   | Type                                                                                           | Description             |
| ------- | ---------------------------------------------------------------------------------------------- | ----------------------- |
| options | [`Event`](broken-reference) \| `Object.<module:types`~~`Event, module:types`~~`EventCallback>` | 可以为事件名，也可以为事件名和事件回调     |
| ext     | [`EventCallback`](broken-reference) \| `undefined`                                             | 事件回调，只有options为事件名时需要设置 |

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

#### flooim.off(options, ext) <a href="#module_flooim.off" id="module_flooim.off"></a>

取消监听

**Kind**: static method of [`flooim`](broken-reference)

| Param   | Type                                                                                           | Description             |
| ------- | ---------------------------------------------------------------------------------------------- | ----------------------- |
| options | [`Event`](broken-reference) \| `Object.<module:types`~~`Event, module:types`~~`EventCallback>` | 可以为事件名，也可以为事件名和事件回调     |
| ext     | [`EventCallback`](broken-reference) \| `undefined`                                             | 事件回调，只有options为事件名时需要设置 |

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

#### flooim.logout() <a href="#module_flooim.logout" id="module_flooim.logout"></a>

退出账户

**Kind**: static method of [`flooim`](broken-reference)
