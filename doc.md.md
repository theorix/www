## Modules

<dl>
<dt><a href="#module_groupManage">groupManage</a></dt>
<dd><p>群管理</p>
</dd>
<dt><a href="#module_rosterManage">rosterManage</a></dt>
<dd><p>好友管理</p>
</dd>
<dt><a href="#module_sysManage">sysManage</a></dt>
<dd></dd>
<dt><a href="#module_userManage">userManage</a></dt>
<dd></dd>
<dt><a href="#module_types">types</a></dt>
<dd></dd>
<dt><a href="#module_flooim">flooim</a></dt>
<dd></dd>
</dl>

# groupManage {#module_groupManage}
群管理


* [groupManage](#module_groupManage)
    * [.asyncGetGroupInfo(group_id, froce)](#module_groupManage.asyncGetGroupInfo) ⇒ [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..GroupInfoAndSettings)
    * [.asyncGetJoinedGroups(froce)](#module_groupManage.asyncGetJoinedGroups) ⇒ <code>Promise.&lt;Array.&lt;number&gt;&gt;</code>
    * [.openGroup(group_id)](#module_groupManage.openGroup)
    * [.getAllGroupDetail()](#module_groupManage.getAllGroupDetail) ⇒ <code>Object.&lt;number, module:types~GroupInfoAndSettings&gt;</code>
    * [.asyncGetGroupMembers(group_id)](#module_groupManage.asyncGetGroupMembers) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code>
    * [.getGroupMembers(group_id)](#module_groupManage.getGroupMembers) ⇒ [<code>Array.&lt;GroupMember&gt;</code>](#module_types..GroupMember)
    * [.asyncGetGroupListDetail(gids)](#module_groupManage.asyncGetGroupListDetail) ⇒ <code>Promise.&lt;Array.&lt;module:types~BriefGroupInfoAndSettings&gt;&gt;</code>
    * [.getGruopMessage(gid)](#module_groupManage.getGruopMessage) ⇒ [<code>Array.&lt;Meta&gt;</code>](#module_types..Meta)
    * [.asyncGetInfo(params)](#module_groupManage.asyncGetInfo) ⇒ [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..GroupInfoAndSettings)
    * [.asyncGetMemberList(param)](#module_groupManage.asyncGetMemberList) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code>
    * [.readGroupMessage(group_id, mid)](#module_groupManage.readGroupMessage)
    * [.recallMessage(uid, mid)](#module_groupManage.recallMessage)
    * [.getUnreadCount(gid)](#module_groupManage.getUnreadCount) ⇒ <code>number</code>
    * [.asyncGetAdminList(params)](#module_groupManage.asyncGetAdminList) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code>
    * [.asyncAdminAdd(params)](#module_groupManage.asyncAdminAdd) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code>
    * [.asyncAdminRemove(params)](#module_groupManage.asyncAdminRemove) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code>
    * [.asyncGetAnouncementById(params)](#module_groupManage.asyncGetAnouncementById) ⇒ [<code>Promise.&lt;GroupAnnouncement&gt;</code>](#module_types..GroupAnnouncement)
    * [.asyncAnouncementDelete(params)](#module_groupManage.asyncAnouncementDelete) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncAnnouncementEdit(params)](#module_groupManage.asyncAnnouncementEdit) ⇒ [<code>Promise.&lt;GroupAnnouncement&gt;</code>](#module_types..GroupAnnouncement)
    * [.asyncGetAnnouncementList(params)](#module_groupManage.asyncGetAnnouncementList) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupAnnouncement&gt;&gt;</code>
    * [.asyncCreate(params)](#module_groupManage.asyncCreate) ⇒ [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..GroupInfoAndSettings)
    * [.asyncDestroy(params)](#module_groupManage.asyncDestroy) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateAvatar(params)](#module_groupManage.asyncUpdateAvatar) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateDescription(params)](#module_groupManage.asyncUpdateDescription) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateExt(params)](#module_groupManage.asyncUpdateExt) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateName(params)](#module_groupManage.asyncUpdateName) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncGroupMsgMutemode(params)](#module_groupManage.asyncGroupMsgMutemode) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncGroupBannedList(params)](#module_groupManage.asyncGroupBannedList) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMemberBanned&gt;&gt;</code>
    * [.asyncGroupBab(params)](#module_groupManage.asyncGroupBab) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code>
    * [.asyncGroupUnban(params)](#module_groupManage.asyncGroupUnban) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code>
    * [.asyncGetSettings(group_id)](#module_groupManage.asyncGetSettings) ⇒ [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..GroupInfoAndSettings)
    * [.asyncUpdateAllowMemberInvitation(params)](#module_groupManage.asyncUpdateAllowMemberInvitation) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateAllowMemberModify(params)](#module_groupManage.asyncUpdateAllowMemberModify) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateEnableReadack(params)](#module_groupManage.asyncUpdateEnableReadack) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateHistoryVisible(params)](#module_groupManage.asyncUpdateHistoryVisible) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateRequireadminapproval(params)](#module_groupManage.asyncUpdateRequireadminapproval) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncBanAll(params)](#module_groupManage.asyncBanAll) ⇒ [<code>Promise.&lt;GroupBanAllResponse&gt;</code>](#module_types..GroupBanAllResponse)
    * [.asyncUnBanAll(params)](#module_groupManage.asyncUnBanAll) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncOwnerTransfer(params)](#module_groupManage.asyncOwnerTransfer) ⇒ [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..GroupUserRelationResponse)
    * [.asyncGetUserJoined(params)](#module_groupManage.asyncGetUserJoined) ⇒ <code>Promise.&lt;Array.&lt;number&gt;&gt;</code>
    * [.asyncApply(params)](#module_groupManage.asyncApply) ⇒ [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..GroupUserRelationResponse)
    * [.asyncApplyHandle(params)](#module_groupManage.asyncApplyHandle) ⇒ [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..GroupUserRelationResponse)
    * [.asyncGroupBockedlist(params)](#module_groupManage.asyncGroupBockedlist) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupBlockedListItem&gt;&gt;</code>
    * [.asyncGroupBlock(params)](#module_groupManage.asyncGroupBlock) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code>
    * [.asyncGroupUnblock(params)](#module_groupManage.asyncGroupUnblock) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code>
    * [.asyncKick(params)](#module_groupManage.asyncKick) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code>
    * [.asyncGetInvitationList()](#module_groupManage.asyncGetInvitationList) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupInvitation&gt;&gt;</code>
    * [.asyncInvite(params)](#module_groupManage.asyncInvite) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code>
    * [.asyncInviteHandle(params)](#module_groupManage.asyncInviteHandle) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncGetMemberDisplayName(params)](#module_groupManage.asyncGetMemberDisplayName) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code>
    * [.asyncLeave(params)](#module_groupManage.asyncLeave) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateDisplayName(params)](#module_groupManage.asyncUpdateDisplayName) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asncGetApplicationList(params)](#module_groupManage.asncGetApplicationList) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupApplication&gt;&gt;</code>
    * [.asyncGetFileList(params)](#module_groupManage.asyncGetFileList) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupSharedFile&gt;&gt;</code>
    * [.asyncFileDelete(params)](#module_groupManage.asyncFileDelete) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupSharedFileResponse&gt;&gt;</code>
    * [.asyncFileUpload(params)](#module_groupManage.asyncFileUpload) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupSharedFile&gt;&gt;</code>

## groupManage.asyncGetGroupInfo(group_id, froce) ⇒ [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..GroupInfoAndSettings) {#module_groupManage.asyncGetGroupInfo}
获取群信息

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..GroupInfoAndSettings) - 群信息  

| Param | Type | Description |
| --- | --- | --- |
| group_id | <code>number</code> | 群ID |
| froce | <code>boolean</code> | 是否强制从服务器拉取： true - 从服务器拉取， false - 优先从本地存储获取 |

## groupManage.asyncGetJoinedGroups(froce) ⇒ <code>Promise.&lt;Array.&lt;number&gt;&gt;</code> {#module_groupManage.asyncGetJoinedGroups}
获取加入的群组

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;number&gt;&gt;</code> - 群组ID列表  

| Param | Type | Description |
| --- | --- | --- |
| froce | <code>boolean</code> | 是否强制从服务器拉取： true - 从服务器拉取， false - 优先从本地存储获取 |

## groupManage.openGroup(group_id) {#module_groupManage.openGroup}
打开群组， 此方法会准备群组聊天界面的一些必备信息。

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  

| Param | Type | Description |
| --- | --- | --- |
| group_id | <code>number</code> | 群组ID |

## groupManage.getAllGroupDetail() ⇒ <code>Object.&lt;number, module:types~GroupInfoAndSettings&gt;</code> {#module_groupManage.getAllGroupDetail}
获取缓存的所有群组详情

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Object.&lt;number, module:types~GroupInfoAndSettings&gt;</code> - 群组详情  
## groupManage.asyncGetGroupMembers(group_id) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code> {#module_groupManage.asyncGetGroupMembers}
获取群组成员（异步）

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code> - 群成员列表  

| Param | Type | Description |
| --- | --- | --- |
| group_id | <code>number</code> | 群组ID |

## groupManage.getGroupMembers(group_id) ⇒ [<code>Array.&lt;GroupMember&gt;</code>](#module_types..GroupMember) {#module_groupManage.getGroupMembers}
获取群组成员（同步）

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: [<code>Array.&lt;GroupMember&gt;</code>](#module_types..GroupMember) - 群成员列表  

| Param | Type | Description |
| --- | --- | --- |
| group_id | <code>number</code> | 群组ID |

## groupManage.asyncGetGroupListDetail(gids) ⇒ <code>Promise.&lt;Array.&lt;module:types~BriefGroupInfoAndSettings&gt;&gt;</code> {#module_groupManage.asyncGetGroupListDetail}
按id获取群组详情

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~BriefGroupInfoAndSettings&gt;&gt;</code> - 群组详情列表  

| Param | Type | Description |
| --- | --- | --- |
| gids | <code>Array.&lt;number&gt;</code> | 群组ID列表 |

## groupManage.getGruopMessage(gid) ⇒ [<code>Array.&lt;Meta&gt;</code>](#module_types..Meta) {#module_groupManage.getGruopMessage}
获取群消息

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: [<code>Array.&lt;Meta&gt;</code>](#module_types..Meta) - 群消息列表  

| Param | Type | Description |
| --- | --- | --- |
| gid | <code>number</code> | 群ID |

## groupManage.asyncGetInfo(params) ⇒ [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..GroupInfoAndSettings) {#module_groupManage.asyncGetInfo}
获取群组详情

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..GroupInfoAndSettings) - 群组详情  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.asyncGetMemberList(param) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code> {#module_groupManage.asyncGetMemberList}
获取群成员列表

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code> - 群成员列表  

| Param | Type | Description |
| --- | --- | --- |
| param | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.readGroupMessage(group_id, mid) {#module_groupManage.readGroupMessage}
将群消息设置已读

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  

| Param | Type | Description |
| --- | --- | --- |
| group_id | <code>number</code> | 群组ID |
| mid | <code>number</code> | 消息ID |

## groupManage.recallMessage(uid, mid) {#module_groupManage.recallMessage}
撤回消息

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  

| Param | Type | Description |
| --- | --- | --- |
| uid | <code>number</code> | 群组ID |
| mid | <code>number</code> | 消息ID |

## groupManage.getUnreadCount(gid) ⇒ <code>number</code> {#module_groupManage.getUnreadCount}
获取群未读消息数

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>number</code> - 未读消息数  

| Param | Type | Description |
| --- | --- | --- |
| gid | <code>number</code> | 群组ID |

## groupManage.asyncGetAdminList(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code> {#module_groupManage.asyncGetAdminList}
获取群管理员列表

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code> - 群管理员列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.asyncAdminAdd(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> {#module_groupManage.asyncAdminAdd}
群添加管理员

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> - 结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_list | <code>Array.&lt;number&gt;</code> | 群成员列表 |

## groupManage.asyncAdminRemove(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> {#module_groupManage.asyncAdminRemove}
移除管理员

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> - 结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_list | <code>Array.&lt;number&gt;</code> | 群成员列表 |

## groupManage.asyncGetAnouncementById(params) ⇒ [<code>Promise.&lt;GroupAnnouncement&gt;</code>](#module_types..GroupAnnouncement) {#module_groupManage.asyncGetAnouncementById}
获取群公告详情

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: [<code>Promise.&lt;GroupAnnouncement&gt;</code>](#module_types..GroupAnnouncement) - 群公告详情  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.announcement_id | <code>Array.&lt;number&gt;</code> | 公告ID |

## groupManage.asyncAnouncementDelete(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupManage.asyncAnouncementDelete}
删除群公告

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.announcement_id | <code>Array.&lt;number&gt;</code> | 公告ID |

## groupManage.asyncAnnouncementEdit(params) ⇒ [<code>Promise.&lt;GroupAnnouncement&gt;</code>](#module_types..GroupAnnouncement) {#module_groupManage.asyncAnnouncementEdit}
编辑群公告

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: [<code>Promise.&lt;GroupAnnouncement&gt;</code>](#module_types..GroupAnnouncement) - 群公告详情  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.title | <code>string</code> | 公告标题 |
| params.content | <code>string</code> | 公告内容 |

## groupManage.asyncGetAnnouncementList(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupAnnouncement&gt;&gt;</code> {#module_groupManage.asyncGetAnnouncementList}
群公告列表

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupAnnouncement&gt;&gt;</code> - 群公告详情列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.asyncCreate(params) ⇒ [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..GroupInfoAndSettings) {#module_groupManage.asyncCreate}
创建群组

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..GroupInfoAndSettings) - 群详情  

| Param | Type | Description |
| --- | --- | --- |
| params | [<code>GroupInfoRequest</code>](#module_types..GroupInfoRequest) | 请求参数 |

## groupManage.asyncDestroy(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupManage.asyncDestroy}
解散群组

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.asyncUpdateAvatar(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupManage.asyncUpdateAvatar}
更新群头像

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>string</code> | 头像地址 |

## groupManage.asyncUpdateDescription(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupManage.asyncUpdateDescription}
更新群描述

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>string</code> | 群组描述 |

## groupManage.asyncUpdateExt(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupManage.asyncUpdateExt}
更新群扩展信息

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>string</code> | 扩展信息 |

## groupManage.asyncUpdateName(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupManage.asyncUpdateName}
更新群名称

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>string</code> | 群名称 |

## groupManage.asyncGroupMsgMutemode(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupManage.asyncGroupMsgMutemode}
设置群消息免打扰情况

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.msg_mute_mode | <code>number</code> | 群消息屏蔽模式: 0 - 表示不屏蔽, 1 - 表示屏蔽本地消息通知, 2 - 表示屏蔽消息，不接收消息 |

## groupManage.asyncGroupBannedList(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMemberBanned&gt;&gt;</code> {#module_groupManage.asyncGroupBannedList}
获取群禁言列表

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupMemberBanned&gt;&gt;</code> - 禁言成员列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.asyncGroupBab(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> {#module_groupManage.asyncGroupBab}
禁言群成员

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> - 请求结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | [<code>GroupBannedMemberRequest</code>](#module_types..GroupBannedMemberRequest) | 请求参数 |

## groupManage.asyncGroupUnban(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> {#module_groupManage.asyncGroupUnban}
解除成员禁言

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> - 请求结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_list | <code>Array.&lt;number&gt;</code> | 群成员列表 |

## groupManage.asyncGetSettings(group_id) ⇒ [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..GroupInfoAndSettings) {#module_groupManage.asyncGetSettings}
获取群设置

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..GroupInfoAndSettings) - 群设置  

| Param | Type | Description |
| --- | --- | --- |
| group_id | <code>number</code> | 群ID |

## groupManage.asyncUpdateAllowMemberInvitation(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupManage.asyncUpdateAllowMemberInvitation}
设置群成员是否可以邀请

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>boolean</code> | 群成员邀请设置: false - 不允许邀请, true - 允许邀请(默认) |

## groupManage.asyncUpdateAllowMemberModify(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupManage.asyncUpdateAllowMemberModify}
设置群成员是否可以修改群信息

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>boolean</code> | 群成员修改群信息设置:  false - 群成员不能修改群信息(默认), true - 群成员可以修改群信息 |

## groupManage.asyncUpdateEnableReadack(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupManage.asyncUpdateEnableReadack}
设置群是否开启已读模式

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>boolean</code> | 是否开启群消息已读功能:  false - 不开启, true - 开启 |

## groupManage.asyncUpdateHistoryVisible(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupManage.asyncUpdateHistoryVisible}
设置群历史是否可见

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>boolean</code> | 设置群历史是否可见:  false - 不可见, true - 可见 |

## groupManage.asyncUpdateRequireadminapproval(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupManage.asyncUpdateRequireadminapproval}
设置入群是否需要申请

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.apply_approval | <code>boolean</code> | 入群申请审批设置, 0:同意所有申请 1:需要管理员确认 2:拒绝所有申请 |

## groupManage.asyncBanAll(params) ⇒ [<code>Promise.&lt;GroupBanAllResponse&gt;</code>](#module_types..GroupBanAllResponse) {#module_groupManage.asyncBanAll}
全员禁言，只允许管理员发消息

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: [<code>Promise.&lt;GroupBanAllResponse&gt;</code>](#module_types..GroupBanAllResponse) - 结果  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.duration | <code>number</code> | 禁言时长，单位为分钟,int64 |
| params.group_id | <code>number</code> | 群id,int64 |

## groupManage.asyncUnBanAll(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupManage.asyncUnBanAll}
取消全员禁言

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群id,int64 |

## groupManage.asyncOwnerTransfer(params) ⇒ [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..GroupUserRelationResponse) {#module_groupManage.asyncOwnerTransfer}
更换群主

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..GroupUserRelationResponse) - 结果  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.new_owner | <code>number</code> | 新群主的用户ID |

## groupManage.asyncGetUserJoined(params) ⇒ <code>Promise.&lt;Array.&lt;number&gt;&gt;</code> {#module_groupManage.asyncGetUserJoined}
获取用户的群组列表

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;number&gt;&gt;</code> - 群ID的列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数, 空对象 |

## groupManage.asyncApply(params) ⇒ [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..GroupUserRelationResponse) {#module_groupManage.asyncApply}
申请加入群

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..GroupUserRelationResponse) - 结果  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.reason | <code>string</code> | 申请入群原因 |

## groupManage.asyncApplyHandle(params) ⇒ [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..GroupUserRelationResponse) {#module_groupManage.asyncApplyHandle}
处理用户的入群申请

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..GroupUserRelationResponse) - 结果  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_id | <code>number</code> | 用户ID |
| params.approval | <code>boolean</code> | 审批结果：true为同意，false为拒绝 |

## groupManage.asyncGroupBockedlist(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupBlockedListItem&gt;&gt;</code> {#module_groupManage.asyncGroupBockedlist}
获取群黑名单

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupBlockedListItem&gt;&gt;</code> - 群黑名单列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.asyncGroupBlock(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> {#module_groupManage.asyncGroupBlock}
将成员加入黑名单

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> - 结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_list | <code>Array.&lt;number&gt;</code> | 群成员列表 |

## groupManage.asyncGroupUnblock(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> {#module_groupManage.asyncGroupUnblock}
解除黑名单

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> - 结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_list | <code>Array.&lt;number&gt;</code> | 群成员列表 |

## groupManage.asyncKick(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> {#module_groupManage.asyncKick}
踢出群组

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> - 结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_list | <code>Array.&lt;number&gt;</code> | 群成员列表 |

## groupManage.asyncGetInvitationList() ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupInvitation&gt;&gt;</code> {#module_groupManage.asyncGetInvitationList}
获取群邀请列表

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupInvitation&gt;&gt;</code> - 群邀请列表  
## groupManage.asyncInvite(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> {#module_groupManage.asyncInvite}
邀请成员加入群

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> - 结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_list | <code>Array.&lt;number&gt;</code> | 群成员列表 |

## groupManage.asyncInviteHandle(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupManage.asyncInviteHandle}
处理群邀请

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_id | <code>number</code> | 用户ID |
| params.approval | <code>boolean</code> | 审批结果：true为同意，false为拒绝 |

## groupManage.asyncGetMemberDisplayName(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code> {#module_groupManage.asyncGetMemberDisplayName}
批量获取群成员的群名片

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code> - 群成员列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_list | <code>Array.&lt;number&gt;</code> | 群成员列表 |

## groupManage.asyncLeave(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupManage.asyncLeave}
退出群

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.asyncUpdateDisplayName(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupManage.asyncUpdateDisplayName}
修改群名片

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>string</code> | 新名片 |

## groupManage.asncGetApplicationList(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupApplication&gt;&gt;</code> {#module_groupManage.asncGetApplicationList}
获取群申请列表

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupApplication&gt;&gt;</code> - 群申请列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_list | <code>Array.&lt;number&gt;</code> | 群列表 |

## groupManage.asyncGetFileList(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupSharedFile&gt;&gt;</code> {#module_groupManage.asyncGetFileList}
获取群文件列表

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupSharedFile&gt;&gt;</code> - 群文件列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.asyncFileDelete(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupSharedFileResponse&gt;&gt;</code> {#module_groupManage.asyncFileDelete}
删除群文件

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupSharedFileResponse&gt;&gt;</code> - 结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.file_list | <code>Array.&lt;number&gt;</code> | 文件ID列表 |

## groupManage.asyncFileUpload(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupSharedFile&gt;&gt;</code> {#module_groupManage.asyncFileUpload}
上传群文件

**Kind**: static method of [<code>groupManage</code>](#module_groupManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupSharedFile&gt;&gt;</code> - 群文件列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群id,int64 |
| params.name | <code>string</code> | 文件名称 |
| params.size | <code>number</code> | 文件大小,int64 |
| params.type | <code>string</code> | 文件类型 |
| params.url | <code>string</code> | 文件url |

# rosterManage {#module_rosterManage}
好友管理


* [rosterManage](#module_rosterManage)
    * [.asyncGetRosterIdList(force)](#module_rosterManage.asyncGetRosterIdList) ⇒ <code>Promise.&lt;Array.&lt;number&gt;&gt;</code>
    * [.asyncGetRosterInfo(roster_id, force)](#module_rosterManage.asyncGetRosterInfo) ⇒ [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..RosterItem)
    * [.asyncRegester(opt)](#module_rosterManage.asyncRegester) ⇒ [<code>Promise.&lt;UserSettings&gt;</code>](#module_types..UserSettings)
    * [.asyncDeleteRoster(param)](#module_rosterManage.asyncDeleteRoster) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asnycGetRosterListDetailByIds(roster_ids)](#module_rosterManage.asnycGetRosterListDetailByIds) ⇒ <code>Promise.&lt;Array.&lt;module:types~RosterItem&gt;&gt;</code>
    * [.getAllRosterDetail()](#module_rosterManage.getAllRosterDetail) ⇒ [<code>Array.&lt;RosterItem&gt;</code>](#module_types..RosterItem)
    * [.asyncGetUserProfile(force)](#module_rosterManage.asyncGetUserProfile) ⇒ [<code>Promise.&lt;UserProfile&gt;</code>](#module_types..UserProfile)
    * [.getRosterMessageByRid(uid)](#module_rosterManage.getRosterMessageByRid) ⇒ [<code>Array.&lt;Meta&gt;</code>](#module_types..Meta)
    * [.readRosterMessage(roster_id, mid)](#module_rosterManage.readRosterMessage)
    * [.recallMessage(uid, mid)](#module_rosterManage.recallMessage)
    * [.unreadMessage(uid, mid)](#module_rosterManage.unreadMessage)
    * [.deleteMessage(uid, mid)](#module_rosterManage.deleteMessage)
    * [.getRosterInfo(rid)](#module_rosterManage.getRosterInfo) ⇒ [<code>RosterItem</code>](#module_types..RosterItem)
    * [.getUnreadCount(uid)](#module_rosterManage.getUnreadCount) ⇒ <code>number</code>
    * [.asyncGetApplyList(params)](#module_rosterManage.asyncGetApplyList) ⇒ <code>Promise.&lt;Array.&lt;module:types~RosterApplication&gt;&gt;</code>
    * [.asyncGetBlockedlist(params)](#module_rosterManage.asyncGetBlockedlist) ⇒ <code>Promise.&lt;Array.&lt;number&gt;&gt;</code>
    * [.asyncBlockeAdd(params)](#module_rosterManage.asyncBlockeAdd) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncBlockeRemove(params)](#module_rosterManage.asyncBlockeRemove) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncApply(params)](#module_rosterManage.asyncApply) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncAccept(params)](#module_rosterManage.asyncAccept) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncDecline(params)](#module_rosterManage.asyncDecline) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateRosterExt(params)](#module_rosterManage.asyncUpdateRosterExt) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncSearchRosterByName(params)](#module_rosterManage.asyncSearchRosterByName) ⇒ [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..RosterItem)
    * [.asyncSearchRosterById(params)](#module_rosterManage.asyncSearchRosterById) ⇒ [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..RosterItem)

## rosterManage.asyncGetRosterIdList(force) ⇒ <code>Promise.&lt;Array.&lt;number&gt;&gt;</code> {#module_rosterManage.asyncGetRosterIdList}
获取好友id列表

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: <code>Promise.&lt;Array.&lt;number&gt;&gt;</code> - 用户ID列表  

| Param | Type | Description |
| --- | --- | --- |
| force | <code>boolean</code> | 是否强制从服务器拉取：true - 从服务器获取， false - 从本地存储获取 |

## rosterManage.asyncGetRosterInfo(roster_id, force) ⇒ [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..RosterItem) {#module_rosterManage.asyncGetRosterInfo}
获取好友信息

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..RosterItem) - 好友信息  

| Param | Type | Description |
| --- | --- | --- |
| roster_id | <code>number</code> | 好友ID |
| force | <code>boolean</code> | 是否强制从服务器拉取： true - 从服务器拉取， false - 优先从本地存储获取 |

## rosterManage.asyncRegester(opt) ⇒ [<code>Promise.&lt;UserSettings&gt;</code>](#module_types..UserSettings) {#module_rosterManage.asyncRegester}
用户注册

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: [<code>Promise.&lt;UserSettings&gt;</code>](#module_types..UserSettings) - 用户设置  

| Param | Type | Description |
| --- | --- | --- |
| opt | <code>object</code> | 用户信息 |
| opt.username | <code>string</code> | 用户名 |
| opt.password | <code>string</code> | 密码 |

## rosterManage.asyncDeleteRoster(param) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_rosterManage.asyncDeleteRoster}
删除好友

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 请求结果  

| Param | Type | Description |
| --- | --- | --- |
| param | <code>object</code> | 参数 |
| param.user_id | <code>number</code> | 好友的用户ID |

## rosterManage.asnycGetRosterListDetailByIds(roster_ids) ⇒ <code>Promise.&lt;Array.&lt;module:types~RosterItem&gt;&gt;</code> {#module_rosterManage.asnycGetRosterListDetailByIds}
根据id列表获取用户详细信息

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~RosterItem&gt;&gt;</code> - 用户详细信息列表  

| Param | Type | Description |
| --- | --- | --- |
| roster_ids | <code>Array.&lt;number&gt;</code> | 用户ID列表 |

## rosterManage.getAllRosterDetail() ⇒ [<code>Array.&lt;RosterItem&gt;</code>](#module_types..RosterItem) {#module_rosterManage.getAllRosterDetail}
获取缓存的所有用户详细信息

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: [<code>Array.&lt;RosterItem&gt;</code>](#module_types..RosterItem) - 用户详细信息列表  
## rosterManage.asyncGetUserProfile(force) ⇒ [<code>Promise.&lt;UserProfile&gt;</code>](#module_types..UserProfile) {#module_rosterManage.asyncGetUserProfile}
获取自己的用户信息

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: [<code>Promise.&lt;UserProfile&gt;</code>](#module_types..UserProfile) - 用户信息  

| Param | Type | Description |
| --- | --- | --- |
| force | <code>boolean</code> | 是否强制从服务器拉取： true - 从服务器拉取， false - 优先从本地存储获取 |

## rosterManage.getRosterMessageByRid(uid) ⇒ [<code>Array.&lt;Meta&gt;</code>](#module_types..Meta) {#module_rosterManage.getRosterMessageByRid}
根据会话ID获取聊天消息

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: [<code>Array.&lt;Meta&gt;</code>](#module_types..Meta) - 聊天消息列表  

| Param | Type | Description |
| --- | --- | --- |
| uid | <code>number</code> | 会话ID |

## rosterManage.readRosterMessage(roster_id, mid) {#module_rosterManage.readRosterMessage}
修改消息状态为已读

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  

| Param | Type | Description |
| --- | --- | --- |
| roster_id | <code>number</code> | 会话ID |
| mid | <code>number</code> | 消息ID |

## rosterManage.recallMessage(uid, mid) {#module_rosterManage.recallMessage}
撤回消息，只能撤回5分钟内的

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  

| Param | Type | Description |
| --- | --- | --- |
| uid | <code>number</code> | 会话ID |
| mid | <code>number</code> | 消息ID |

## rosterManage.unreadMessage(uid, mid) {#module_rosterManage.unreadMessage}
设置消息成未读

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  

| Param | Type | Description |
| --- | --- | --- |
| uid | <code>number</code> | 会话ID |
| mid | <code>number</code> | 消息ID |

## rosterManage.deleteMessage(uid, mid) {#module_rosterManage.deleteMessage}
删除消息

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  

| Param | Type | Description |
| --- | --- | --- |
| uid | <code>number</code> | 会话ID |
| mid | <code>number</code> | 消息ID |

## rosterManage.getRosterInfo(rid) ⇒ [<code>RosterItem</code>](#module_types..RosterItem) {#module_rosterManage.getRosterInfo}
获取好友信息

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: [<code>RosterItem</code>](#module_types..RosterItem) - 好友信息  

| Param | Type | Description |
| --- | --- | --- |
| rid | <code>number</code> | 好友ID |

## rosterManage.getUnreadCount(uid) ⇒ <code>number</code> {#module_rosterManage.getUnreadCount}
获取指定会话的未读数

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: <code>number</code> - 未读数  

| Param | Type | Description |
| --- | --- | --- |
| uid | <code>number</code> | 会话IID |

## rosterManage.asyncGetApplyList(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~RosterApplication&gt;&gt;</code> {#module_rosterManage.asyncGetApplyList}
获取好友申请列表

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~RosterApplication&gt;&gt;</code> - 好友申请列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.cursor | <code>number</code> | 从哪开始获取：可以传空字符串表示从头开始取 |

## rosterManage.asyncGetBlockedlist(params) ⇒ <code>Promise.&lt;Array.&lt;number&gt;&gt;</code> {#module_rosterManage.asyncGetBlockedlist}
获取黑名单

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: <code>Promise.&lt;Array.&lt;number&gt;&gt;</code> - 用户ID列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数：空对象 |

## rosterManage.asyncBlockeAdd(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_rosterManage.asyncBlockeAdd}
加入黑名单

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.user_id | <code>number</code> | 用户ID |

## rosterManage.asyncBlockeRemove(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_rosterManage.asyncBlockeRemove}
移除黑名单

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.user_id | <code>number</code> | 用户ID |

## rosterManage.asyncApply(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_rosterManage.asyncApply}
请求加为好友

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.user_id | <code>number</code> | 用户ID |
| params.alias | <code>string</code> | 备注 |

## rosterManage.asyncAccept(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_rosterManage.asyncAccept}
通过好友申请

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.user_id | <code>number</code> | 用户ID |

## rosterManage.asyncDecline(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_rosterManage.asyncDecline}
拒绝好友申请

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.user_id | <code>number</code> | 用户ID |

## rosterManage.asyncUpdateRosterExt(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_rosterManage.asyncUpdateRosterExt}
修改好友扩展字段

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.user_id | <code>number</code> | 用户ID |
| params.ext | <code>string</code> | 扩展字段 |

## rosterManage.asyncSearchRosterByName(params) ⇒ [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..RosterItem) {#module_rosterManage.asyncSearchRosterByName}
按名称搜索用户

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..RosterItem) - 用户信息  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.username | <code>string</code> | 用户名 |

## rosterManage.asyncSearchRosterById(params) ⇒ [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..RosterItem) {#module_rosterManage.asyncSearchRosterById}
按ID搜索用户

**Kind**: static method of [<code>rosterManage</code>](#module_rosterManage)  
**Returns**: [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..RosterItem) - 用户信息  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.user_id | <code>number</code> | 用户ID |

# sysManage {#module_sysManage}

* [sysManage](#module_sysManage)
    * [.sendRosterMessage(msg)](#module_sysManage.sendRosterMessage) ⇒ <code>number</code>
    * [.sendGroupMessage(msg)](#module_sysManage.sendGroupMessage) ⇒ <code>number</code>
    * [.requireHistoryMessage(uid, sid, amount)](#module_sysManage.requireHistoryMessage)
    * [.sendMentionMessage(params)](#module_sysManage.sendMentionMessage) ⇒ <code>number</code>
    * [.sendInputStatusMessage(uid, status)](#module_sysManage.sendInputStatusMessage) ⇒ <code>number</code>
    * [.forwardMessage(param)](#module_sysManage.forwardMessage) ⇒ <code>number</code>
    * [.getMessageStatus(cid, mid, isGroup)](#module_sysManage.getMessageStatus) ⇒ <code>string</code>
    * [.asyncFileUpload(param)](#module_sysManage.asyncFileUpload) ⇒ [<code>Promise.&lt;FileUploadResult&gt;</code>](#module_types..FileUploadResult)
    * [.getImage(param)](#module_sysManage.getImage) ⇒ <code>string</code>
    * [.deleteConversation(id, other_devices)](#module_sysManage.deleteConversation)
    * [.asyncGetGroupAvatarUploadUrl(params)](#module_sysManage.asyncGetGroupAvatarUploadUrl) ⇒ [<code>Promise.&lt;FileUpload&gt;</code>](#module_types..FileUpload)
    * [.asyncGetFileUploadChatFileUrl(params)](#module_sysManage.asyncGetFileUploadChatFileUrl) ⇒ [<code>Promise.&lt;FileUpload&gt;</code>](#module_types..FileUpload)

## sysManage.sendRosterMessage(msg) ⇒ <code>number</code> {#module_sysManage.sendRosterMessage}
发送单聊消息

**Kind**: static method of [<code>sysManage</code>](#module_sysManage)  
**Returns**: <code>number</code> - 客户端生成的消息ID  

| Param | Type | Description |
| --- | --- | --- |
| msg | <code>object</code> | 消息体 |
| msg.uid | <code>string</code> | 接收者ID |
| msg.content | <code>string</code> | 消息内容 |
| msg.type | <code>string</code> | 消息类型： text - 文本, image - 图片， audio - 语音, video - 视频，file - 文件, location - 位置， command - 命令, forward - 转发 |
| msg.ext | <code>string</code> \| <code>object</code> | 扩展字段 |
| msg.attachment | <code>string</code> \| <code>object</code> | 附件信息 |

## sysManage.sendGroupMessage(msg) ⇒ <code>number</code> {#module_sysManage.sendGroupMessage}
发送群聊消息

**Kind**: static method of [<code>sysManage</code>](#module_sysManage)  
**Returns**: <code>number</code> - 客户端生成的消息ID  

| Param | Type | Description |
| --- | --- | --- |
| msg | <code>object</code> | 发送消息体 |
| msg.gid | <code>string</code> | 群组ID |
| msg.content | <code>string</code> | 消息内容 |
| msg.type | <code>string</code> | 消息类型： text - 文本, image - 图片， audio - 语音, video - 视频，file - 文件, location - 位置， command - 命令, forward - 转发 |
| msg.ext | <code>string</code> \| <code>object</code> | 扩展字段 |
| msg.attachment | <code>string</code> \| <code>object</code> | 附件信息 |
| msg.priority | <code>number</code> | 设置消息的扩散优先级，默认为0。0表示扩散，数字越小扩散的越多。 |

## sysManage.requireHistoryMessage(uid, sid, amount) {#module_sysManage.requireHistoryMessage}
请求历史消息

**Kind**: static method of [<code>sysManage</code>](#module_sysManage)  

| Param | Type | Description |
| --- | --- | --- |
| uid | <code>number</code> | 会话ID |
| sid | <code>number</code> | 消息ID: 从哪个消息向前拉取，传0表示从最新一条消息开始拉取。 |
| amount | <code>number</code> | 拉取的条数 |

## sysManage.sendMentionMessage(params) ⇒ <code>number</code> {#module_sysManage.sendMentionMessage}
群发送&#64;消息

**Kind**: static method of [<code>sysManage</code>](#module_sysManage)  
**Returns**: <code>number</code> - 客户端生成的消息ID  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> |  |
| params.gid | <code>number</code> | 群ID |
| params.txt | <code>string</code> | 消息文本内容 |
| params.mentionAll | <code>boolean</code> | 是否&#64;所有人 |
| params.mentionList | <code>Array.&lt;number&gt;</code> | &#64;的成员ID列表 |
| params.mentionedMessage | <code>string</code> | &#64;消息的显示内容 |
| params.mentionedMessage | <code>string</code> | &#64;消息的推送内容 |
| params.senderNickname | <code>string</code> | 发送者昵称 |

## sysManage.sendInputStatusMessage(uid, status) ⇒ <code>number</code> {#module_sysManage.sendInputStatusMessage}
发送输入状态消息

**Kind**: static method of [<code>sysManage</code>](#module_sysManage)  
**Returns**: <code>number</code> - 客户端生成的消息ID  

| Param | Type | Description |
| --- | --- | --- |
| uid | <code>number</code> | 会话ID |
| status | <code>string</code> | 状态： nothing - 未输入， typing - 正在输入 |

## sysManage.forwardMessage(param) ⇒ <code>number</code> {#module_sysManage.forwardMessage}
转发消息

**Kind**: static method of [<code>sysManage</code>](#module_sysManage)  
**Returns**: <code>number</code> - 客户端生成的消息ID  

| Param | Type | Description |
| --- | --- | --- |
| param | <code>object</code> | 参数 |
| param.uid | <code>number</code> | 接收方用户ID（仅转发单聊时设置） |
| param.gid | <code>number</code> | 接收方群组ID（仅转发群聊时设置） |
| param.mid | <code>number</code> | 要转发的消息ID |

## sysManage.getMessageStatus(cid, mid, isGroup) ⇒ <code>string</code> {#module_sysManage.getMessageStatus}
获取消息的状态

**Kind**: static method of [<code>sysManage</code>](#module_sysManage)  
**Returns**: <code>string</code> - 消息状态:   unread - 未读， delivered - 已投递， read - 已读  

| Param | Type | Default | Description |
| --- | --- | --- | --- |
| cid | <code>number</code> |  | 会话ID |
| mid | <code>number</code> |  | 消息ID |
| isGroup | <code>boolean</code> | <code>false</code> | 是否是群聊 |

## sysManage.asyncFileUpload(param) ⇒ [<code>Promise.&lt;FileUploadResult&gt;</code>](#module_types..FileUploadResult) {#module_sysManage.asyncFileUpload}
上传文件

**Kind**: static method of [<code>sysManage</code>](#module_sysManage)  
**Returns**: [<code>Promise.&lt;FileUploadResult&gt;</code>](#module_types..FileUploadResult) - 文件上传结果  

| Param | Type | Description |
| --- | --- | --- |
| param | <code>object</code> | 参数 |
| param.group_d | <code>number</code> | 群组ID |
| param.toType | <code>number</code> | 接收者类型：rosterAvatar - 用户头像， chat - 聊天文件， groupAvatar - 群头像 |
| param.to_id | <code>number</code> | 接收者ID |
| param.file | <code>File</code> | 文件 |
| param.fileType | <code>string</code> | 文件类型：file - 普通聊天文件, audio - 语音聊天文件(amr格式),image - 图片聊天文件, video - 视频聊天文件, audio-mp3 - 语音聊天文件(mp3格式), shareFile - 普通共享文件, shareAudio - 语音共享文件, shareImage - 图片共享文件, shareVideo - 视频共享文件 |
| param.chatType | <code>number</code> | 聊天类型： roster - 单聊, group - 群聊 |
| param.processCallback | [<code>fileUploadProgress</code>](#module_types..fileUploadProgress) | 上传进度回调 |

## sysManage.getImage(param) ⇒ <code>string</code> {#module_sysManage.getImage}
拼装图片路径

**Kind**: static method of [<code>sysManage</code>](#module_sysManage)  
**Returns**: <code>string</code> - 图片地址  

| Param | Type | Description |
| --- | --- | --- |
| param | <code>object</code> |  |
| param.avatar | <code>string</code> | 文件地址 |
| param.type | <code>string</code> | 类型： roster - 用户, group - 群 |
| param.thumbnail | <code>boolean</code> | 是否缩略图：默认为true |
| param.sdefault | <code>string</code> | 默认图片地址 |

## sysManage.deleteConversation(id, other_devices) {#module_sysManage.deleteConversation}
删除会话

**Kind**: static method of [<code>sysManage</code>](#module_sysManage)  

| Param | Type | Default | Description |
| --- | --- | --- | --- |
| id | <code>number</code> |  | 会话ID |
| other_devices | <code>boolean</code> | <code>true</code> | 是否同时删除其它设备上的会话 |

## sysManage.asyncGetGroupAvatarUploadUrl(params) ⇒ [<code>Promise.&lt;FileUpload&gt;</code>](#module_types..FileUpload) {#module_sysManage.asyncGetGroupAvatarUploadUrl}
获取上传群头像URL

**Kind**: static method of [<code>sysManage</code>](#module_sysManage)  
**Returns**: [<code>Promise.&lt;FileUpload&gt;</code>](#module_types..FileUpload) - 文件上传信息  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## sysManage.asyncGetFileUploadChatFileUrl(params) ⇒ [<code>Promise.&lt;FileUpload&gt;</code>](#module_types..FileUpload) {#module_sysManage.asyncGetFileUploadChatFileUrl}
获取聊天文件上传地址

**Kind**: static method of [<code>sysManage</code>](#module_sysManage)  
**Returns**: [<code>Promise.&lt;FileUpload&gt;</code>](#module_types..FileUpload) - 文件上传信息  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.file_type | <code>number</code> | 文件类型: 100 - 普通聊天文件, 101 - 语音聊天文件(amr格式),102 - 图片聊天文件, 103 - 视频聊天文件, 104 - 语音聊天文件(mp3格式)200 - 普通共享文件, 201 - 语音共享文件, 202 - 图片共享文件, 203 - 视频共享文件 |
| params.to_type | <code>number</code> | 会话类型： 1 - 用户，2 - 群组 |
| params.to_id | <code>number</code> | 会话ID |

# userManage {#module_userManage}

* [userManage](#module_userManage)
    * [.getToken()](#module_userManage.getToken) ⇒ <code>string</code>
    * [.getUid()](#module_userManage.getUid) ⇒ <code>number</code>
    * [.getAppid()](#module_userManage.getAppid) ⇒ <code>string</code>
    * [.getConversationList()](#module_userManage.getConversationList) ⇒ [<code>Array.&lt;ConversationItem&gt;</code>](#module_types..ConversationItem)
    * [.asyncUpdateAvatar(params)](#module_userManage.asyncUpdateAvatar) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateNickName(params)](#module_userManage.asyncUpdateNickName) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncGetProfile()](#module_userManage.asyncGetProfile) ⇒ [<code>Promise.&lt;UserProfile&gt;</code>](#module_types..UserProfile)
    * [.asyncUpdateProfile(params)](#module_userManage.asyncUpdateProfile) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncGetSettings()](#module_userManage.asyncGetSettings) ⇒ [<code>Promise.&lt;UserSettings&gt;</code>](#module_types..UserSettings)
    * [.asyncUpdateSettings(settings)](#module_userManage.asyncUpdateSettings) ⇒ <code>Promise.&lt;boolean&gt;</code>

## userManage.getToken() ⇒ <code>string</code> {#module_userManage.getToken}
获取登录用户的token

**Kind**: static method of [<code>userManage</code>](#module_userManage)  
**Returns**: <code>string</code> - 用户的token  
## userManage.getUid() ⇒ <code>number</code> {#module_userManage.getUid}
获取登录用户的uid

**Kind**: static method of [<code>userManage</code>](#module_userManage)  
**Returns**: <code>number</code> - 用户ID  
## userManage.getAppid() ⇒ <code>string</code> {#module_userManage.getAppid}
获取appid

**Kind**: static method of [<code>userManage</code>](#module_userManage)  
**Returns**: <code>string</code> - APP ID  
## userManage.getConversationList() ⇒ [<code>Array.&lt;ConversationItem&gt;</code>](#module_types..ConversationItem) {#module_userManage.getConversationList}
获取最近会话列表

**Kind**: static method of [<code>userManage</code>](#module_userManage)  
## userManage.asyncUpdateAvatar(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_userManage.asyncUpdateAvatar}
更新头像

**Kind**: static method of [<code>userManage</code>](#module_userManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.avatar | <code>string</code> | 头像 url |

## userManage.asyncUpdateNickName(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_userManage.asyncUpdateNickName}
更新昵称

**Kind**: static method of [<code>userManage</code>](#module_userManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.nick_name | <code>string</code> | 昵称 |

## userManage.asyncGetProfile() ⇒ [<code>Promise.&lt;UserProfile&gt;</code>](#module_types..UserProfile) {#module_userManage.asyncGetProfile}
获取用户profile

**Kind**: static method of [<code>userManage</code>](#module_userManage)  
**Returns**: [<code>Promise.&lt;UserProfile&gt;</code>](#module_types..UserProfile) - 用户信息  
## userManage.asyncUpdateProfile(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_userManage.asyncUpdateProfile}
更新用户profile

**Kind**: static method of [<code>userManage</code>](#module_userManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> |  |
| params.description | <code>string</code> | 描述信息 |
| params.nick_name | <code>string</code> | 昵称 |
| params.private_info | <code>string</code> | 私有信息，仅自己可见 |
| params.public_info | <code>string</code> | 公开信息，好友和陌生人可见 |

## userManage.asyncGetSettings() ⇒ [<code>Promise.&lt;UserSettings&gt;</code>](#module_types..UserSettings) {#module_userManage.asyncGetSettings}
获取用户设置信息

**Kind**: static method of [<code>userManage</code>](#module_userManage)  
**Returns**: [<code>Promise.&lt;UserSettings&gt;</code>](#module_types..UserSettings) - 用户信息  
## userManage.asyncUpdateSettings(settings) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_userManage.asyncUpdateSettings}
修改用户设置

**Kind**: static method of [<code>userManage</code>](#module_userManage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| settings | [<code>UserSettings</code>](#module_types..UserSettings) | 更新的设置 |

# types {#module_types}

* [types](#module_types)
    * ["flooNotice" (res)](#event_flooNotice)
    * ["flooError" (res)](#event_flooError)
    * ["loginFail" (desc)](#event_loginFail)
    * ["loginSuccess" (res)](#event_loginSuccess)
    * ["onGroupListUpdate" (meta)](#event_onGroupListUpdate)
    * ["onGroupMemberChanged" (groupId)](#event_onGroupMemberChanged)
    * ["onGroupMessage" (meta)](#event_onGroupMessage)
    * ["onInputStatusMessage" (res)](#event_onInputStatusMessage)
    * ["onMentionMessage" (meta)](#event_onMentionMessage)
    * ["onMessageCanceled" (res)](#event_onMessageCanceled)
    * ["onMessageDeleted" (res)](#event_onMessageDeleted)
    * ["onMessageRecalled" (res)](#event_onMessageRecalled)
    * ["onMessageStatusChanged" (res)](#event_onMessageStatusChanged)
    * ["onReceiveHistoryMsg" (res)](#event_onReceiveHistoryMsg)
    * ["onRosterInfoUpdate" (res)](#event_onRosterInfoUpdate)
    * ["onRosterListUpdate" (meta)](#event_onRosterListUpdate)
    * ["onRosterMessage" (meta)](#event_onRosterMessage)
    * ["onSendingMessageStatusChanged" (res)](#event_onSendingMessageStatusChanged)
    * ["onUnreadChange" (cid)](#event_onUnreadChange)
    * ["recentlistUpdate"](#event_recentlistUpdate)
    * ["onGroupCreated" (meta)](#event_onGroupCreated)
    * ["onGroupDestoryed" (meta)](#event_onGroupDestoryed)
    * ["onGroupJoined" (meta)](#event_onGroupJoined)
    * ["onGroupApplyAccepted" (meta)](#event_onGroupApplyAccepted)
    * ["onGroupApplyDeclined" (meta)](#event_onGroupApplyDeclined)
    * ["onGroupBaned" (meta)](#event_onGroupBaned)
    * ["onGroupUnbaned" (meta)](#event_onGroupUnbaned)
    * [~RosterItem](#module_types..RosterItem) : <code>object</code>
    * [~UserSettings](#module_types..UserSettings) : <code>object</code>
    * [~UserProfile](#module_types..UserProfile) : <code>object</code>
    * [~Meta](#module_types..Meta) : <code>object</code>
    * [~RosterApplication](#module_types..RosterApplication) : <code>object</code>
    * [~GroupInfoAndSettings](#module_types..GroupInfoAndSettings) : <code>object</code>
    * [~BriefGroupInfoAndSettings](#module_types..BriefGroupInfoAndSettings) : <code>object</code>
    * [~GroupMember](#module_types..GroupMember) : <code>object</code>
    * [~GroupMemberBanned](#module_types..GroupMemberBanned) : <code>object</code>
    * [~GroupUserRelationResponse](#module_types..GroupUserRelationResponse) : <code>object</code>
    * [~GroupAnnouncement](#module_types..GroupAnnouncement) : <code>object</code>
    * [~GroupInfoRequest](#module_types..GroupInfoRequest) : <code>object</code>
    * [~GroupBannedMemberRequest](#module_types..GroupBannedMemberRequest) : <code>object</code>
    * [~GroupBlockedListItem](#module_types..GroupBlockedListItem) : <code>object</code>
    * [~GroupInvitation](#module_types..GroupInvitation) : <code>object</code>
    * [~GroupApplication](#module_types..GroupApplication) : <code>object</code>
    * [~GroupSharedFile](#module_types..GroupSharedFile) : <code>object</code>
    * [~GroupSharedFileResponse](#module_types..GroupSharedFileResponse) : <code>object</code>
    * [~GroupBanAllResponse](#module_types..GroupBanAllResponse) : <code>object</code>
    * [~FileUpload](#module_types..FileUpload) : <code>object</code>
    * [~FileUploadResult](#module_types..FileUploadResult) : <code>object</code>
    * [~fileUploadProgress](#module_types..fileUploadProgress) : <code>function</code>
    * [~ConversationItem](#module_types..ConversationItem) : <code>object</code>
    * [~UserProfile](#module_types..UserProfile) : <code>object</code>
    * [~UserSettings](#module_types..UserSettings) : <code>object</code>
    * [~Event](#module_types..Event) : <code>string</code>
    * [~EventCallback](#module_types..EventCallback) : <code>function</code>

## "flooNotice" (res) {#event_flooNotice}
Floo通知

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> | 结果 |
| res.category | <code>string</code> | 类别 |
| res.desc | <code>string</code> | 描述 |

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
## "flooError" (res) {#event_flooError}
Floo错误

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> |  |
| res.category | <code>string</code> | 类别 |
| res.desc | <code>string</code> | 描述 |

**Example**  
```js
{category: 'USER_BANNED', desc:'用户被禁言'}
{category: 'USER_FROZEN', desc:'用户被冻结，请联系App管理员。'}
{category: 'APP_FROZEN', desc:'APP 被冻结，请登陆美信拓扑控制台查看详情。'}
{category: 'LICENSE', desc:'无效 LICENSE，请确认服务已按时付费。'}
{category: 'LICENSE', desc:'超出 LICENSE 用户数限制，请购买更高规格服务。'}
{category: 'DNS_FAILED', desc: dnsServer } // DNS错误: 无法访问
```
## "loginFail" (desc) {#event_loginFail}
登录失败

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| desc | <code>string</code> | 失败原因 |

## "loginSuccess" (res) {#event_loginSuccess}
登录成功

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> | 空对象 |

## "onGroupListUpdate" (meta) {#event_onGroupListUpdate}
群列表更新

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..Meta) \| <code>undefined</code> | 通知消息内容 |

## "onGroupMemberChanged" (groupId) {#event_onGroupMemberChanged}
群成员列表更新

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| groupId | <code>number</code> | 群ID |

## "onGroupMessage" (meta) {#event_onGroupMessage}
收到群消息

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..Meta) | 消息内容 |

## "onInputStatusMessage" (res) {#event_onInputStatusMessage}
对方正在输入

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> |  |
| res.ext | <code>string</code> | 扩展字段 |
| res.from | <code>string</code> | 发送者用户ID |
| res.to | <code>string</code> | 接收者用户ID |

## "onMentionMessage" (meta) {#event_onMentionMessage}
收到群组&#64;消息

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..Meta) | 消息内容 |

## "onMessageCanceled" (res) {#event_onMessageCanceled}
消息被取消已读

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> |  |
| res.uid | <code>string</code> | 会话ID |
| res.mid | <code>string</code> | 消息ID |

## "onMessageDeleted" (res) {#event_onMessageDeleted}
消息被删除

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> |  |
| res.uid | <code>string</code> | 会话ID |
| res.mid | <code>string</code> | 消息ID |

## "onMessageRecalled" (res) {#event_onMessageRecalled}
消息被撤回

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> |  |
| res.uid | <code>string</code> | 会话ID |
| res.mid | <code>string</code> | 消息ID |

## "onMessageStatusChanged" (res) {#event_onMessageStatusChanged}
消息状态变更：撤回/删除/已读

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> |  |
| res.uid | <code>string</code> | 会话ID |
| res.mid | <code>string</code> | 消息ID |

## "onReceiveHistoryMsg" (res) {#event_onReceiveHistoryMsg}
收到历史消息

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> |  |
| res.next | <code>number</code> | 下次取历史消息的key |

## "onRosterInfoUpdate" (res) {#event_onRosterInfoUpdate}
好友信息变更

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> |  |
| res.rosterIds | <code>Array.&lt;number&gt;</code> | 好友的用户ID列表 |

## "onRosterListUpdate" (meta) {#event_onRosterListUpdate}
好友列表变更

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..Meta) | 好友通知的消息内容 |

## "onRosterMessage" (meta) {#event_onRosterMessage}
收到单聊消息

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..Meta) | 消息内容 |

## "onSendingMessageStatusChanged" (res) {#event_onSendingMessageStatusChanged}
消息发送状态变更

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> |  |
| res.status: | <code>number</code> | 发送状态，取值为sending|failed|sent |
| res.mid: | <code>number</code> | 客户端生成的client_mid |

## "onUnreadChange" (cid) {#event_onUnreadChange}
未读数改变

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| cid | <code>number</code> | 会话ID |

## "recentlistUpdate" {#event_recentlistUpdate}
最近会话更新

**Kind**: event emitted by [<code>types</code>](#module_types)  
## "onGroupCreated" (meta) {#event_onGroupCreated}
群组创建通知

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..Meta) | 群通知的消息内容 |

## "onGroupDestoryed" (meta) {#event_onGroupDestoryed}
群组解散通知

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..Meta) | 群通知的消息内容 |

## "onGroupJoined" (meta) {#event_onGroupJoined}
成员入群通知

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..Meta) | 群通知的消息内容 |

## "onGroupApplyAccepted" (meta) {#event_onGroupApplyAccepted}
群申请被通过

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..Meta) | 群通知的消息内容 |

## "onGroupApplyDeclined" (meta) {#event_onGroupApplyDeclined}
群申请被拒绝

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..Meta) | 群通知的消息内容 |

## "onGroupBaned" (meta) {#event_onGroupBaned}
被群禁言

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..Meta) | 群通知的消息内容 |

## "onGroupUnbaned" (meta) {#event_onGroupUnbaned}
被群取消禁言

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..Meta) | 群通知的消息内容 |

## types~RosterItem : <code>object</code> {#module_types..RosterItem}
好友信息

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| alias | <code>string</code> | 别名 |
| auth_mode | <code>number</code> | 验证方式, 0 - 无需验证，任何人可以加为好友, 1 - 需要同意方可加为好友, 2 - 需要回答问题正确方可加为好友, 3 - 拒绝所有加好友申请,int32 |
| auth_question | <code>string</code> | 验证问题 |
| avatar | <code>string</code> | 头像 |
| description | <code>string</code> | 描述信息 |
| ext | <code>string</code> | 扩展信息 |
| mute_notification | <code>boolean</code> | 是否接收消息提醒 |
| nick_name | <code>string</code> | 昵称或名称 |
| public_info | <code>string</code> | 公开信息，好友和陌生人可见 |
| relation | <code>number</code> | 关系: 0 - 好友，1 - 被删除，2 - 陌生人, int32 |
| user_id | <code>number</code> | 好友用户ID,int64 |
| username | <code>string</code> | 用户名 |

## types~UserSettings : <code>object</code> {#module_types..UserSettings}
用户设置信息

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| auth_answer | <code>string</code> | 验证问题答案 |
| auth_mode | <code>number</code> | 验证方式, 0 - 无需验证，任何人可以加为好友, 1 - 需要同意方可加为好友, 2 - 需要回答问题正确方可加为好友, 3 - 拒绝所有加好友申请,int32 |
| auth_question | <code>string</code> | 验证问题 |
| auto_download | <code>boolean</code> | 是否自动下载 |
| group_confirm | <code>boolean</code> | 邀请入群时是否需要用户确认: true - 需要用户同意才可加入， false - 自动同意邀请 |
| id | <code>number</code> | 用户ID, int64 |
| no_push | <code>boolean</code> | 是否关闭推送消息 |
| no_push_detail | <code>boolean</code> | 是否推送详情 |
| no_push_end_hour | <code>number</code> | 推送免打扰结束时间,int32 |
| no_push_start_hour | <code>number</code> | 推送免打扰开始时间,int32 |
| no_sounds | <code>boolean</code> | 收到消息时是否静音 |
| push_nick_name | <code>string</code> | 推送昵称 |
| push_token | <code>string</code> | 推送token |
| silence_end_time | <code>number</code> | 推送不提醒结束时间,int32 |
| silence_start_time | <code>number</code> | 推送不提醒开始时间,int32 |
| user_id | <code>number</code> | 用户ID,int64 |
| vibratory | <code>boolean</code> | 收到消息时否振动 |

## types~UserProfile : <code>object</code> {#module_types..UserProfile}
用户信息

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| avatar | <code>string</code> | 头像 url |
| description | <code>string</code> | 描述信息 |
| email | <code>string</code> | 邮箱 |
| mobile | <code>string</code> | 手机号码 |
| nick_name | <code>string</code> | 昵称 |
| private_info | <code>string</code> | 私有信息，仅自己可见 |
| public_info | <code>string</code> | 公开信息，好友和陌生人可见 |
| user_id | <code>number</code> | 用户ID,int64 |
| username | <code>string</code> | 用户名 |

## types~Meta : <code>object</code> {#module_types..Meta}
消息体

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| id | <code>string</code> | 消息ID |
| from | <code>string</code> | 发送者 |
| to | <code>string</code> | 接收者 |
| content | <code>string</code> | 消息内容 |
| type | <code>string</code> | 消息类型： text - 文本, image - 图片， audio - 语音, video - 视频，file - 文件, location - 位置， command - 命令, forward - 转发 |
| ext | <code>string</code> \| <code>object</code> | 扩展字段 |
| config | <code>string</code> \| <code>object</code> | SDK扩展字段 |
| attach | <code>string</code> \| <code>object</code> | 附件信息 |
| status | <code>number</code> | 消息状态： 0 - 未读, 1 - 已投递, 2 - 已读 |
| timestamp | <code>string</code> | 消息发送时间戳（毫秒） |
| toType | <code>string</code> | 接收者类型： roster - 好友， group - 群组 |

## types~RosterApplication : <code>object</code> {#module_types..RosterApplication}
加好友申请列表项

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| expired_time | <code>number</code> | 过期时间,int64 |
| reason | <code>string</code> | 申请描述 |
| status | <code>number</code> | 状态： 0 - 等待确认， 1 - 接受， 2 - 拒绝。 int32 |
| user_id | <code>number</code> | 发起加好友申请的用户ID,int64 |

## types~GroupInfoAndSettings : <code>object</code> {#module_types..GroupInfoAndSettings}
群信息

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| apply_approval | <code>number</code> | 入群申请审批设置, 0:同意所有申请 1:需要管理员确认 2:拒绝所有申请 |
| avatar | <code>string</code> | 群头像 |
| ban_expire_time | <code>number</code> | 全员禁言过期时间（秒），禁言期间只允许管理员发消息， 为0或小于当前时间表示不禁言, -1表示永久禁言 |
| created_at | <code>number</code> | 创建时间 |
| description | <code>string</code> | 群描述 |
| ext | <code>string</code> | 群扩展信息 |
| group_id | <code>number</code> | 群id,int64 |
| history_visible | <code>boolean</code> | 新成员可见历史聊天记录设置 |
| member_invite | <code>boolean</code> | 群成员邀请设置: false - 不允许邀请, true - 允许邀请(默认) |
| member_modify | <code>boolean</code> | 群成员修改群信息设置:  false - 群成员不能修改群信息(默认), true - 群成员可以修改群信息 |
| msg_mute_mode | <code>number</code> | 群消息屏蔽模式: 0 - 表示不屏蔽, 1 - 表示屏蔽本地消息通知, 2 - 表示屏蔽消息，不接收消息 |
| msg_push_mode | <code>number</code> | 群消息推送模式：0 - 接收所有推送，1 - 不接受推送，2 - 接收管理员和@消息推送， 3 - 只接收管理员消息推送， 4 - 只接收&#64;消息推送 |
| name | <code>string</code> | 群名称 |
| owner_id | <code>number</code> | 群主id,int64 |
| read_ack | <code>boolean</code> | 群消息已读功能设置 |
| status | <code>number</code> | 群状态, 0：正常, 1：已解散 |
| type | <code>number</code> | 群类型: 1表示公开群，0表示私有群, 2表示聊天室 |
| updated_at | <code>number</code> | 更新时间,int64 |
| count | <code>number</code> | 群成员数 |
| capacity | <code>number</code> | 群容量 |

## types~BriefGroupInfoAndSettings : <code>object</code> {#module_types..BriefGroupInfoAndSettings}
群简要信息及用户设置

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| apply_approval | <code>number</code> | 入群申请审批设置, 0:同意所有申请 1:需要管理员确认 2:拒绝所有申请 |
| avatar | <code>string</code> | 群头像 |
| capacity | <code>number</code> | 群容量 |
| count | <code>number</code> | 群成员数 |
| group_id | <code>number</code> | 群id,int64 |
| msg_mute_mode | <code>number</code> | 群消息屏蔽模式: 0 - 表示不屏蔽, 1 - 表示屏蔽本地消息通知, 2 - 表示屏蔽消息，不接收消息 |
| msg_push_mode | <code>number</code> | 群消息推送模式：0 - 接收所有推送，1 - 不接受推送，2 - 接收管理员和@消息推送， 3 - 只接收管理员消息推送， 4 - 只接收&#64;消息推送 |
| name | <code>string</code> | 群名称 |
| owner | <code>number</code> | 群主id,int64 |
| status | <code>number</code> | 群状态, 0：正常, 1：已解散,int32 |
| type | <code>number</code> | 群类型: 1表示公开群，0表示私有群, 2表示聊天室。int32 |

## types~GroupMember : <code>object</code> {#module_types..GroupMember}
群成员格式

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| display_name | <code>string</code> | 成员群名片 |
| join_time | <code>number</code> | 成员入群时间,int64 |
| user_id | <code>number</code> | 用户id,int64 |
| avatar | <code>string</code> | 头像地址 |

## types~GroupMemberBanned : <code>object</code> {#module_types..GroupMemberBanned}
禁言成员

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| display_name | <code>string</code> | 成员群名片 |
| join_time | <code>number</code> | 成员入群时间,int64 |
| user_id | <code>number</code> | 用户id,int64 |
| avatar | <code>string</code> | 头像地址 |
| expired_time | <code>number</code> | 禁言过期时间 |

## types~GroupUserRelationResponse : <code>object</code> {#module_types..GroupUserRelationResponse}
群用户请求结果

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| reason | <code>string</code> | 原因 |
| result | <code>string</code> | 结果 |
| user_id | <code>number</code> | 用户ID，int64 |

## types~GroupAnnouncement : <code>object</code> {#module_types..GroupAnnouncement}
群公告内容

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| author | <code>number</code> | 公告发布者,int64 |
| content | <code>string</code> | 公告内容 |
| created_at | <code>number</code> | 公告发布时间,int64 |
| group_id | <code>number</code> | 群id,int64 |
| id | <code>number</code> | 公告id,int64 |
| title | <code>string</code> | 公告标题 |

## types~GroupInfoRequest : <code>object</code> {#module_types..GroupInfoRequest}
创建群

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| avatar | <code>string</code> | 群头像 |
| description | <code>string</code> | 群描述 |
| name | <code>string</code> | 群名称 |
| type | <code>number</code> | 群类型 1表示公开群，0表示私有群, 2表示聊天室,int32 |
| user_list | <code>Array.&lt;number&gt;</code> | 邀请入群的用户id列表 |

## types~GroupBannedMemberRequest : <code>object</code> {#module_types..GroupBannedMemberRequest}
禁言请求

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| duration | <code>number</code> | 禁言时长，单位为分钟,int64 |
| group_id | <code>number</code> | 群id,int64 |
| user_list | <code>Array.&lt;number&gt;</code> | 用户id列表 |

## types~GroupBlockedListItem : <code>object</code> {#module_types..GroupBlockedListItem}
群组黑名单

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| user_id | <code>number</code> | 用户id,int64 |
| group_id | <code>number</code> | 群id,int64 |
| create_at | <code>string</code> | 创建时间 |

## types~GroupInvitation : <code>object</code> {#module_types..GroupInvitation}
群组邀请信息

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| group_id | <code>number</code> | 群ID |
| inviter_id | <code>number</code> | 邀请者ID |
| invitee_id | <code>number</code> | 被邀请者ID |
| reason | <code>string</code> | 原因 |
| status | <code>number</code> | 状态： 0 - 待处理，1 - 用户同意，2 - 用户拒绝 |
| expire_time | <code>number</code> | 过期时间 |
| create_at | <code>string</code> | 创建时间 |

## types~GroupApplication : <code>object</code> {#module_types..GroupApplication}
群申请信息

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| group_id | <code>number</code> | 群ID |
| applicant_id | <code>number</code> | 申请者ID |
| reason | <code>string</code> | 原因 |
| expire_time | <code>number</code> | 过期时间 |
| status | <code>number</code> | 状态： 0 - 待处理，1 - 同意，2 - 拒绝 |

## types~GroupSharedFile : <code>object</code> {#module_types..GroupSharedFile}
群共享文件返回格式

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| created_at | <code>number</code> | int64 |
| file_id | <code>number</code> | 共享文件id,int64 |
| group_id | <code>number</code> | 群id,int64 |
| name | <code>string</code> | 共享文件名称 |
| size | <code>number</code> | 共享文件大小,int64 |
| type | <code>string</code> | 共享文件类型 |
| updated_at | <code>number</code> | int64 |
| uploader | <code>number</code> | 共享文件上传者,int64 |
| url | <code>string</code> | 共享文件url |

## types~GroupSharedFileResponse : <code>object</code> {#module_types..GroupSharedFileResponse}
删除群共享文件结果

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| file_id | <code>number</code> | 文件ID |
| reason | <code>string</code> | 原因 |
| result | <code>string</code> | 结果 |

## types~GroupBanAllResponse : <code>object</code> {#module_types..GroupBanAllResponse}
全员禁言结果

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| ban_expire_time | <code>number</code> | 全员禁言过期时间,int64 |

## types~FileUpload : <code>object</code> {#module_types..FileUpload}
文件上传信息

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| download_url | <code>string</code> | 下载地址 |
| oss_body_param | <code>object.&lt;string, string&gt;</code> | 额外参数 |
| upload_url | <code>string</code> | 上传地址 |

## types~FileUploadResult : <code>object</code> {#module_types..FileUploadResult}
文件上传结果

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| url | <code>string</code> | 下载地址 |

## types~fileUploadProgress : <code>function</code> {#module_types..fileUploadProgress}
文件上传进度回调

**Kind**: inner typedef of [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> | 进度 |
| res.loaded | <code>number</code> | 已下载字节数 |
| res.total | <code>number</code> | 总字节数 |

## types~ConversationItem : <code>object</code> {#module_types..ConversationItem}
会话信息

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| id | <code>number</code> | 会话ID |
| content | <code>string</code> | 消息内容 |
| timestamp | <code>string</code> | 消息发送时间戳（毫秒） |
| type | <code>string</code> | 会话类型： roster - 单聊， group - 群聊 |

## types~UserProfile : <code>object</code> {#module_types..UserProfile}
用户信息

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| avatar | <code>string</code> | 头像 url |
| description | <code>string</code> | 描述信息 |
| email | <code>string</code> | 邮箱 |
| mobile | <code>string</code> | 手机号码 |
| nick_name | <code>string</code> | 昵称 |
| private_info | <code>string</code> | 私有信息，仅自己可见 |
| public_info | <code>string</code> | 公开信息，好友和陌生人可见 |
| user_id | <code>number</code> | 用户ID,int64 |
| username | <code>string</code> | 用户名 |

## types~UserSettings : <code>object</code> {#module_types..UserSettings}
用户设置信息

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| auth_answer | <code>string</code> | 验证问题答案 |
| auth_mode | <code>number</code> | 验证方式, 0 - 无需验证，任何人可以加为好友, 1 - 需要同意方可加为好友, 2 - 需要回答问题正确方可加为好友, 3 - 拒绝所有加好友申请,int32 |
| auth_question | <code>string</code> | 验证问题 |
| auto_download | <code>boolean</code> | 是否自动下载 |
| group_confirm | <code>boolean</code> | 邀请入群时是否需要用户确认: true - 需要用户同意才可加入， false - 自动同意邀请 |
| id | <code>number</code> | 设置ID |
| no_push | <code>boolean</code> | 是否关闭推送消息 |
| no_push_detail | <code>boolean</code> | 是否推送详情 |
| no_push_end_hour | <code>number</code> | 推送免打扰结束时间,int32 |
| no_push_start_hour | <code>number</code> | 推送免打扰开始时间,int32 |
| no_sounds | <code>boolean</code> | 收到消息时是否静音 |
| push_nick_name | <code>string</code> | 推送昵称 |
| push_token | <code>string</code> | 推送token |
| silence_end_time | <code>number</code> | 推送不提醒结束时间,int32 |
| silence_start_time | <code>number</code> | 推送不提醒开始时间,int32 |
| user_id | <code>number</code> | 用户ID,int64 |
| vibratory | <code>boolean</code> | 收到消息时否振动 |

## types~Event : <code>string</code> {#module_types..Event}
监听事件名称

**Kind**: inner typedef of [<code>types</code>](#module_types)  
## types~EventCallback : <code>function</code> {#module_types..EventCallback}
监听事件回调

**Kind**: inner typedef of [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | [<code>flooNotice</code>](#event_flooNotice) \| [<code>flooError</code>](#event_flooError) \| [<code>loginFail</code>](#event_loginFail) \| [<code>loginSuccess</code>](#event_loginSuccess) \| [<code>onGroupListUpdate</code>](#event_onGroupListUpdate) \| [<code>onGroupMemberChanged</code>](#event_onGroupMemberChanged) \| [<code>onGroupMessage</code>](#event_onGroupMessage) \| [<code>onInputStatusMessage</code>](#event_onInputStatusMessage) \| [<code>onMentionMessage</code>](#event_onMentionMessage) \| [<code>onMessageCanceled</code>](#event_onMessageCanceled) \| [<code>onMessageDeleted</code>](#event_onMessageDeleted) \| [<code>onMessageRecalled</code>](#event_onMessageRecalled) \| [<code>onMessageStatusChanged</code>](#event_onMessageStatusChanged) \| [<code>onReceiveHistoryMsg</code>](#event_onReceiveHistoryMsg) \| [<code>onRosterInfoUpdate</code>](#event_onRosterInfoUpdate) \| [<code>onRosterListUpdate</code>](#event_onRosterListUpdate) \| [<code>onRosterMessage</code>](#event_onRosterMessage) \| [<code>onSendingMessageStatusChanged</code>](#event_onSendingMessageStatusChanged) \| [<code>onUnreadChange</code>](#event_onUnreadChange) \| [<code>recentlistUpdate</code>](#event_recentlistUpdate) \| [<code>onGroupCreated</code>](#event_onGroupCreated) \| [<code>onGroupDestoryed</code>](#event_onGroupDestoryed) \| [<code>onGroupJoined</code>](#event_onGroupJoined) \| [<code>onGroupApplyAccepted</code>](#event_onGroupApplyAccepted) \| [<code>onGroupApplyDeclined</code>](#event_onGroupApplyDeclined) \| [<code>onGroupBaned</code>](#event_onGroupBaned) \| [<code>onGroupUnbaned</code>](#event_onGroupUnbaned) | 事件结果 |

# flooim {#module_flooim}

* [flooim](#module_flooim)
    * [.flooim(config)](#module_flooim.flooim) ⇒ <code>object</code>
    * [.login(opt)](#module_flooim.login)
    * [.qrlogin(opt)](#module_flooim.qrlogin)
    * [.tokenLogin(opt)](#module_flooim.tokenLogin)
    * [.idLogin(opt)](#module_flooim.idLogin)
    * [.isLogin()](#module_flooim.isLogin) ⇒ <code>boolean</code>
    * [.on(options, ext)](#module_flooim.on)
    * [.off(options, ext)](#module_flooim.off)
    * [.logout()](#module_flooim.logout)

## flooim.flooim(config) ⇒ <code>object</code> {#module_flooim.flooim}
初始化SDK

**Kind**: static method of [<code>flooim</code>](#module_flooim)  
**Returns**: <code>object</code> - flooim对象  

| Param | Type | Description |
| --- | --- | --- |
| config | <code>object</code> | SDK初始化设置 |
| config.appid | <code>string</code> | APPID |
| config.ws | <code>boolean</code> | 连接地址前缀是否为ws/wss: true - 连接地址前缀为ws或wss, false - 连接地址前缀为http/https |
| config.autoLogin | <code>boolean</code> | 是否自动登录 |
| config.dnsServer | <code>string</code> \| <code>undefined</code> | DNS服务器地址， 可以不设置，默认为 https://dns.maximtop.com/v2/app_dns |

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
## flooim.login(opt) {#module_flooim.login}
登录

**Kind**: static method of [<code>flooim</code>](#module_flooim)  

| Param | Type | Description |
| --- | --- | --- |
| opt | <code>object</code> |  |
| opt.name | <code>string</code> | 用户名 |
| opt.password | <code>string</code> | 密码 |

## flooim.qrlogin(opt) {#module_flooim.qrlogin}
二维码登录

**Kind**: static method of [<code>flooim</code>](#module_flooim)  

| Param | Type | Description |
| --- | --- | --- |
| opt | <code>object</code> |  |
| opt.user_id | <code>number</code> | 用户ID |
| opt.password | <code>string</code> | 密码 |

## flooim.tokenLogin(opt) {#module_flooim.tokenLogin}
token登录

**Kind**: static method of [<code>flooim</code>](#module_flooim)  

| Param | Type | Description |
| --- | --- | --- |
| opt | <code>object</code> |  |
| opt.user_id | <code>number</code> | 用户ID |
| opt.token | <code>string</code> | Token |

## flooim.idLogin(opt) {#module_flooim.idLogin}
使用用户ID和密码登录

**Kind**: static method of [<code>flooim</code>](#module_flooim)  

| Param | Type | Description |
| --- | --- | --- |
| opt | <code>object</code> |  |
| opt.user_id | <code>number</code> | 用户ID |
| opt.password | <code>string</code> | 密码 |

## flooim.isLogin() ⇒ <code>boolean</code> {#module_flooim.isLogin}
是否已登录

**Kind**: static method of [<code>flooim</code>](#module_flooim)  
**Returns**: <code>boolean</code> - 是否已登录  
## flooim.on(options, ext) {#module_flooim.on}
事件监听

**Kind**: static method of [<code>flooim</code>](#module_flooim)  

| Param | Type | Description |
| --- | --- | --- |
| options | [<code>Event</code>](#module_types..Event) \| <code>Object.&lt;module:types~Event, module:types~EventCallback&gt;</code> | 可以为事件名，也可以为事件名和事件回调 |
| ext | [<code>EventCallback</code>](#module_types..EventCallback) \| <code>undefined</code> | 事件回调，只有options为事件名时需要设置 |

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
## flooim.off(options, ext) {#module_flooim.off}
取消监听

**Kind**: static method of [<code>flooim</code>](#module_flooim)  

| Param | Type | Description |
| --- | --- | --- |
| options | [<code>Event</code>](#module_types..Event) \| <code>Object.&lt;module:types~Event, module:types~EventCallback&gt;</code> | 可以为事件名，也可以为事件名和事件回调 |
| ext | [<code>EventCallback</code>](#module_types..EventCallback) \| <code>undefined</code> | 事件回调，只有options为事件名时需要设置 |

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
## flooim.logout() {#module_flooim.logout}
退出账户

**Kind**: static method of [<code>flooim</code>](#module_flooim)  
