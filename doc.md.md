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

# groupManage {#module_groupmanage}
群管理


* [groupManage](#module_groupmanage)
    * [.asyncGetGroupInfo(group_id, froce)](#module_groupmanage.asyncgetgroupinfo) ⇒ [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..groupinfoandsettings)
    * [.asyncGetJoinedGroups(froce)](#module_groupmanage.asyncgetjoinedgroups) ⇒ <code>Promise.&lt;Array.&lt;number&gt;&gt;</code>
    * [.openGroup(group_id)](#module_groupmanage.opengroup)
    * [.getAllGroupDetail()](#module_groupmanage.getallgroupdetail) ⇒ <code>Object.&lt;number, module:types~GroupInfoAndSettings&gt;</code>
    * [.asyncGetGroupMembers(group_id)](#module_groupmanage.asyncgetgroupmembers) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code>
    * [.getGroupMembers(group_id)](#module_groupmanage.getgroupmembers) ⇒ [<code>Array.&lt;GroupMember&gt;</code>](#module_types..groupmember)
    * [.asyncGetGroupListDetail(gids)](#module_groupmanage.asyncgetgrouplistdetail) ⇒ <code>Promise.&lt;Array.&lt;module:types~BriefGroupInfoAndSettings&gt;&gt;</code>
    * [.getGruopMessage(gid)](#module_groupmanage.getgruopmessage) ⇒ [<code>Array.&lt;Meta&gt;</code>](#module_types..meta)
    * [.asyncGetInfo(params)](#module_groupmanage.asyncgetinfo) ⇒ [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..groupinfoandsettings)
    * [.asyncGetMemberList(param)](#module_groupmanage.asyncgetmemberlist) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code>
    * [.readGroupMessage(group_id, mid)](#module_groupmanage.readgroupmessage)
    * [.recallMessage(uid, mid)](#module_groupmanage.recallmessage)
    * [.getUnreadCount(gid)](#module_groupmanage.getunreadcount) ⇒ <code>number</code>
    * [.asyncGetAdminList(params)](#module_groupmanage.asyncgetadminlist) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code>
    * [.asyncAdminAdd(params)](#module_groupmanage.asyncadminadd) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code>
    * [.asyncAdminRemove(params)](#module_groupmanage.asyncadminremove) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code>
    * [.asyncGetAnouncementById(params)](#module_groupmanage.asyncgetanouncementbyid) ⇒ [<code>Promise.&lt;GroupAnnouncement&gt;</code>](#module_types..groupannouncement)
    * [.asyncAnouncementDelete(params)](#module_groupmanage.asyncanouncementdelete) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncAnnouncementEdit(params)](#module_groupmanage.asyncannouncementedit) ⇒ [<code>Promise.&lt;GroupAnnouncement&gt;</code>](#module_types..groupannouncement)
    * [.asyncGetAnnouncementList(params)](#module_groupmanage.asyncgetannouncementlist) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupAnnouncement&gt;&gt;</code>
    * [.asyncCreate(params)](#module_groupmanage.asynccreate) ⇒ [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..groupinfoandsettings)
    * [.asyncDestroy(params)](#module_groupmanage.asyncdestroy) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateAvatar(params)](#module_groupmanage.asyncupdateavatar) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateDescription(params)](#module_groupmanage.asyncupdatedescription) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateExt(params)](#module_groupmanage.asyncupdateext) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateName(params)](#module_groupmanage.asyncupdatename) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncGroupMsgMutemode(params)](#module_groupmanage.asyncgroupmsgmutemode) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncGroupBannedList(params)](#module_groupmanage.asyncgroupbannedlist) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMemberBanned&gt;&gt;</code>
    * [.asyncGroupBab(params)](#module_groupmanage.asyncgroupbab) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code>
    * [.asyncGroupUnban(params)](#module_groupmanage.asyncgroupunban) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code>
    * [.asyncGetSettings(group_id)](#module_groupmanage.asyncgetsettings) ⇒ [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..groupinfoandsettings)
    * [.asyncUpdateAllowMemberInvitation(params)](#module_groupmanage.asyncupdateallowmemberinvitation) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateAllowMemberModify(params)](#module_groupmanage.asyncupdateallowmembermodify) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateEnableReadack(params)](#module_groupmanage.asyncupdateenablereadack) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateHistoryVisible(params)](#module_groupmanage.asyncupdatehistoryvisible) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateRequireadminapproval(params)](#module_groupmanage.asyncupdaterequireadminapproval) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncBanAll(params)](#module_groupmanage.asyncbanall) ⇒ [<code>Promise.&lt;GroupBanAllResponse&gt;</code>](#module_types..groupbanallresponse)
    * [.asyncUnBanAll(params)](#module_groupmanage.asyncunbanall) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncOwnerTransfer(params)](#module_groupmanage.asyncownertransfer) ⇒ [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..groupuserrelationresponse)
    * [.asyncGetUserJoined(params)](#module_groupmanage.asyncgetuserjoined) ⇒ <code>Promise.&lt;Array.&lt;number&gt;&gt;</code>
    * [.asyncApply(params)](#module_groupmanage.asyncapply) ⇒ [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..groupuserrelationresponse)
    * [.asyncApplyHandle(params)](#module_groupmanage.asyncapplyhandle) ⇒ [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..groupuserrelationresponse)
    * [.asyncGroupBockedlist(params)](#module_groupmanage.asyncgroupbockedlist) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupBlockedListItem&gt;&gt;</code>
    * [.asyncGroupBlock(params)](#module_groupmanage.asyncgroupblock) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code>
    * [.asyncGroupUnblock(params)](#module_groupmanage.asyncgroupunblock) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code>
    * [.asyncKick(params)](#module_groupmanage.asynckick) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code>
    * [.asyncGetInvitationList()](#module_groupmanage.asyncgetinvitationlist) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupInvitation&gt;&gt;</code>
    * [.asyncInvite(params)](#module_groupmanage.asyncinvite) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code>
    * [.asyncInviteHandle(params)](#module_groupmanage.asyncinvitehandle) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncGetMemberDisplayName(params)](#module_groupmanage.asyncgetmemberdisplayname) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code>
    * [.asyncLeave(params)](#module_groupmanage.asyncleave) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateDisplayName(params)](#module_groupmanage.asyncupdatedisplayname) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asncGetApplicationList(params)](#module_groupmanage.asncgetapplicationlist) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupApplication&gt;&gt;</code>
    * [.asyncGetFileList(params)](#module_groupmanage.asyncgetfilelist) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupSharedFile&gt;&gt;</code>
    * [.asyncFileDelete(params)](#module_groupmanage.asyncfiledelete) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupSharedFileResponse&gt;&gt;</code>
    * [.asyncFileUpload(params)](#module_groupmanage.asyncfileupload) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupSharedFile&gt;&gt;</code>

## groupManage.asyncGetGroupInfo(group_id, froce) ⇒ [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..groupinfoandsettings) {#module_groupmanage.asyncgetgroupinfo}
获取群信息

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..groupinfoandsettings) - 群信息  

| Param | Type | Description |
| --- | --- | --- |
| group_id | <code>number</code> | 群ID |
| froce | <code>boolean</code> | 是否强制从服务器拉取： true - 从服务器拉取， false - 优先从本地存储获取 |

## groupManage.asyncGetJoinedGroups(froce) ⇒ <code>Promise.&lt;Array.&lt;number&gt;&gt;</code> {#module_groupmanage.asyncgetjoinedgroups}
获取加入的群组

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;number&gt;&gt;</code> - 群组ID列表  

| Param | Type | Description |
| --- | --- | --- |
| froce | <code>boolean</code> | 是否强制从服务器拉取： true - 从服务器拉取， false - 优先从本地存储获取 |

## groupManage.openGroup(group_id) {#module_groupmanage.opengroup}
打开群组， 此方法会准备群组聊天界面的一些必备信息。

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  

| Param | Type | Description |
| --- | --- | --- |
| group_id | <code>number</code> | 群组ID |

## groupManage.getAllGroupDetail() ⇒ <code>Object.&lt;number, module:types~GroupInfoAndSettings&gt;</code> {#module_groupmanage.getallgroupdetail}
获取缓存的所有群组详情

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Object.&lt;number, module:types~GroupInfoAndSettings&gt;</code> - 群组详情  
## groupManage.asyncGetGroupMembers(group_id) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code> {#module_groupmanage.asyncgetgroupmembers}
获取群组成员（异步）

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code> - 群成员列表  

| Param | Type | Description |
| --- | --- | --- |
| group_id | <code>number</code> | 群组ID |

## groupManage.getGroupMembers(group_id) ⇒ [<code>Array.&lt;GroupMember&gt;</code>](#module_types..groupmember) {#module_groupmanage.getgroupmembers}
获取群组成员（同步）

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: [<code>Array.&lt;GroupMember&gt;</code>](#module_types..groupmember) - 群成员列表  

| Param | Type | Description |
| --- | --- | --- |
| group_id | <code>number</code> | 群组ID |

## groupManage.asyncGetGroupListDetail(gids) ⇒ <code>Promise.&lt;Array.&lt;module:types~BriefGroupInfoAndSettings&gt;&gt;</code> {#module_groupmanage.asyncgetgrouplistdetail}
按id获取群组详情

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~BriefGroupInfoAndSettings&gt;&gt;</code> - 群组详情列表  

| Param | Type | Description |
| --- | --- | --- |
| gids | <code>Array.&lt;number&gt;</code> | 群组ID列表 |

## groupManage.getGruopMessage(gid) ⇒ [<code>Array.&lt;Meta&gt;</code>](#module_types..meta) {#module_groupmanage.getgruopmessage}
获取群消息

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: [<code>Array.&lt;Meta&gt;</code>](#module_types..meta) - 群消息列表  

| Param | Type | Description |
| --- | --- | --- |
| gid | <code>number</code> | 群ID |

## groupManage.asyncGetInfo(params) ⇒ [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..groupinfoandsettings) {#module_groupmanage.asyncgetinfo}
获取群组详情

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..groupinfoandsettings) - 群组详情  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.asyncGetMemberList(param) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code> {#module_groupmanage.asyncgetmemberlist}
获取群成员列表

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code> - 群成员列表  

| Param | Type | Description |
| --- | --- | --- |
| param | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.readGroupMessage(group_id, mid) {#module_groupmanage.readgroupmessage}
将群消息设置已读

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  

| Param | Type | Description |
| --- | --- | --- |
| group_id | <code>number</code> | 群组ID |
| mid | <code>number</code> | 消息ID |

## groupManage.recallMessage(uid, mid) {#module_groupmanage.recallmessage}
撤回消息

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  

| Param | Type | Description |
| --- | --- | --- |
| uid | <code>number</code> | 群组ID |
| mid | <code>number</code> | 消息ID |

## groupManage.getUnreadCount(gid) ⇒ <code>number</code> {#module_groupmanage.getunreadcount}
获取群未读消息数

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>number</code> - 未读消息数  

| Param | Type | Description |
| --- | --- | --- |
| gid | <code>number</code> | 群组ID |

## groupManage.asyncGetAdminList(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code> {#module_groupmanage.asyncgetadminlist}
获取群管理员列表

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code> - 群管理员列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.asyncAdminAdd(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> {#module_groupmanage.asyncadminadd}
群添加管理员

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> - 结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_list | <code>Array.&lt;number&gt;</code> | 群成员列表 |

## groupManage.asyncAdminRemove(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> {#module_groupmanage.asyncadminremove}
移除管理员

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> - 结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_list | <code>Array.&lt;number&gt;</code> | 群成员列表 |

## groupManage.asyncGetAnouncementById(params) ⇒ [<code>Promise.&lt;GroupAnnouncement&gt;</code>](#module_types..groupannouncement) {#module_groupmanage.asyncgetanouncementbyid}
获取群公告详情

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: [<code>Promise.&lt;GroupAnnouncement&gt;</code>](#module_types..groupannouncement) - 群公告详情  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.announcement_id | <code>Array.&lt;number&gt;</code> | 公告ID |

## groupManage.asyncAnouncementDelete(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupmanage.asyncanouncementdelete}
删除群公告

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.announcement_id | <code>Array.&lt;number&gt;</code> | 公告ID |

## groupManage.asyncAnnouncementEdit(params) ⇒ [<code>Promise.&lt;GroupAnnouncement&gt;</code>](#module_types..groupannouncement) {#module_groupmanage.asyncannouncementedit}
编辑群公告

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: [<code>Promise.&lt;GroupAnnouncement&gt;</code>](#module_types..groupannouncement) - 群公告详情  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.title | <code>string</code> | 公告标题 |
| params.content | <code>string</code> | 公告内容 |

## groupManage.asyncGetAnnouncementList(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupAnnouncement&gt;&gt;</code> {#module_groupmanage.asyncgetannouncementlist}
群公告列表

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupAnnouncement&gt;&gt;</code> - 群公告详情列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.asyncCreate(params) ⇒ [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..groupinfoandsettings) {#module_groupmanage.asynccreate}
创建群组

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..groupinfoandsettings) - 群详情  

| Param | Type | Description |
| --- | --- | --- |
| params | [<code>GroupInfoRequest</code>](#module_types..groupinforequest) | 请求参数 |

## groupManage.asyncDestroy(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupmanage.asyncdestroy}
解散群组

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.asyncUpdateAvatar(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupmanage.asyncupdateavatar}
更新群头像

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>string</code> | 头像地址 |

## groupManage.asyncUpdateDescription(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupmanage.asyncupdatedescription}
更新群描述

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>string</code> | 群组描述 |

## groupManage.asyncUpdateExt(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupmanage.asyncupdateext}
更新群扩展信息

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>string</code> | 扩展信息 |

## groupManage.asyncUpdateName(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupmanage.asyncupdatename}
更新群名称

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>string</code> | 群名称 |

## groupManage.asyncGroupMsgMutemode(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupmanage.asyncgroupmsgmutemode}
设置群消息免打扰情况

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.msg_mute_mode | <code>number</code> | 群消息屏蔽模式: 0 - 表示不屏蔽, 1 - 表示屏蔽本地消息通知, 2 - 表示屏蔽消息，不接收消息 |

## groupManage.asyncGroupBannedList(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMemberBanned&gt;&gt;</code> {#module_groupmanage.asyncgroupbannedlist}
获取群禁言列表

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupMemberBanned&gt;&gt;</code> - 禁言成员列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.asyncGroupBab(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> {#module_groupmanage.asyncgroupbab}
禁言群成员

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> - 请求结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | [<code>GroupBannedMemberRequest</code>](#module_types..groupbannedmemberrequest) | 请求参数 |

## groupManage.asyncGroupUnban(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> {#module_groupmanage.asyncgroupunban}
解除成员禁言

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> - 请求结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_list | <code>Array.&lt;number&gt;</code> | 群成员列表 |

## groupManage.asyncGetSettings(group_id) ⇒ [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..groupinfoandsettings) {#module_groupmanage.asyncgetsettings}
获取群设置

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: [<code>Promise.&lt;GroupInfoAndSettings&gt;</code>](#module_types..groupinfoandsettings) - 群设置  

| Param | Type | Description |
| --- | --- | --- |
| group_id | <code>number</code> | 群ID |

## groupManage.asyncUpdateAllowMemberInvitation(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupmanage.asyncupdateallowmemberinvitation}
设置群成员是否可以邀请

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>boolean</code> | 群成员邀请设置: false - 不允许邀请, true - 允许邀请(默认) |

## groupManage.asyncUpdateAllowMemberModify(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupmanage.asyncupdateallowmembermodify}
设置群成员是否可以修改群信息

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>boolean</code> | 群成员修改群信息设置:  false - 群成员不能修改群信息(默认), true - 群成员可以修改群信息 |

## groupManage.asyncUpdateEnableReadack(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupmanage.asyncupdateenablereadack}
设置群是否开启已读模式

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>boolean</code> | 是否开启群消息已读功能:  false - 不开启, true - 开启 |

## groupManage.asyncUpdateHistoryVisible(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupmanage.asyncupdatehistoryvisible}
设置群历史是否可见

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>boolean</code> | 设置群历史是否可见:  false - 不可见, true - 可见 |

## groupManage.asyncUpdateRequireadminapproval(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupmanage.asyncupdaterequireadminapproval}
设置入群是否需要申请

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.apply_approval | <code>boolean</code> | 入群申请审批设置, 0:同意所有申请 1:需要管理员确认 2:拒绝所有申请 |

## groupManage.asyncBanAll(params) ⇒ [<code>Promise.&lt;GroupBanAllResponse&gt;</code>](#module_types..groupbanallresponse) {#module_groupmanage.asyncbanall}
全员禁言，只允许管理员发消息

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: [<code>Promise.&lt;GroupBanAllResponse&gt;</code>](#module_types..groupbanallresponse) - 结果  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.duration | <code>number</code> | 禁言时长，单位为分钟,int64 |
| params.group_id | <code>number</code> | 群id,int64 |

## groupManage.asyncUnBanAll(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupmanage.asyncunbanall}
取消全员禁言

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群id,int64 |

## groupManage.asyncOwnerTransfer(params) ⇒ [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..groupuserrelationresponse) {#module_groupmanage.asyncownertransfer}
更换群主

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..groupuserrelationresponse) - 结果  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.new_owner | <code>number</code> | 新群主的用户ID |

## groupManage.asyncGetUserJoined(params) ⇒ <code>Promise.&lt;Array.&lt;number&gt;&gt;</code> {#module_groupmanage.asyncgetuserjoined}
获取用户的群组列表

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;number&gt;&gt;</code> - 群ID的列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数, 空对象 |

## groupManage.asyncApply(params) ⇒ [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..groupuserrelationresponse) {#module_groupmanage.asyncapply}
申请加入群

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..groupuserrelationresponse) - 结果  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.reason | <code>string</code> | 申请入群原因 |

## groupManage.asyncApplyHandle(params) ⇒ [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..groupuserrelationresponse) {#module_groupmanage.asyncapplyhandle}
处理用户的入群申请

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: [<code>Promise.&lt;GroupUserRelationResponse&gt;</code>](#module_types..groupuserrelationresponse) - 结果  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_id | <code>number</code> | 用户ID |
| params.approval | <code>boolean</code> | 审批结果：true为同意，false为拒绝 |

## groupManage.asyncGroupBockedlist(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupBlockedListItem&gt;&gt;</code> {#module_groupmanage.asyncgroupbockedlist}
获取群黑名单

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupBlockedListItem&gt;&gt;</code> - 群黑名单列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.asyncGroupBlock(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> {#module_groupmanage.asyncgroupblock}
将成员加入黑名单

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> - 结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_list | <code>Array.&lt;number&gt;</code> | 群成员列表 |

## groupManage.asyncGroupUnblock(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> {#module_groupmanage.asyncgroupunblock}
解除黑名单

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> - 结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_list | <code>Array.&lt;number&gt;</code> | 群成员列表 |

## groupManage.asyncKick(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> {#module_groupmanage.asynckick}
踢出群组

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> - 结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_list | <code>Array.&lt;number&gt;</code> | 群成员列表 |

## groupManage.asyncGetInvitationList() ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupInvitation&gt;&gt;</code> {#module_groupmanage.asyncgetinvitationlist}
获取群邀请列表

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupInvitation&gt;&gt;</code> - 群邀请列表  
## groupManage.asyncInvite(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> {#module_groupmanage.asyncinvite}
邀请成员加入群

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupUserRelationResponse&gt;&gt;</code> - 结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_list | <code>Array.&lt;number&gt;</code> | 群成员列表 |

## groupManage.asyncInviteHandle(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupmanage.asyncinvitehandle}
处理群邀请

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_id | <code>number</code> | 用户ID |
| params.approval | <code>boolean</code> | 审批结果：true为同意，false为拒绝 |

## groupManage.asyncGetMemberDisplayName(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code> {#module_groupmanage.asyncgetmemberdisplayname}
批量获取群成员的群名片

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupMember&gt;&gt;</code> - 群成员列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.user_list | <code>Array.&lt;number&gt;</code> | 群成员列表 |

## groupManage.asyncLeave(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupmanage.asyncleave}
退出群

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.asyncUpdateDisplayName(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_groupmanage.asyncupdatedisplayname}
修改群名片

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.value | <code>string</code> | 新名片 |

## groupManage.asncGetApplicationList(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupApplication&gt;&gt;</code> {#module_groupmanage.asncgetapplicationlist}
获取群申请列表

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupApplication&gt;&gt;</code> - 群申请列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_list | <code>Array.&lt;number&gt;</code> | 群列表 |

## groupManage.asyncGetFileList(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupSharedFile&gt;&gt;</code> {#module_groupmanage.asyncgetfilelist}
获取群文件列表

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupSharedFile&gt;&gt;</code> - 群文件列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## groupManage.asyncFileDelete(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupSharedFileResponse&gt;&gt;</code> {#module_groupmanage.asyncfiledelete}
删除群文件

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupSharedFileResponse&gt;&gt;</code> - 结果列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |
| params.file_list | <code>Array.&lt;number&gt;</code> | 文件ID列表 |

## groupManage.asyncFileUpload(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~GroupSharedFile&gt;&gt;</code> {#module_groupmanage.asyncfileupload}
上传群文件

**Kind**: static method of [<code>groupManage</code>](#module_groupmanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~GroupSharedFile&gt;&gt;</code> - 群文件列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群id,int64 |
| params.name | <code>string</code> | 文件名称 |
| params.size | <code>number</code> | 文件大小,int64 |
| params.type | <code>string</code> | 文件类型 |
| params.url | <code>string</code> | 文件url |

# rosterManage {#module_rostermanage}
好友管理


* [rosterManage](#module_rostermanage)
    * [.asyncGetRosterIdList(force)](#module_rostermanage.asyncgetrosteridlist) ⇒ <code>Promise.&lt;Array.&lt;number&gt;&gt;</code>
    * [.asyncGetRosterInfo(roster_id, force)](#module_rostermanage.asyncgetrosterinfo) ⇒ [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..rosteritem)
    * [.asyncRegester(opt)](#module_rostermanage.asyncregester) ⇒ [<code>Promise.&lt;UserSettings&gt;</code>](#module_types..usersettings)
    * [.asyncDeleteRoster(param)](#module_rostermanage.asyncdeleteroster) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asnycGetRosterListDetailByIds(roster_ids)](#module_rostermanage.asnycgetrosterlistdetailbyids) ⇒ <code>Promise.&lt;Array.&lt;module:types~RosterItem&gt;&gt;</code>
    * [.getAllRosterDetail()](#module_rostermanage.getallrosterdetail) ⇒ [<code>Array.&lt;RosterItem&gt;</code>](#module_types..rosteritem)
    * [.asyncGetUserProfile(force)](#module_rostermanage.asyncgetuserprofile) ⇒ [<code>Promise.&lt;UserProfile&gt;</code>](#module_types..userprofile)
    * [.getRosterMessageByRid(uid)](#module_rostermanage.getrostermessagebyrid) ⇒ [<code>Array.&lt;Meta&gt;</code>](#module_types..meta)
    * [.readRosterMessage(roster_id, mid)](#module_rostermanage.readrostermessage)
    * [.recallMessage(uid, mid)](#module_rostermanage.recallmessage)
    * [.unreadMessage(uid, mid)](#module_rostermanage.unreadmessage)
    * [.deleteMessage(uid, mid)](#module_rostermanage.deletemessage)
    * [.getRosterInfo(rid)](#module_rostermanage.getrosterinfo) ⇒ [<code>RosterItem</code>](#module_types..rosteritem)
    * [.getUnreadCount(uid)](#module_rostermanage.getunreadcount) ⇒ <code>number</code>
    * [.asyncGetApplyList(params)](#module_rostermanage.asyncgetapplylist) ⇒ <code>Promise.&lt;Array.&lt;module:types~RosterApplication&gt;&gt;</code>
    * [.asyncGetBlockedlist(params)](#module_rostermanage.asyncgetblockedlist) ⇒ <code>Promise.&lt;Array.&lt;number&gt;&gt;</code>
    * [.asyncBlockeAdd(params)](#module_rostermanage.asyncblockeadd) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncBlockeRemove(params)](#module_rostermanage.asyncblockeremove) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncApply(params)](#module_rostermanage.asyncapply) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncAccept(params)](#module_rostermanage.asyncaccept) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncDecline(params)](#module_rostermanage.asyncdecline) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateRosterExt(params)](#module_rostermanage.asyncupdaterosterext) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncSearchRosterByName(params)](#module_rostermanage.asyncsearchrosterbyname) ⇒ [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..rosteritem)
    * [.asyncSearchRosterById(params)](#module_rostermanage.asyncsearchrosterbyid) ⇒ [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..rosteritem)

## rosterManage.asyncGetRosterIdList(force) ⇒ <code>Promise.&lt;Array.&lt;number&gt;&gt;</code> {#module_rostermanage.asyncgetrosteridlist}
获取好友id列表

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: <code>Promise.&lt;Array.&lt;number&gt;&gt;</code> - 用户ID列表  

| Param | Type | Description |
| --- | --- | --- |
| force | <code>boolean</code> | 是否强制从服务器拉取：true - 从服务器获取， false - 从本地存储获取 |

## rosterManage.asyncGetRosterInfo(roster_id, force) ⇒ [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..rosteritem) {#module_rostermanage.asyncgetrosterinfo}
获取好友信息

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..rosteritem) - 好友信息  

| Param | Type | Description |
| --- | --- | --- |
| roster_id | <code>number</code> | 好友ID |
| force | <code>boolean</code> | 是否强制从服务器拉取： true - 从服务器拉取， false - 优先从本地存储获取 |

## rosterManage.asyncRegester(opt) ⇒ [<code>Promise.&lt;UserSettings&gt;</code>](#module_types..usersettings) {#module_rostermanage.asyncregester}
用户注册

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: [<code>Promise.&lt;UserSettings&gt;</code>](#module_types..usersettings) - 用户设置  

| Param | Type | Description |
| --- | --- | --- |
| opt | <code>object</code> | 用户信息 |
| opt.username | <code>string</code> | 用户名 |
| opt.password | <code>string</code> | 密码 |

## rosterManage.asyncDeleteRoster(param) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_rostermanage.asyncdeleteroster}
删除好友

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 请求结果  

| Param | Type | Description |
| --- | --- | --- |
| param | <code>object</code> | 参数 |
| param.user_id | <code>number</code> | 好友的用户ID |

## rosterManage.asnycGetRosterListDetailByIds(roster_ids) ⇒ <code>Promise.&lt;Array.&lt;module:types~RosterItem&gt;&gt;</code> {#module_rostermanage.asnycgetrosterlistdetailbyids}
根据id列表获取用户详细信息

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~RosterItem&gt;&gt;</code> - 用户详细信息列表  

| Param | Type | Description |
| --- | --- | --- |
| roster_ids | <code>Array.&lt;number&gt;</code> | 用户ID列表 |

## rosterManage.getAllRosterDetail() ⇒ [<code>Array.&lt;RosterItem&gt;</code>](#module_types..rosteritem) {#module_rostermanage.getallrosterdetail}
获取缓存的所有用户详细信息

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: [<code>Array.&lt;RosterItem&gt;</code>](#module_types..rosteritem) - 用户详细信息列表  
## rosterManage.asyncGetUserProfile(force) ⇒ [<code>Promise.&lt;UserProfile&gt;</code>](#module_types..userprofile) {#module_rostermanage.asyncgetuserprofile}
获取自己的用户信息

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: [<code>Promise.&lt;UserProfile&gt;</code>](#module_types..userprofile) - 用户信息  

| Param | Type | Description |
| --- | --- | --- |
| force | <code>boolean</code> | 是否强制从服务器拉取： true - 从服务器拉取， false - 优先从本地存储获取 |

## rosterManage.getRosterMessageByRid(uid) ⇒ [<code>Array.&lt;Meta&gt;</code>](#module_types..meta) {#module_rostermanage.getrostermessagebyrid}
根据会话ID获取聊天消息

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: [<code>Array.&lt;Meta&gt;</code>](#module_types..meta) - 聊天消息列表  

| Param | Type | Description |
| --- | --- | --- |
| uid | <code>number</code> | 会话ID |

## rosterManage.readRosterMessage(roster_id, mid) {#module_rostermanage.readrostermessage}
修改消息状态为已读

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  

| Param | Type | Description |
| --- | --- | --- |
| roster_id | <code>number</code> | 会话ID |
| mid | <code>number</code> | 消息ID |

## rosterManage.recallMessage(uid, mid) {#module_rostermanage.recallmessage}
撤回消息，只能撤回5分钟内的

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  

| Param | Type | Description |
| --- | --- | --- |
| uid | <code>number</code> | 会话ID |
| mid | <code>number</code> | 消息ID |

## rosterManage.unreadMessage(uid, mid) {#module_rostermanage.unreadmessage}
设置消息成未读

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  

| Param | Type | Description |
| --- | --- | --- |
| uid | <code>number</code> | 会话ID |
| mid | <code>number</code> | 消息ID |

## rosterManage.deleteMessage(uid, mid) {#module_rostermanage.deletemessage}
删除消息

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  

| Param | Type | Description |
| --- | --- | --- |
| uid | <code>number</code> | 会话ID |
| mid | <code>number</code> | 消息ID |

## rosterManage.getRosterInfo(rid) ⇒ [<code>RosterItem</code>](#module_types..rosteritem) {#module_rostermanage.getrosterinfo}
获取好友信息

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: [<code>RosterItem</code>](#module_types..rosteritem) - 好友信息  

| Param | Type | Description |
| --- | --- | --- |
| rid | <code>number</code> | 好友ID |

## rosterManage.getUnreadCount(uid) ⇒ <code>number</code> {#module_rostermanage.getunreadcount}
获取指定会话的未读数

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: <code>number</code> - 未读数  

| Param | Type | Description |
| --- | --- | --- |
| uid | <code>number</code> | 会话IID |

## rosterManage.asyncGetApplyList(params) ⇒ <code>Promise.&lt;Array.&lt;module:types~RosterApplication&gt;&gt;</code> {#module_rostermanage.asyncgetapplylist}
获取好友申请列表

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: <code>Promise.&lt;Array.&lt;module:types~RosterApplication&gt;&gt;</code> - 好友申请列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.cursor | <code>number</code> | 从哪开始获取：可以传空字符串表示从头开始取 |

## rosterManage.asyncGetBlockedlist(params) ⇒ <code>Promise.&lt;Array.&lt;number&gt;&gt;</code> {#module_rostermanage.asyncgetblockedlist}
获取黑名单

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: <code>Promise.&lt;Array.&lt;number&gt;&gt;</code> - 用户ID列表  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数：空对象 |

## rosterManage.asyncBlockeAdd(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_rostermanage.asyncblockeadd}
加入黑名单

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.user_id | <code>number</code> | 用户ID |

## rosterManage.asyncBlockeRemove(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_rostermanage.asyncblockeremove}
移除黑名单

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.user_id | <code>number</code> | 用户ID |

## rosterManage.asyncApply(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_rostermanage.asyncapply}
请求加为好友

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.user_id | <code>number</code> | 用户ID |
| params.alias | <code>string</code> | 备注 |

## rosterManage.asyncAccept(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_rostermanage.asyncaccept}
通过好友申请

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.user_id | <code>number</code> | 用户ID |

## rosterManage.asyncDecline(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_rostermanage.asyncdecline}
拒绝好友申请

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.user_id | <code>number</code> | 用户ID |

## rosterManage.asyncUpdateRosterExt(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_rostermanage.asyncupdaterosterext}
修改好友扩展字段

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.user_id | <code>number</code> | 用户ID |
| params.ext | <code>string</code> | 扩展字段 |

## rosterManage.asyncSearchRosterByName(params) ⇒ [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..rosteritem) {#module_rostermanage.asyncsearchrosterbyname}
按名称搜索用户

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..rosteritem) - 用户信息  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.username | <code>string</code> | 用户名 |

## rosterManage.asyncSearchRosterById(params) ⇒ [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..rosteritem) {#module_rostermanage.asyncsearchrosterbyid}
按ID搜索用户

**Kind**: static method of [<code>rosterManage</code>](#module_rostermanage)  
**Returns**: [<code>Promise.&lt;RosterItem&gt;</code>](#module_types..rosteritem) - 用户信息  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.user_id | <code>number</code> | 用户ID |

# sysManage {#module_sysmanage}

* [sysManage](#module_sysmanage)
    * [.sendRosterMessage(msg)](#module_sysmanage.sendrostermessage) ⇒ <code>number</code>
    * [.sendGroupMessage(msg)](#module_sysmanage.sendgroupmessage) ⇒ <code>number</code>
    * [.requireHistoryMessage(uid, sid, amount)](#module_sysmanage.requirehistorymessage)
    * [.sendMentionMessage(params)](#module_sysmanage.sendmentionmessage) ⇒ <code>number</code>
    * [.sendInputStatusMessage(uid, status)](#module_sysmanage.sendinputstatusmessage) ⇒ <code>number</code>
    * [.forwardMessage(param)](#module_sysmanage.forwardmessage) ⇒ <code>number</code>
    * [.getMessageStatus(cid, mid, isGroup)](#module_sysmanage.getmessagestatus) ⇒ <code>string</code>
    * [.asyncFileUpload(param)](#module_sysmanage.asyncfileupload) ⇒ [<code>Promise.&lt;FileUploadResult&gt;</code>](#module_types..fileuploadresult)
    * [.getImage(param)](#module_sysmanage.getimage) ⇒ <code>string</code>
    * [.deleteConversation(id, other_devices)](#module_sysmanage.deleteconversation)
    * [.asyncGetGroupAvatarUploadUrl(params)](#module_sysmanage.asyncgetgroupavataruploadurl) ⇒ [<code>Promise.&lt;FileUpload&gt;</code>](#module_types..fileupload)
    * [.asyncGetFileUploadChatFileUrl(params)](#module_sysmanage.asyncgetfileuploadchatfileurl) ⇒ [<code>Promise.&lt;FileUpload&gt;</code>](#module_types..fileupload)

## sysManage.sendRosterMessage(msg) ⇒ <code>number</code> {#module_sysmanage.sendrostermessage}
发送单聊消息

**Kind**: static method of [<code>sysManage</code>](#module_sysmanage)  
**Returns**: <code>number</code> - 客户端生成的消息ID  

| Param | Type | Description |
| --- | --- | --- |
| msg | <code>object</code> | 消息体 |
| msg.uid | <code>string</code> | 接收者ID |
| msg.content | <code>string</code> | 消息内容 |
| msg.type | <code>string</code> | 消息类型： text - 文本, image - 图片， audio - 语音, video - 视频，file - 文件, location - 位置， command - 命令, forward - 转发 |
| msg.ext | <code>string</code> \| <code>object</code> | 扩展字段 |
| msg.attachment | <code>string</code> \| <code>object</code> | 附件信息 |

## sysManage.sendGroupMessage(msg) ⇒ <code>number</code> {#module_sysmanage.sendgroupmessage}
发送群聊消息

**Kind**: static method of [<code>sysManage</code>](#module_sysmanage)  
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

## sysManage.requireHistoryMessage(uid, sid, amount) {#module_sysmanage.requirehistorymessage}
请求历史消息

**Kind**: static method of [<code>sysManage</code>](#module_sysmanage)  

| Param | Type | Description |
| --- | --- | --- |
| uid | <code>number</code> | 会话ID |
| sid | <code>number</code> | 消息ID: 从哪个消息向前拉取，传0表示从最新一条消息开始拉取。 |
| amount | <code>number</code> | 拉取的条数 |

## sysManage.sendMentionMessage(params) ⇒ <code>number</code> {#module_sysmanage.sendmentionmessage}
群发送&#64;消息

**Kind**: static method of [<code>sysManage</code>](#module_sysmanage)  
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

## sysManage.sendInputStatusMessage(uid, status) ⇒ <code>number</code> {#module_sysmanage.sendinputstatusmessage}
发送输入状态消息

**Kind**: static method of [<code>sysManage</code>](#module_sysmanage)  
**Returns**: <code>number</code> - 客户端生成的消息ID  

| Param | Type | Description |
| --- | --- | --- |
| uid | <code>number</code> | 会话ID |
| status | <code>string</code> | 状态： nothing - 未输入， typing - 正在输入 |

## sysManage.forwardMessage(param) ⇒ <code>number</code> {#module_sysmanage.forwardmessage}
转发消息

**Kind**: static method of [<code>sysManage</code>](#module_sysmanage)  
**Returns**: <code>number</code> - 客户端生成的消息ID  

| Param | Type | Description |
| --- | --- | --- |
| param | <code>object</code> | 参数 |
| param.uid | <code>number</code> | 接收方用户ID（仅转发单聊时设置） |
| param.gid | <code>number</code> | 接收方群组ID（仅转发群聊时设置） |
| param.mid | <code>number</code> | 要转发的消息ID |

## sysManage.getMessageStatus(cid, mid, isGroup) ⇒ <code>string</code> {#module_sysmanage.getmessagestatus}
获取消息的状态

**Kind**: static method of [<code>sysManage</code>](#module_sysmanage)  
**Returns**: <code>string</code> - 消息状态:   unread - 未读， delivered - 已投递， read - 已读  

| Param | Type | Default | Description |
| --- | --- | --- | --- |
| cid | <code>number</code> |  | 会话ID |
| mid | <code>number</code> |  | 消息ID |
| isGroup | <code>boolean</code> | <code>false</code> | 是否是群聊 |

## sysManage.asyncFileUpload(param) ⇒ [<code>Promise.&lt;FileUploadResult&gt;</code>](#module_types..fileuploadresult) {#module_sysmanage.asyncfileupload}
上传文件

**Kind**: static method of [<code>sysManage</code>](#module_sysmanage)  
**Returns**: [<code>Promise.&lt;FileUploadResult&gt;</code>](#module_types..fileuploadresult) - 文件上传结果  

| Param | Type | Description |
| --- | --- | --- |
| param | <code>object</code> | 参数 |
| param.group_d | <code>number</code> | 群组ID |
| param.toType | <code>number</code> | 接收者类型：rosterAvatar - 用户头像， chat - 聊天文件， groupAvatar - 群头像 |
| param.to_id | <code>number</code> | 接收者ID |
| param.file | <code>File</code> | 文件 |
| param.fileType | <code>string</code> | 文件类型：file - 普通聊天文件, audio - 语音聊天文件(amr格式),image - 图片聊天文件, video - 视频聊天文件, audio-mp3 - 语音聊天文件(mp3格式), shareFile - 普通共享文件, shareAudio - 语音共享文件, shareImage - 图片共享文件, shareVideo - 视频共享文件 |
| param.chatType | <code>number</code> | 聊天类型： roster - 单聊, group - 群聊 |
| param.processCallback | [<code>fileUploadProgress</code>](#module_types..fileuploadprogress) | 上传进度回调 |

## sysManage.getImage(param) ⇒ <code>string</code> {#module_sysmanage.getimage}
拼装图片路径

**Kind**: static method of [<code>sysManage</code>](#module_sysmanage)  
**Returns**: <code>string</code> - 图片地址  

| Param | Type | Description |
| --- | --- | --- |
| param | <code>object</code> |  |
| param.avatar | <code>string</code> | 文件地址 |
| param.type | <code>string</code> | 类型： roster - 用户, group - 群 |
| param.thumbnail | <code>boolean</code> | 是否缩略图：默认为true |
| param.sdefault | <code>string</code> | 默认图片地址 |

## sysManage.deleteConversation(id, other_devices) {#module_sysmanage.deleteconversation}
删除会话

**Kind**: static method of [<code>sysManage</code>](#module_sysmanage)  

| Param | Type | Default | Description |
| --- | --- | --- | --- |
| id | <code>number</code> |  | 会话ID |
| other_devices | <code>boolean</code> | <code>true</code> | 是否同时删除其它设备上的会话 |

## sysManage.asyncGetGroupAvatarUploadUrl(params) ⇒ [<code>Promise.&lt;FileUpload&gt;</code>](#module_types..fileupload) {#module_sysmanage.asyncgetgroupavataruploadurl}
获取上传群头像URL

**Kind**: static method of [<code>sysManage</code>](#module_sysmanage)  
**Returns**: [<code>Promise.&lt;FileUpload&gt;</code>](#module_types..fileupload) - 文件上传信息  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.group_id | <code>number</code> | 群组ID |

## sysManage.asyncGetFileUploadChatFileUrl(params) ⇒ [<code>Promise.&lt;FileUpload&gt;</code>](#module_types..fileupload) {#module_sysmanage.asyncgetfileuploadchatfileurl}
获取聊天文件上传地址

**Kind**: static method of [<code>sysManage</code>](#module_sysmanage)  
**Returns**: [<code>Promise.&lt;FileUpload&gt;</code>](#module_types..fileupload) - 文件上传信息  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.file_type | <code>number</code> | 文件类型: 100 - 普通聊天文件, 101 - 语音聊天文件(amr格式),102 - 图片聊天文件, 103 - 视频聊天文件, 104 - 语音聊天文件(mp3格式)200 - 普通共享文件, 201 - 语音共享文件, 202 - 图片共享文件, 203 - 视频共享文件 |
| params.to_type | <code>number</code> | 会话类型： 1 - 用户，2 - 群组 |
| params.to_id | <code>number</code> | 会话ID |

# userManage {#module_usermanage}

* [userManage](#module_usermanage)
    * [.getToken()](#module_usermanage.gettoken) ⇒ <code>string</code>
    * [.getUid()](#module_usermanage.getuid) ⇒ <code>number</code>
    * [.getAppid()](#module_usermanage.getappid) ⇒ <code>string</code>
    * [.getConversationList()](#module_usermanage.getconversationlist) ⇒ [<code>Array.&lt;ConversationItem&gt;</code>](#module_types..conversationitem)
    * [.asyncUpdateAvatar(params)](#module_usermanage.asyncupdateavatar) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncUpdateNickName(params)](#module_usermanage.asyncupdatenickname) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncGetProfile()](#module_usermanage.asyncgetprofile) ⇒ [<code>Promise.&lt;UserProfile&gt;</code>](#module_types..userprofile)
    * [.asyncUpdateProfile(params)](#module_usermanage.asyncupdateprofile) ⇒ <code>Promise.&lt;boolean&gt;</code>
    * [.asyncGetSettings()](#module_usermanage.asyncgetsettings) ⇒ [<code>Promise.&lt;UserSettings&gt;</code>](#module_types..usersettings)
    * [.asyncUpdateSettings(settings)](#module_usermanage.asyncupdatesettings) ⇒ <code>Promise.&lt;boolean&gt;</code>

## userManage.getToken() ⇒ <code>string</code> {#module_usermanage.gettoken}
获取登录用户的token

**Kind**: static method of [<code>userManage</code>](#module_usermanage)  
**Returns**: <code>string</code> - 用户的token  
## userManage.getUid() ⇒ <code>number</code> {#module_usermanage.getuid}
获取登录用户的uid

**Kind**: static method of [<code>userManage</code>](#module_usermanage)  
**Returns**: <code>number</code> - 用户ID  
## userManage.getAppid() ⇒ <code>string</code> {#module_usermanage.getappid}
获取appid

**Kind**: static method of [<code>userManage</code>](#module_usermanage)  
**Returns**: <code>string</code> - APP ID  
## userManage.getConversationList() ⇒ [<code>Array.&lt;ConversationItem&gt;</code>](#module_types..conversationitem) {#module_usermanage.getconversationlist}
获取最近会话列表

**Kind**: static method of [<code>userManage</code>](#module_usermanage)  
## userManage.asyncUpdateAvatar(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_usermanage.asyncupdateavatar}
更新头像

**Kind**: static method of [<code>userManage</code>](#module_usermanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.avatar | <code>string</code> | 头像 url |

## userManage.asyncUpdateNickName(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_usermanage.asyncupdatenickname}
更新昵称

**Kind**: static method of [<code>userManage</code>](#module_usermanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> | 参数 |
| params.nick_name | <code>string</code> | 昵称 |

## userManage.asyncGetProfile() ⇒ [<code>Promise.&lt;UserProfile&gt;</code>](#module_types..userprofile) {#module_usermanage.asyncgetprofile}
获取用户profile

**Kind**: static method of [<code>userManage</code>](#module_usermanage)  
**Returns**: [<code>Promise.&lt;UserProfile&gt;</code>](#module_types..userprofile) - 用户信息  
## userManage.asyncUpdateProfile(params) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_usermanage.asyncupdateprofile}
更新用户profile

**Kind**: static method of [<code>userManage</code>](#module_usermanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| params | <code>object</code> |  |
| params.description | <code>string</code> | 描述信息 |
| params.nick_name | <code>string</code> | 昵称 |
| params.private_info | <code>string</code> | 私有信息，仅自己可见 |
| params.public_info | <code>string</code> | 公开信息，好友和陌生人可见 |

## userManage.asyncGetSettings() ⇒ [<code>Promise.&lt;UserSettings&gt;</code>](#module_types..usersettings) {#module_usermanage.asyncgetsettings}
获取用户设置信息

**Kind**: static method of [<code>userManage</code>](#module_usermanage)  
**Returns**: [<code>Promise.&lt;UserSettings&gt;</code>](#module_types..usersettings) - 用户信息  
## userManage.asyncUpdateSettings(settings) ⇒ <code>Promise.&lt;boolean&gt;</code> {#module_usermanage.asyncupdatesettings}
修改用户设置

**Kind**: static method of [<code>userManage</code>](#module_usermanage)  
**Returns**: <code>Promise.&lt;boolean&gt;</code> - 是否成功  

| Param | Type | Description |
| --- | --- | --- |
| settings | [<code>UserSettings</code>](#module_types..usersettings) | 更新的设置 |

# types {#module_types}

* [types](#module_types)
    * ["flooNotice" (res)](#event_floonotice)
    * ["flooError" (res)](#event_flooerror)
    * ["loginFail" (desc)](#event_loginfail)
    * ["loginSuccess" (res)](#event_loginsuccess)
    * ["onGroupListUpdate" (meta)](#event_ongrouplistupdate)
    * ["onGroupMemberChanged" (groupId)](#event_ongroupmemberchanged)
    * ["onGroupMessage" (meta)](#event_ongroupmessage)
    * ["onInputStatusMessage" (res)](#event_oninputstatusmessage)
    * ["onMentionMessage" (meta)](#event_onmentionmessage)
    * ["onMessageCanceled" (res)](#event_onmessagecanceled)
    * ["onMessageDeleted" (res)](#event_onmessagedeleted)
    * ["onMessageRecalled" (res)](#event_onmessagerecalled)
    * ["onMessageStatusChanged" (res)](#event_onmessagestatuschanged)
    * ["onReceiveHistoryMsg" (res)](#event_onreceivehistorymsg)
    * ["onRosterInfoUpdate" (res)](#event_onrosterinfoupdate)
    * ["onRosterListUpdate" (meta)](#event_onrosterlistupdate)
    * ["onRosterMessage" (meta)](#event_onrostermessage)
    * ["onSendingMessageStatusChanged" (res)](#event_onsendingmessagestatuschanged)
    * ["onUnreadChange" (cid)](#event_onunreadchange)
    * ["recentlistUpdate"](#event_recentlistupdate)
    * ["onGroupCreated" (meta)](#event_ongroupcreated)
    * ["onGroupDestoryed" (meta)](#event_ongroupdestoryed)
    * ["onGroupJoined" (meta)](#event_ongroupjoined)
    * ["onGroupApplyAccepted" (meta)](#event_ongroupapplyaccepted)
    * ["onGroupApplyDeclined" (meta)](#event_ongroupapplydeclined)
    * ["onGroupBaned" (meta)](#event_ongroupbaned)
    * ["onGroupUnbaned" (meta)](#event_ongroupunbaned)
    * [~RosterItem](#module_types..rosteritem) : <code>object</code>
    * [~UserSettings](#module_types..usersettings) : <code>object</code>
    * [~UserProfile](#module_types..userprofile) : <code>object</code>
    * [~Meta](#module_types..meta) : <code>object</code>
    * [~RosterApplication](#module_types..rosterapplication) : <code>object</code>
    * [~GroupInfoAndSettings](#module_types..groupinfoandsettings) : <code>object</code>
    * [~BriefGroupInfoAndSettings](#module_types..briefgroupinfoandsettings) : <code>object</code>
    * [~GroupMember](#module_types..groupmember) : <code>object</code>
    * [~GroupMemberBanned](#module_types..groupmemberbanned) : <code>object</code>
    * [~GroupUserRelationResponse](#module_types..groupuserrelationresponse) : <code>object</code>
    * [~GroupAnnouncement](#module_types..groupannouncement) : <code>object</code>
    * [~GroupInfoRequest](#module_types..groupinforequest) : <code>object</code>
    * [~GroupBannedMemberRequest](#module_types..groupbannedmemberrequest) : <code>object</code>
    * [~GroupBlockedListItem](#module_types..groupblockedlistitem) : <code>object</code>
    * [~GroupInvitation](#module_types..groupinvitation) : <code>object</code>
    * [~GroupApplication](#module_types..groupapplication) : <code>object</code>
    * [~GroupSharedFile](#module_types..groupsharedfile) : <code>object</code>
    * [~GroupSharedFileResponse](#module_types..groupsharedfileresponse) : <code>object</code>
    * [~GroupBanAllResponse](#module_types..groupbanallresponse) : <code>object</code>
    * [~FileUpload](#module_types..fileupload) : <code>object</code>
    * [~FileUploadResult](#module_types..fileuploadresult) : <code>object</code>
    * [~fileUploadProgress](#module_types..fileuploadprogress) : <code>function</code>
    * [~ConversationItem](#module_types..conversationitem) : <code>object</code>
    * [~UserProfile](#module_types..userprofile) : <code>object</code>
    * [~UserSettings](#module_types..usersettings) : <code>object</code>
    * [~Event](#module_types..event) : <code>string</code>
    * [~EventCallback](#module_types..eventcallback) : <code>function</code>

## "flooNotice" (res) {#event_floonotice}
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
## "flooError" (res) {#event_flooerror}
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
## "loginFail" (desc) {#event_loginfail}
登录失败

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| desc | <code>string</code> | 失败原因 |

## "loginSuccess" (res) {#event_loginsuccess}
登录成功

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> | 空对象 |

## "onGroupListUpdate" (meta) {#event_ongrouplistupdate}
群列表更新

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..meta) \| <code>undefined</code> | 通知消息内容 |

## "onGroupMemberChanged" (groupId) {#event_ongroupmemberchanged}
群成员列表更新

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| groupId | <code>number</code> | 群ID |

## "onGroupMessage" (meta) {#event_ongroupmessage}
收到群消息

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..meta) | 消息内容 |

## "onInputStatusMessage" (res) {#event_oninputstatusmessage}
对方正在输入

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> |  |
| res.ext | <code>string</code> | 扩展字段 |
| res.from | <code>string</code> | 发送者用户ID |
| res.to | <code>string</code> | 接收者用户ID |

## "onMentionMessage" (meta) {#event_onmentionmessage}
收到群组&#64;消息

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..meta) | 消息内容 |

## "onMessageCanceled" (res) {#event_onmessagecanceled}
消息被取消已读

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> |  |
| res.uid | <code>string</code> | 会话ID |
| res.mid | <code>string</code> | 消息ID |

## "onMessageDeleted" (res) {#event_onmessagedeleted}
消息被删除

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> |  |
| res.uid | <code>string</code> | 会话ID |
| res.mid | <code>string</code> | 消息ID |

## "onMessageRecalled" (res) {#event_onmessagerecalled}
消息被撤回

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> |  |
| res.uid | <code>string</code> | 会话ID |
| res.mid | <code>string</code> | 消息ID |

## "onMessageStatusChanged" (res) {#event_onmessagestatuschanged}
消息状态变更：撤回/删除/已读

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> |  |
| res.uid | <code>string</code> | 会话ID |
| res.mid | <code>string</code> | 消息ID |

## "onReceiveHistoryMsg" (res) {#event_onreceivehistorymsg}
收到历史消息

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> |  |
| res.next | <code>number</code> | 下次取历史消息的key |

## "onRosterInfoUpdate" (res) {#event_onrosterinfoupdate}
好友信息变更

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> |  |
| res.rosterIds | <code>Array.&lt;number&gt;</code> | 好友的用户ID列表 |

## "onRosterListUpdate" (meta) {#event_onrosterlistupdate}
好友列表变更

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..meta) | 好友通知的消息内容 |

## "onRosterMessage" (meta) {#event_onrostermessage}
收到单聊消息

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..meta) | 消息内容 |

## "onSendingMessageStatusChanged" (res) {#event_onsendingmessagestatuschanged}
消息发送状态变更

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> |  |
| res.status: | <code>number</code> | 发送状态，取值为sending|failed|sent |
| res.mid: | <code>number</code> | 客户端生成的client_mid |

## "onUnreadChange" (cid) {#event_onunreadchange}
未读数改变

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| cid | <code>number</code> | 会话ID |

## "recentlistUpdate" {#event_recentlistupdate}
最近会话更新

**Kind**: event emitted by [<code>types</code>](#module_types)  
## "onGroupCreated" (meta) {#event_ongroupcreated}
群组创建通知

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..meta) | 群通知的消息内容 |

## "onGroupDestoryed" (meta) {#event_ongroupdestoryed}
群组解散通知

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..meta) | 群通知的消息内容 |

## "onGroupJoined" (meta) {#event_ongroupjoined}
成员入群通知

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..meta) | 群通知的消息内容 |

## "onGroupApplyAccepted" (meta) {#event_ongroupapplyaccepted}
群申请被通过

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..meta) | 群通知的消息内容 |

## "onGroupApplyDeclined" (meta) {#event_ongroupapplydeclined}
群申请被拒绝

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..meta) | 群通知的消息内容 |

## "onGroupBaned" (meta) {#event_ongroupbaned}
被群禁言

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..meta) | 群通知的消息内容 |

## "onGroupUnbaned" (meta) {#event_ongroupunbaned}
被群取消禁言

**Kind**: event emitted by [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| meta | [<code>Meta</code>](#module_types..meta) | 群通知的消息内容 |

## types~RosterItem : <code>object</code> {#module_types..rosteritem}
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

## types~UserSettings : <code>object</code> {#module_types..usersettings}
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

## types~UserProfile : <code>object</code> {#module_types..userprofile}
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

## types~Meta : <code>object</code> {#module_types..meta}
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

## types~RosterApplication : <code>object</code> {#module_types..rosterapplication}
加好友申请列表项

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| expired_time | <code>number</code> | 过期时间,int64 |
| reason | <code>string</code> | 申请描述 |
| status | <code>number</code> | 状态： 0 - 等待确认， 1 - 接受， 2 - 拒绝。 int32 |
| user_id | <code>number</code> | 发起加好友申请的用户ID,int64 |

## types~GroupInfoAndSettings : <code>object</code> {#module_types..groupinfoandsettings}
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

## types~BriefGroupInfoAndSettings : <code>object</code> {#module_types..briefgroupinfoandsettings}
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

## types~GroupMember : <code>object</code> {#module_types..groupmember}
群成员格式

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| display_name | <code>string</code> | 成员群名片 |
| join_time | <code>number</code> | 成员入群时间,int64 |
| user_id | <code>number</code> | 用户id,int64 |
| avatar | <code>string</code> | 头像地址 |

## types~GroupMemberBanned : <code>object</code> {#module_types..groupmemberbanned}
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

## types~GroupUserRelationResponse : <code>object</code> {#module_types..groupuserrelationresponse}
群用户请求结果

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| reason | <code>string</code> | 原因 |
| result | <code>string</code> | 结果 |
| user_id | <code>number</code> | 用户ID，int64 |

## types~GroupAnnouncement : <code>object</code> {#module_types..groupannouncement}
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

## types~GroupInfoRequest : <code>object</code> {#module_types..groupinforequest}
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

## types~GroupBannedMemberRequest : <code>object</code> {#module_types..groupbannedmemberrequest}
禁言请求

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| duration | <code>number</code> | 禁言时长，单位为分钟,int64 |
| group_id | <code>number</code> | 群id,int64 |
| user_list | <code>Array.&lt;number&gt;</code> | 用户id列表 |

## types~GroupBlockedListItem : <code>object</code> {#module_types..groupblockedlistitem}
群组黑名单

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| user_id | <code>number</code> | 用户id,int64 |
| group_id | <code>number</code> | 群id,int64 |
| create_at | <code>string</code> | 创建时间 |

## types~GroupInvitation : <code>object</code> {#module_types..groupinvitation}
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

## types~GroupApplication : <code>object</code> {#module_types..groupapplication}
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

## types~GroupSharedFile : <code>object</code> {#module_types..groupsharedfile}
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

## types~GroupSharedFileResponse : <code>object</code> {#module_types..groupsharedfileresponse}
删除群共享文件结果

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| file_id | <code>number</code> | 文件ID |
| reason | <code>string</code> | 原因 |
| result | <code>string</code> | 结果 |

## types~GroupBanAllResponse : <code>object</code> {#module_types..groupbanallresponse}
全员禁言结果

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| ban_expire_time | <code>number</code> | 全员禁言过期时间,int64 |

## types~FileUpload : <code>object</code> {#module_types..fileupload}
文件上传信息

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| download_url | <code>string</code> | 下载地址 |
| oss_body_param | <code>object.&lt;string, string&gt;</code> | 额外参数 |
| upload_url | <code>string</code> | 上传地址 |

## types~FileUploadResult : <code>object</code> {#module_types..fileuploadresult}
文件上传结果

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| url | <code>string</code> | 下载地址 |

## types~fileUploadProgress : <code>function</code> {#module_types..fileuploadprogress}
文件上传进度回调

**Kind**: inner typedef of [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | <code>object</code> | 进度 |
| res.loaded | <code>number</code> | 已下载字节数 |
| res.total | <code>number</code> | 总字节数 |

## types~ConversationItem : <code>object</code> {#module_types..conversationitem}
会话信息

**Kind**: inner typedef of [<code>types</code>](#module_types)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| id | <code>number</code> | 会话ID |
| content | <code>string</code> | 消息内容 |
| timestamp | <code>string</code> | 消息发送时间戳（毫秒） |
| type | <code>string</code> | 会话类型： roster - 单聊， group - 群聊 |

## types~UserProfile : <code>object</code> {#module_types..userprofile}
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

## types~UserSettings : <code>object</code> {#module_types..usersettings}
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

## types~Event : <code>string</code> {#module_types..event}
监听事件名称

**Kind**: inner typedef of [<code>types</code>](#module_types)  
## types~EventCallback : <code>function</code> {#module_types..eventcallback}
监听事件回调

**Kind**: inner typedef of [<code>types</code>](#module_types)  

| Param | Type | Description |
| --- | --- | --- |
| res | [<code>flooNotice</code>](#event_floonotice) \| [<code>flooError</code>](#event_flooerror) \| [<code>loginFail</code>](#event_loginfail) \| [<code>loginSuccess</code>](#event_loginsuccess) \| [<code>onGroupListUpdate</code>](#event_ongrouplistupdate) \| [<code>onGroupMemberChanged</code>](#event_ongroupmemberchanged) \| [<code>onGroupMessage</code>](#event_ongroupmessage) \| [<code>onInputStatusMessage</code>](#event_oninputstatusmessage) \| [<code>onMentionMessage</code>](#event_onmentionmessage) \| [<code>onMessageCanceled</code>](#event_onmessagecanceled) \| [<code>onMessageDeleted</code>](#event_onmessagedeleted) \| [<code>onMessageRecalled</code>](#event_onmessagerecalled) \| [<code>onMessageStatusChanged</code>](#event_onmessagestatuschanged) \| [<code>onReceiveHistoryMsg</code>](#event_onreceivehistorymsg) \| [<code>onRosterInfoUpdate</code>](#event_onrosterinfoupdate) \| [<code>onRosterListUpdate</code>](#event_onrosterlistupdate) \| [<code>onRosterMessage</code>](#event_onrostermessage) \| [<code>onSendingMessageStatusChanged</code>](#event_onsendingmessagestatuschanged) \| [<code>onUnreadChange</code>](#event_onunreadchange) \| [<code>recentlistUpdate</code>](#event_recentlistupdate) \| [<code>onGroupCreated</code>](#event_ongroupcreated) \| [<code>onGroupDestoryed</code>](#event_ongroupdestoryed) \| [<code>onGroupJoined</code>](#event_ongroupjoined) \| [<code>onGroupApplyAccepted</code>](#event_ongroupapplyaccepted) \| [<code>onGroupApplyDeclined</code>](#event_ongroupapplydeclined) \| [<code>onGroupBaned</code>](#event_ongroupbaned) \| [<code>onGroupUnbaned</code>](#event_ongroupunbaned) | 事件结果 |

# flooim {#module_flooim}

* [flooim](#module_flooim)
    * [.flooim(config)](#module_flooim.flooim) ⇒ <code>object</code>
    * [.login(opt)](#module_flooim.login)
    * [.qrlogin(opt)](#module_flooim.qrlogin)
    * [.tokenLogin(opt)](#module_flooim.tokenlogin)
    * [.idLogin(opt)](#module_flooim.idlogin)
    * [.isLogin()](#module_flooim.islogin) ⇒ <code>boolean</code>
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

## flooim.tokenLogin(opt) {#module_flooim.tokenlogin}
token登录

**Kind**: static method of [<code>flooim</code>](#module_flooim)  

| Param | Type | Description |
| --- | --- | --- |
| opt | <code>object</code> |  |
| opt.user_id | <code>number</code> | 用户ID |
| opt.token | <code>string</code> | Token |

## flooim.idLogin(opt) {#module_flooim.idlogin}
使用用户ID和密码登录

**Kind**: static method of [<code>flooim</code>](#module_flooim)  

| Param | Type | Description |
| --- | --- | --- |
| opt | <code>object</code> |  |
| opt.user_id | <code>number</code> | 用户ID |
| opt.password | <code>string</code> | 密码 |

## flooim.isLogin() ⇒ <code>boolean</code> {#module_flooim.islogin}
是否已登录

**Kind**: static method of [<code>flooim</code>](#module_flooim)  
**Returns**: <code>boolean</code> - 是否已登录  
## flooim.on(options, ext) {#module_flooim.on}
事件监听

**Kind**: static method of [<code>flooim</code>](#module_flooim)  

| Param | Type | Description |
| --- | --- | --- |
| options | [<code>Event</code>](#module_types..event) \| <code>Object.&lt;module:types~Event, module:types~EventCallback&gt;</code> | 可以为事件名，也可以为事件名和事件回调 |
| ext | [<code>EventCallback</code>](#module_types..eventcallback) \| <code>undefined</code> | 事件回调，只有options为事件名时需要设置 |

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
| options | [<code>Event</code>](#module_types..event) \| <code>Object.&lt;module:types~Event, module:types~EventCallback&gt;</code> | 可以为事件名，也可以为事件名和事件回调 |
| ext | [<code>EventCallback</code>](#module_types..eventcallback) \| <code>undefined</code> | 事件回调，只有options为事件名时需要设置 |

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
