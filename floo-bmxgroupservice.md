# floo::BMXGroupService

群组Service

`#include <bmx_group_service.h>`

## Public Types

|                                                   | Name                      |
| ------------------------------------------------- | ------------------------- |
| typedef std::function< void(int percent)>         | **Callback**              |
| typedef std::shared\_ptr< \[CreateGroupOptions] > | **CreateGroupOptionsPtr** |

## Public Functions

|                      | Name                                                                                                                                                                                                          |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| virtual              | **\~BMXGroupService**()                                                                                                                                                                                       |
| virtual BMXErrorCode | <p><strong>get</strong>(BMXGroupList &#x26; list, bool forceRefresh) =0<br>获取群组列表，如果设置了forceRefresh则从服务器拉取</p>                                                                                                |
| virtual BMXErrorCode | <p><strong>search</strong>(BMXGroupList &#x26; list, bool forceRefresh) =0<br>Deprecated.</p>                                                                                                                 |
| virtual BMXErrorCode | <p><strong>fetchGroupsByIdList</strong>(const std::vector&#x3C; int64_t > &#x26; groupIdList, BMXGroupList &#x26; list, bool forceRefresh) =0<br>通过传入群组的id列表获取群组信息列表，如果设置了forceRefresh则从服务器拉取</p>             |
| virtual BMXErrorCode | <p><strong>search</strong>(const std::vector&#x3C; int64_t > &#x26; groupIdList, BMXGroupList &#x26; list, bool forceRefresh) =0<br>Deprecated.</p>                                                           |
| virtual BMXErrorCode | <p><strong>fetchGroupById</strong>(int64_t groupId, BMXGroupPtr &#x26; group, bool forceRefresh) =0<br>通过群组id获取群信息，如果设置了forceRefresh则从服务器拉取</p>                                                               |
| virtual BMXErrorCode | <p><strong>search</strong>(int64_t groupId, BMXGroupPtr &#x26; group, bool forceRefresh) =0<br>Deprecated.</p>                                                                                                |
| virtual BMXErrorCode | <p><strong>fetchLocalGroupsByName</strong>(BMXGroupList &#x26; list, const std::string &#x26; name) =0<br>通过群名称查询本地群信息，从本地数据库中通过群名称查询获取群组</p>                                                                 |
| virtual BMXErrorCode | <p><strong>search</strong>(BMXGroupList &#x26; list, const std::string &#x26; name) =0<br>Deprecated.</p>                                                                                                     |
| virtual BMXErrorCode | <p><strong>create</strong>(const [CreateGroupOptions] &#x26; options, BMXGroupPtr &#x26; group) =0<br>创建群</p>                                                                                                 |
| virtual BMXErrorCode | <p><strong>destroy</strong>(BMXGroupPtr group) =0<br>销毁群</p>                                                                                                                                                  |
| virtual BMXErrorCode | <p><strong>join</strong>(BMXGroupPtr group, const std::string &#x26; message) =0<br>加入一个群，根据群设置可能需要管理员批准</p>                                                                                                  |
| virtual BMXErrorCode | <p><strong>leave</strong>(BMXGroupPtr group) =0<br>退出群</p>                                                                                                                                                    |
| virtual BMXErrorCode | <p><strong>getInfo</strong>(BMXGroupPtr group) =0<br>获取群详情，从服务端拉取最新信息</p>                                                                                                                                     |
| virtual BMXErrorCode | <p><strong>getMembersNickname</strong>(BMXGroupPtr group, const std::vector&#x3C; int64_t > &#x26; members, BMXGroup::MemberList &#x26; list) =0<br>获取群组成员详细信息</p>                                            |
| virtual BMXErrorCode | <p><strong>getInvitationList</strong>(BMXGroupInvitationPagePtr &#x26; result, const std::string &#x26; cursor ="", int pageSize =10) =0<br>分页获取群组邀请列表</p>                                                    |
| virtual BMXErrorCode | <p><strong>getApplicationList</strong>(BMXGroupList list, BMXGroupApplicationPagePtr &#x26; result, const std::string &#x26; cursor ="", int pageSize =10) =0<br>分页获取群组申请列表</p>                               |
| virtual BMXErrorCode | <p><strong>getMembers</strong>(BMXGroupPtr group, BMXGroupMemberResultPagePtr &#x26; result, const std::string &#x26; cursor ="", int pageSize =200) =0<br>分页获取群成员列表，如果设置了forceRefresh则从服务器拉取，单页最大数量为500.</p> |
| virtual BMXErrorCode | <p><strong>getMembers</strong>(BMXGroupPtr group, BMXGroup::MemberList &#x26; list, bool forceRefresh) =0<br>获取群成员列表，如果设置了forceRefresh则从服务器拉取，最多拉取1000人</p>                                                   |
| virtual BMXErrorCode | <p><strong>addMembers</strong>(BMXGroupPtr group, const std::vector&#x3C; int64_t > &#x26; members, const std::string &#x26; message) =0<br>添加群成员</p>                                                         |
| virtual BMXErrorCode | <p><strong>removeMembers</strong>(BMXGroupPtr group, const std::vector&#x3C; int64_t > &#x26; members, const std::string &#x26; reason) =0<br>删除群成员</p>                                                       |
| virtual BMXErrorCode | <p><strong>addAdmins</strong>(BMXGroupPtr group, const std::vector&#x3C; int64_t > &#x26; admins, const std::string &#x26; message) =0<br>添加管理员</p>                                                           |
| virtual BMXErrorCode | <p><strong>removeAdmins</strong>(BMXGroupPtr group, const std::vector&#x3C; int64_t > &#x26; admins, const std::string &#x26; reason) =0<br>删除管理员</p>                                                         |
| virtual BMXErrorCode | <p><strong>getAdmins</strong>(BMXGroupPtr group, BMXGroup::MemberList &#x26; list, bool forceRefresh) =0<br>获取Admins列表，如果设置了forceRefresh则从服务器拉取</p>                                                           |
| virtual BMXErrorCode | <p><strong>blockMembers</strong>(BMXGroupPtr group, const std::vector&#x3C; int64_t > &#x26; members) =0<br>添加黑名单</p>                                                                                         |
| virtual BMXErrorCode | <p><strong>unblockMembers</strong>(BMXGroupPtr group, const std::vector&#x3C; int64_t > &#x26; members) =0<br>从黑名单删除</p>                                                                                      |
| virtual BMXErrorCode | <p><strong>getBlockList</strong>(BMXGroupPtr group, BMXGroupMemberResultPagePtr &#x26; result, const std::string &#x26; cursor ="", int pageSize =200) =0<br>分页获取黑名单</p>                                      |
| virtual BMXErrorCode | <p><strong>getBlockList</strong>(BMXGroupPtr group, BMXGroup::MemberList &#x26; list, bool forceRefresh) =0<br>获取黑名单</p>                                                                                      |
| virtual BMXErrorCode | <p><strong>banMembers</strong>(BMXGroupPtr group, const std::vector&#x3C; int64_t > &#x26; members, int64_t duration, const std::string &#x26; reason ="") =0<br>禁言</p>                                       |
| virtual BMXErrorCode | <p><strong>banGroup</strong>(BMXGroupPtr group, int64_t duration) =0<br>全员禁言，当前服务器时间加上禁言时长后计算出全员禁言到期时间（只有管理和群主可以发言）</p>                                                                                       |
| virtual BMXErrorCode | <p><strong>unbanMembers</strong>(BMXGroupPtr group, const std::vector&#x3C; int64_t > &#x26; members) =0<br>解除禁言</p>                                                                                          |
| virtual BMXErrorCode | <p><strong>unbanGroup</strong>(BMXGroupPtr group) =0<br>全员解除禁言</p>                                                                                                                                            |
| virtual BMXErrorCode | <p><strong>getBannedMembers</strong>(BMXGroupPtr group, BMXGroupBannedMemberResultPagePtr &#x26; result, const std::string &#x26; cursor ="", int pageSize =200) =0<br>分页获取禁言列表</p>                           |
| virtual BMXErrorCode | <p><strong>getBannedMembers</strong>(BMXGroupPtr group, BMXGroup::BannedMemberList &#x26; list) =0<br>获取禁言列表</p>                                                                                              |
| virtual BMXErrorCode | <p><strong>muteMessage</strong>(BMXGroupPtr group, BMXGroup::MsgMuteMode mode) =0<br>设置是否屏蔽群消息</p>                                                                                                            |
| virtual BMXErrorCode | <p><strong>acceptApplication</strong>(BMXGroupPtr group, int64_t applicantId) =0<br>接受入群申请</p>                                                                                                                |
| virtual BMXErrorCode | <p><strong>declineApplication</strong>(BMXGroupPtr group, int64_t applicantId, const std::string &#x26; reason ="") =0<br>拒绝入群申请</p>                                                                          |
| virtual BMXErrorCode | <p><strong>acceptInvitation</strong>(BMXGroupPtr group, int64_t inviter) =0<br>接受入群邀请</p>                                                                                                                     |
| virtual BMXErrorCode | <p><strong>declineInvitation</strong>(BMXGroupPtr group, int64_t inviter, const std::string &#x26; reason ="") =0<br>拒绝入群邀请</p>                                                                               |
| virtual BMXErrorCode | <p><strong>transferOwner</strong>(BMXGroupPtr group, int64_t newOwnerId) =0<br>转移群主</p>                                                                                                                       |
| virtual BMXErrorCode | <p><strong>uploadSharedFile</strong>(BMXGroupPtr group, const std::string &#x26; filePath, const std::string &#x26; displayName, const std::string &#x26; extensionName, Callback ) =0<br>添加群共享文件</p>         |
| virtual BMXErrorCode | <p><strong>cancelUploadSharedFile</strong>(BMXGroupPtr group, const std::string &#x26; filePath) =0<br>取消上传群共享文件</p>                                                                                          |
| virtual BMXErrorCode | <p><strong>removeSharedFile</strong>(BMXGroupPtr group, BMXGroup::SharedFilePtr sharedFile) =0<br>移除群共享文件</p>                                                                                                 |
| virtual BMXErrorCode | <p><strong>downloadSharedFile</strong>(BMXGroupPtr group, BMXGroup::SharedFilePtr sharedFile, Callback ) =0<br>下载群共享文件</p>                                                                                    |
| virtual BMXErrorCode | <p><strong>cancelDownloadSharedFile</strong>(BMXGroupPtr group, BMXGroup::SharedFilePtr sharedFile) =0<br>取消下载群共享文件</p>                                                                                       |
| virtual BMXErrorCode | <p><strong>getSharedFilesList</strong>(BMXGroupPtr group, BMXGroup::SharedFileList &#x26; list, bool forceRefresh) =0<br>获取群共享文件列表</p>                                                                        |
| virtual BMXErrorCode | <p><strong>changeSharedFileName</strong>(BMXGroupPtr group, BMXGroup::SharedFilePtr sharedFile, const std::string &#x26; name) =0<br>修改群共享文件名称</p>                                                            |
| virtual BMXErrorCode | <p><strong>getLatestAnnouncement</strong>(BMXGroupPtr group, BMXGroup::AnnouncementPtr &#x26; announcement, bool forceRefresh) =0<br>获取最新的群公告</p>                                                             |
| virtual BMXErrorCode | <p><strong>getAnnouncementList</strong>(BMXGroupPtr group, BMXGroup::AnnouncementList &#x26; list, bool forceRefresh) =0<br>获取群公告列表</p>                                                                       |
| virtual BMXErrorCode | <p><strong>editAnnouncement</strong>(BMXGroupPtr group, const std::string &#x26; title, const std::string &#x26; content) =0<br>设置群公告</p>                                                                     |
| virtual BMXErrorCode | <p><strong>deleteAnnouncement</strong>(BMXGroupPtr group, int64_t announcementId) =0<br>删除群公告</p>                                                                                                             |
| virtual BMXErrorCode | <p><strong>setName</strong>(BMXGroupPtr group, const std::string &#x26; name) =0<br>设置群名称</p>                                                                                                                 |
| virtual BMXErrorCode | <p><strong>setDescription</strong>(BMXGroupPtr group, const std::string &#x26; description) =0<br>设置群描述信息</p>                                                                                                 |
| virtual BMXErrorCode | <p><strong>setExtension</strong>(BMXGroupPtr group, const std::string &#x26; extension) =0<br>设置群扩展信息</p>                                                                                                     |
| virtual BMXErrorCode | <p><strong>setMyNickname</strong>(BMXGroupPtr group, const std::string &#x26; nickname) =0<br>设置在群里的昵称</p>                                                                                                    |
| virtual BMXErrorCode | <p><strong>setMsgPushMode</strong>(BMXGroupPtr group, BMXGroup::MsgPushMode mode) =0<br>设置群消息通知模式</p>                                                                                                         |
| virtual BMXErrorCode | <p><strong>setJoinAuthMode</strong>(BMXGroupPtr group, BMXGroup::JoinAuthMode mode) =0<br>设置入群审批模式</p>                                                                                                        |
| virtual BMXErrorCode | <p><strong>setInviteMode</strong>(BMXGroupPtr group, BMXGroup::InviteMode mode) =0<br>设置邀请模式</p>                                                                                                              |
| virtual BMXErrorCode | <p><strong>setAllowMemberModify</strong>(BMXGroupPtr group, bool enable) =0<br>设置是否允许群成员设置群信息</p>                                                                                                             |
| virtual BMXErrorCode | <p><strong>setEnableReadAck</strong>(BMXGroupPtr group, bool enable) =0<br>设置是否开启群消息已读功能</p>                                                                                                                  |
| virtual BMXErrorCode | <p><strong>setHistoryVisible</strong>(BMXGroupPtr group, bool enable) =0<br>设置群成员是否开可见群历史聊天记录</p>                                                                                                             |
| virtual BMXErrorCode | <p><strong>setAvatar</strong>(BMXGroupPtr group, const std::string &#x26; avatarPath, Callback ) =0<br>设置群头像</p>                                                                                              |
| virtual BMXErrorCode | <p><strong>downloadAvatar</strong>(BMXGroupPtr group, bool thumbnail, Callback callback) =0<br>下载群头像</p>                                                                                                      |
| virtual void         | <p><strong>addGroupListener</strong>(<a href="broken-reference">BMXGroupServiceListener</a> * listener) =0<br>添加群组变化监听者</p>                                                                                   |
| virtual void         | <p><strong>removeGroupListener</strong>(<a href="broken-reference">BMXGroupServiceListener</a> * listener) =0<br>移除群组变化监听者</p>                                                                                |

## Protected Functions

|   | Name                  |
| - | --------------------- |
|   | **BMXGroupService**() |

## Public Types Documentation

### typedef Callback

```cpp
typedef std::function<void(int percent)> floo::BMXGroupService::Callback;
```

### typedef CreateGroupOptionsPtr

```cpp
typedef std::shared_ptr<CreateGroupOptions> floo::BMXGroupService::CreateGroupOptionsPtr;
```

## Public Functions Documentation

### function \~BMXGroupService

```cpp
inline virtual ~BMXGroupService()
```

### function get

```cpp
virtual BMXErrorCode get(
    BMXGroupList & list,
    bool forceRefresh
) =0
```

获取群组列表，如果设置了forceRefresh则从服务器拉取

**Parameters**:

* **list** 群组id列表，传入空列表函数返回后从此处获取返回的群组id列表
* **forceRefresh** 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Return**: BMXErrorCode

### function search

```cpp
virtual BMXErrorCode search(
    BMXGroupList & list,
    bool forceRefresh
) =0
```

Deprecated.

**Parameters**:

* **list** 群组id列表，传入空列表函数返回后从此处获取返回的群组id列表
* **forceRefresh** 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Return**: BMXErrorCode

use get instead.

获取群组列表，如果设置了forceRefresh则从服务器拉取

### function fetchGroupsByIdList

```cpp
virtual BMXErrorCode fetchGroupsByIdList(
    const std::vector< int64_t > & groupIdList,
    BMXGroupList & list,
    bool forceRefresh
) =0
```

通过传入群组的id列表获取群组信息列表，如果设置了forceRefresh则从服务器拉取

**Parameters**:

* **groupIdList** 群组id列表
* **list** 群组详细信息列表，传入空列表函数返回后从此处获取返回的群组详细信息列表
* **forceRefresh** 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Return**: BMXErrorCode

### function search

```cpp
virtual BMXErrorCode search(
    const std::vector< int64_t > & groupIdList,
    BMXGroupList & list,
    bool forceRefresh
) =0
```

Deprecated.

**Parameters**:

* **groupIdList** 群组id列表
* **list** 群组详细信息列表，传入空列表函数返回后从此处获取返回的群组详细信息列表
* **forceRefresh** 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Return**: BMXErrorCode

use fetchGroupsByIdList instead.

获取传入群组id的群组信息列表，如果设置了forceRefresh则从服务器拉取

### function fetchGroupById

```cpp
virtual BMXErrorCode fetchGroupById(
    int64_t groupId,
    BMXGroupPtr & group,
    bool forceRefresh
) =0
```

通过群组id获取群信息，如果设置了forceRefresh则从服务器拉取

**Parameters**:

* **groupId** 要搜索的群组id
* **group** 搜索返回的群组信息，传入指向为空的shared\_ptr对象函数执行后从此获取返回结果
* **forceRefresh** 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Return**: BMXErrorCode

### function search

```cpp
virtual BMXErrorCode search(
    int64_t groupId,
    BMXGroupPtr & group,
    bool forceRefresh
) =0
```

Deprecated.

**Parameters**:

* **groupId** 要搜索的群组id
* **group** 搜索返回的群组信息，传入指向为空的shared\_ptr对象函数执行后从此获取返回结果
* **forceRefresh** 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Return**: BMXErrorCode

use fetchGroupById instead.

获取群信息，如果设置了forceRefresh则从服务器拉取

### function fetchLocalGroupsByName

```cpp
virtual BMXErrorCode fetchLocalGroupsByName(
    BMXGroupList & list,
    const std::string & name
) =0
```

通过群名称查询本地群信息，从本地数据库中通过群名称查询获取群组

**Parameters**:

* **list** 搜索结果返回的群列表信息
* **name** 查询的群名称关键字

**Return**: BMXErrorCode

### function search

```cpp
virtual BMXErrorCode search(
    BMXGroupList & list,
    const std::string & name
) =0
```

Deprecated.

**Parameters**:

* **list** 搜索结果返回的群列表信息
* **name** 查询的群名称关键字

**Return**: BMXErrorCode

use fetchLocalGroupsByName instead.

通过群名称查询本地群信息，从本地数据库中通过群名称查询获取群组

### function create

```cpp
virtual BMXErrorCode create(
    const CreateGroupOptions & options,
    BMXGroupPtr & group
) =0
```

创建群

**Parameters**:

* **options** 创建群组时传入的参数选项
* **group** 创建返回的结果，传入指向为空的shared\_ptr对象函数执行后从此获取返回结果

**Return**: BMXErrorCode

### function destroy

```cpp
virtual BMXErrorCode destroy(
    BMXGroupPtr group
) =0
```

销毁群

**Parameters**:

* **group** 要销毁的群组

**Return**: BMXErrorCode

### function join

```cpp
virtual BMXErrorCode join(
    BMXGroupPtr group,
    const std::string & message
) =0
```

加入一个群，根据群设置可能需要管理员批准

**Parameters**:

* **group** 要加入的群组
* **message** 申请入群的信息

**Return**: BMXErrorCode

### function leave

```cpp
virtual BMXErrorCode leave(
    BMXGroupPtr group
) =0
```

退出群

**Parameters**:

* **group** 要退出的群组

**Return**: BMXErrorCode

### function getInfo

```cpp
virtual BMXErrorCode getInfo(
    BMXGroupPtr group
) =0
```

获取群详情，从服务端拉取最新信息

**Parameters**:

* **group** 要获取群组最新信息的群组

**Return**: BMXErrorCode

### function getMembersNickname

```cpp
virtual BMXErrorCode getMembersNickname(
    BMXGroupPtr group,
    const std::vector< int64_t > & members,
    BMXGroup::MemberList & list
) =0
```

获取群组成员详细信息

**Parameters**:

* **group** 进行操作的群组
* **members** 要获取群组成员信息详情的群成员id
* **list** 返回的群成员详细，传入空列表在函数操作后从此处获取群成员详细信息列表

**Return**: BMXErrorCode

### function getInvitationList

```cpp
virtual BMXErrorCode getInvitationList(
    BMXGroupInvitationPagePtr & result,
    const std::string & cursor ="",
    int pageSize =10
) =0
```

分页获取群组邀请列表

**Parameters**:

* **result** 分页获取的群组邀请列表，传入指向为空的shared\_ptr对象函数执行后从此处获取结果
* **cursor** 分页获取的起始cursor，第一次传入为空，后续传入上次操作返回的result中的cursor
* **pageSize** 分页大小

**Return**: BMXErrorCode

### function getApplicationList

```cpp
virtual BMXErrorCode getApplicationList(
    BMXGroupList list,
    BMXGroupApplicationPagePtr & result,
    const std::string & cursor ="",
    int pageSize =10
) =0
```

分页获取群组申请列表

**Parameters**:

* **list** 需要获取群组申请列表信息的群组id列表
* **result** 分页获取的群组申请列表，传入指向为空的shared\_ptr对象函数执行后从此处获取结果
* **cursor** 分页获取的起始cursor，第一次传入为空，后续传入上次操作返回的result中的cursor
* **pageSize** 分页大小

**Return**: BMXErrorCode

### function getMembers

```cpp
virtual BMXErrorCode getMembers(
    BMXGroupPtr group,
    BMXGroupMemberResultPagePtr & result,
    const std::string & cursor ="",
    int pageSize =200
) =0
```

分页获取群成员列表，如果设置了forceRefresh则从服务器拉取，单页最大数量为500.

**Parameters**:

* **group** 进行操作的群组
* **result** 分页获取的群成员列表，传入指向为空的shared\_ptr对象函数执行后从此处获取结果
* **cursor** 分页获取的起始cursor，第一次传入为空，后续传入上次操作返回的result中的cursor
* **pageSize** 分页大小

**Return**: BMXErrorCode

### function getMembers

```cpp
virtual BMXErrorCode getMembers(
    BMXGroupPtr group,
    BMXGroup::MemberList & list,
    bool forceRefresh
) =0
```

获取群成员列表，如果设置了forceRefresh则从服务器拉取，最多拉取1000人

**Parameters**:

* **group** 进行操作的群组
* **list** 群成员列表，传入空列表函数返回后从此处获取返回的群组详细信息列表
* **forceRefresh** 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Return**: BMXErrorCode

### function addMembers

```cpp
virtual BMXErrorCode addMembers(
    BMXGroupPtr group,
    const std::vector< int64_t > & members,
    const std::string & message
) =0
```

添加群成员

**Parameters**:

* **group** 进行操作的群组
* **members** 要添加进群的成员id列表
* **message** 添加成员原因信息

**Return**: BMXErrorCode

### function removeMembers

```cpp
virtual BMXErrorCode removeMembers(
    BMXGroupPtr group,
    const std::vector< int64_t > & members,
    const std::string & reason
) =0
```

删除群成员

**Parameters**:

* **group** 进行操作的群组
* **members** 要删除的群组成员id列表
* **reason** 删除的原因

**Return**: BMXErrorCode

### function addAdmins

```cpp
virtual BMXErrorCode addAdmins(
    BMXGroupPtr group,
    const std::vector< int64_t > & admins,
    const std::string & message
) =0
```

添加管理员

**Parameters**:

* **group** 进行操作的群组
* **admins** 要添加为管理员的成员id列表
* **message** 添加为管理员的原因

**Return**: BMXErrorCode

### function removeAdmins

```cpp
virtual BMXErrorCode removeAdmins(
    BMXGroupPtr group,
    const std::vector< int64_t > & admins,
    const std::string & reason
) =0
```

删除管理员

**Parameters**:

* **group** 进行操作的群组
* **admins** 要从管理员移除的成员id列表
* **reason** 要移除管理员的原因

**Return**: BMXErrorCode

### function getAdmins

```cpp
virtual BMXErrorCode getAdmins(
    BMXGroupPtr group,
    BMXGroup::MemberList & list,
    bool forceRefresh
) =0
```

获取Admins列表，如果设置了forceRefresh则从服务器拉取

**Parameters**:

* **group** 进行操作的群组
* **list** 群管理员列表，传入空列表函数返回后从此处获取返回的群组详细信息列表
* **forceRefresh** 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Return**: BMXErrorCode

### function blockMembers

```cpp
virtual BMXErrorCode blockMembers(
    BMXGroupPtr group,
    const std::vector< int64_t > & members
) =0
```

添加黑名单

**Parameters**:

* **group** 进行操作的群组
* **members** 要加入黑名单的群成员id列表

**Return**: BMXErrorCode

### function unblockMembers

```cpp
virtual BMXErrorCode unblockMembers(
    BMXGroupPtr group,
    const std::vector< int64_t > & members
) =0
```

从黑名单删除

**Parameters**:

* **group** 进行操作的群组
* **members** 从黑名单移除的用户id列表

**Return**: BMXErrorCode

### function getBlockList

```cpp
virtual BMXErrorCode getBlockList(
    BMXGroupPtr group,
    BMXGroupMemberResultPagePtr & result,
    const std::string & cursor ="",
    int pageSize =200
) =0
```

分页获取黑名单

**Parameters**:

* **group** 进行操作的群组
* **result** 分页获取的黑名单列表，传入指向为空的shared\_ptr对象函数执行后从此处获取结果
* **cursor** 分页获取的起始cursor，第一次传入为空，后续传入上次操作返回的result中的cursor
* **pageSize** 分页大小

**Return**: BMXErrorCode

### function getBlockList

```cpp
virtual BMXErrorCode getBlockList(
    BMXGroupPtr group,
    BMXGroup::MemberList & list,
    bool forceRefresh
) =0
```

获取黑名单

**Parameters**:

* **group** 进行操作的群组
* **list** 群黑名单列表，传入空列表函数返回后从此处获取返回的群组详细信息列表
* **forceRefresh** 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Return**: BMXErrorCode

### function banMembers

```cpp
virtual BMXErrorCode banMembers(
    BMXGroupPtr group,
    const std::vector< int64_t > & members,
    int64_t duration,
    const std::string & reason =""
) =0
```

禁言

**Parameters**:

* **group** 进行操作的群组
* **members** 被禁言的群成员id列表
* **duration** 禁言时长
* **reason** 禁言原因

**Return**: BMXErrorCode

### function banGroup

```cpp
virtual BMXErrorCode banGroup(
    BMXGroupPtr group,
    int64_t duration
) =0
```

全员禁言，当前服务器时间加上禁言时长后计算出全员禁言到期时间（只有管理和群主可以发言）

**Parameters**:

* **group** 进行操作的群组
* **duration** 禁言时长(分钟)

**Return**: BMXErrorCode

### function unbanMembers

```cpp
virtual BMXErrorCode unbanMembers(
    BMXGroupPtr group,
    const std::vector< int64_t > & members
) =0
```

解除禁言

**Parameters**:

* **group** 进行操作的群组
* **members** 被解除禁言的群成员id列表

**Return**: BMXErrorCode

### function unbanGroup

```cpp
virtual BMXErrorCode unbanGroup(
    BMXGroupPtr group
) =0
```

全员解除禁言

**Parameters**:

* **group** 进行操作的群组

**Return**: BMXErrorCode

### function getBannedMembers

```cpp
virtual BMXErrorCode getBannedMembers(
    BMXGroupPtr group,
    BMXGroupBannedMemberResultPagePtr & result,
    const std::string & cursor ="",
    int pageSize =200
) =0
```

分页获取禁言列表

**Parameters**:

* **group** 进行操作的群组
* **result** 分页获取的禁言列表，传入指向为空的shared\_ptr对象函数执行后从此处获取结果
* **cursor** 分页获取的起始cursor，第一次传入为空，后续传入上次操作返回的result中的cursor
* **pageSize** 分页大小

**Return**: BMXErrorCode

### function getBannedMembers

```cpp
virtual BMXErrorCode getBannedMembers(
    BMXGroupPtr group,
    BMXGroup::BannedMemberList & list
) =0
```

获取禁言列表

**Parameters**:

* **group** 进行操作的群组
* **list** 群禁言列表，传入空列表函数返回后从此处获取返回的群组详细信息列表

**Return**: BMXErrorCode

### function muteMessage

```cpp
virtual BMXErrorCode muteMessage(
    BMXGroupPtr group,
    BMXGroup::MsgMuteMode mode
) =0
```

设置是否屏蔽群消息

**Parameters**:

* **group** 进行操作的群组
* **mode** 群屏蔽的模式

**Return**: BMXErrorCode

### function acceptApplication

```cpp
virtual BMXErrorCode acceptApplication(
    BMXGroupPtr group,
    int64_t applicantId
) =0
```

接受入群申请

**Parameters**:

* **group** 进行操作的群组
* **applicantId** 申请进群的用户id

**Return**: BMXErrorCode

### function declineApplication

```cpp
virtual BMXErrorCode declineApplication(
    BMXGroupPtr group,
    int64_t applicantId,
    const std::string & reason =""
) =0
```

拒绝入群申请

**Parameters**:

* **group** 进行操作的群组
* **applicantId** 申请进群的用户id
* **reason** 拒绝的原因

**Return**: BMXErrorCode

### function acceptInvitation

```cpp
virtual BMXErrorCode acceptInvitation(
    BMXGroupPtr group,
    int64_t inviter
) =0
```

接受入群邀请

**Parameters**:

* **group** 进行操作的群组
* **inviter** 邀请者id

**Return**: BMXErrorCode

### function declineInvitation

```cpp
virtual BMXErrorCode declineInvitation(
    BMXGroupPtr group,
    int64_t inviter,
    const std::string & reason =""
) =0
```

拒绝入群邀请

**Parameters**:

* **group** 进行操作的群组
* **inviter** 邀请者id
* **reason** 拒绝的原因

**Return**: BMXErrorCode

### function transferOwner

```cpp
virtual BMXErrorCode transferOwner(
    BMXGroupPtr group,
    int64_t newOwnerId
) =0
```

转移群主

**Parameters**:

* **group** 进行操作的群组
* **newOwnerId** 转让为新群主的用户id

**Return**: BMXErrorCode

### function uploadSharedFile

```cpp
virtual BMXErrorCode uploadSharedFile(
    BMXGroupPtr group,
    const std::string & filePath,
    const std::string & displayName,
    const std::string & extensionName,
    Callback 
) =0
```

添加群共享文件

**Parameters**:

* **group** 进行操作的群组
* **filePath** 文件的本地路径
* **displayName** 文件的展示名
* **extensionName** 文件的扩展名
* **Callback** 上传回调函数

**Return**: BMXErrorCode

### function cancelUploadSharedFile

```cpp
virtual BMXErrorCode cancelUploadSharedFile(
    BMXGroupPtr group,
    const std::string & filePath
) =0
```

取消上传群共享文件

**Parameters**:

* **group** 进行操作的群组
* **filePath** 文件的本地路径

**Return**: BMXErrorCode

### function removeSharedFile

```cpp
virtual BMXErrorCode removeSharedFile(
    BMXGroupPtr group,
    BMXGroup::SharedFilePtr sharedFile
) =0
```

移除群共享文件

**Parameters**:

* **group** 进行操作的群组
* **sharedFile** 删除的群共享文件

**Return**: BMXErrorCode

### function downloadSharedFile

```cpp
virtual BMXErrorCode downloadSharedFile(
    BMXGroupPtr group,
    BMXGroup::SharedFilePtr sharedFile,
    Callback 
) =0
```

下载群共享文件

**Parameters**:

* **group** 进行操作的群组
* **sharedFile** 下载的群共享文件
* **Callback** 下载回调函数

**Return**: BMXErrorCode

### function cancelDownloadSharedFile

```cpp
virtual BMXErrorCode cancelDownloadSharedFile(
    BMXGroupPtr group,
    BMXGroup::SharedFilePtr sharedFile
) =0
```

取消下载群共享文件

**Parameters**:

* **group** 进行操作的群组
* **sharedFile** 下载的群共享文件

**Return**: BMXErrorCode

### function getSharedFilesList

```cpp
virtual BMXErrorCode getSharedFilesList(
    BMXGroupPtr group,
    BMXGroup::SharedFileList & list,
    bool forceRefresh
) =0
```

获取群共享文件列表

**Parameters**:

* **group** 进行操作的群组
* **list** 群共享文件列表，传入空列表函数返回后从此处获取返回的群组详细信息列表
* **forceRefresh** 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Return**: BMXErrorCode

### function changeSharedFileName

```cpp
virtual BMXErrorCode changeSharedFileName(
    BMXGroupPtr group,
    BMXGroup::SharedFilePtr sharedFile,
    const std::string & name
) =0
```

修改群共享文件名称

**Parameters**:

* **group** 进行操作的群组
* **sharedFile** 进行更改的群共享文件
* **name** 修改的群共享文件名称

**Return**: BMXErrorCode

### function getLatestAnnouncement

```cpp
virtual BMXErrorCode getLatestAnnouncement(
    BMXGroupPtr group,
    BMXGroup::AnnouncementPtr & announcement,
    bool forceRefresh
) =0
```

获取最新的群公告

**Parameters**:

* **group** 进行操作的群组
* **announcement** 最新的群组公告，传入指向为空的shared\_ptr对象函数返回后从此处获取最新的群组公告
* **forceRefresh** 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Return**: BMXErrorCode

### function getAnnouncementList

```cpp
virtual BMXErrorCode getAnnouncementList(
    BMXGroupPtr group,
    BMXGroup::AnnouncementList & list,
    bool forceRefresh
) =0
```

获取群公告列表

**Parameters**:

* **group** 进行操作的群组
* **list** 群公告列表，传入空列表函数返回后从此处获取返回的群组详细信息列表
* **forceRefresh** 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Return**: BMXErrorCode

### function editAnnouncement

```cpp
virtual BMXErrorCode editAnnouncement(
    BMXGroupPtr group,
    const std::string & title,
    const std::string & content
) =0
```

设置群公告

**Parameters**:

* **group** 进行操作的群组
* **title** 群公告的标题
* **content** 群公告的内容

**Return**: BMXErrorCode

### function deleteAnnouncement

```cpp
virtual BMXErrorCode deleteAnnouncement(
    BMXGroupPtr group,
    int64_t announcementId
) =0
```

删除群公告

**Parameters**:

* **group** 进行操作的群组
* **announcementId** 删除的群公告id

**Return**: BMXErrorCode

### function setName

```cpp
virtual BMXErrorCode setName(
    BMXGroupPtr group,
    const std::string & name
) =0
```

设置群名称

**Parameters**:

* **group** 进行操作的群组
* **name** 群组名称

**Return**: BMXErrorCode

### function setDescription

```cpp
virtual BMXErrorCode setDescription(
    BMXGroupPtr group,
    const std::string & description
) =0
```

设置群描述信息

**Parameters**:

* **group** 进行操作的群组
* **description** 群组描述

**Return**: BMXErrorCode

### function setExtension

```cpp
virtual BMXErrorCode setExtension(
    BMXGroupPtr group,
    const std::string & extension
) =0
```

设置群扩展信息

**Parameters**:

* **group** 进行操作的群组
* **extension** 群组的扩展信息

**Return**: BMXErrorCode

### function setMyNickname

```cpp
virtual BMXErrorCode setMyNickname(
    BMXGroupPtr group,
    const std::string & nickname
) =0
```

设置在群里的昵称

**Parameters**:

* **group** 进行操作的群组
* **nickname** 用户在群组内的昵称

**Return**: BMXErrorCode

### function setMsgPushMode

```cpp
virtual BMXErrorCode setMsgPushMode(
    BMXGroupPtr group,
    BMXGroup::MsgPushMode mode
) =0
```

设置群消息通知模式

**Parameters**:

* **group** 进行操作的群组
* **mode** 群消息通知模式

**Return**: BMXErrorCode

### function setJoinAuthMode

```cpp
virtual BMXErrorCode setJoinAuthMode(
    BMXGroupPtr group,
    BMXGroup::JoinAuthMode mode
) =0
```

设置入群审批模式

**Parameters**:

* **group** 进行操作的群组
* **mode** 入群审批模式

**Return**: BMXErrorCode

### function setInviteMode

```cpp
virtual BMXErrorCode setInviteMode(
    BMXGroupPtr group,
    BMXGroup::InviteMode mode
) =0
```

设置邀请模式

**Parameters**:

* **group** 进行操作的群组
* **mode** 群组的邀请模式

**Return**: BMXErrorCode

### function setAllowMemberModify

```cpp
virtual BMXErrorCode setAllowMemberModify(
    BMXGroupPtr group,
    bool enable
) =0
```

设置是否允许群成员设置群信息

**Parameters**:

* **group** 进行操作的群组
* **enable** 是否允许操作

**Return**: BMXErrorCode

### function setEnableReadAck

```cpp
virtual BMXErrorCode setEnableReadAck(
    BMXGroupPtr group,
    bool enable
) =0
```

设置是否开启群消息已读功能

**Parameters**:

* **group** 进行操作的群组
* **enable** 是否开启

**Return**: BMXErrorCode

### function setHistoryVisible

```cpp
virtual BMXErrorCode setHistoryVisible(
    BMXGroupPtr group,
    bool enable
) =0
```

设置群成员是否开可见群历史聊天记录

**Parameters**:

* **group** 进行操作的群组
* **enable** 是否开启

**Return**: BMXErrorCode

### function setAvatar

```cpp
virtual BMXErrorCode setAvatar(
    BMXGroupPtr group,
    const std::string & avatarPath,
    Callback 
) =0
```

设置群头像

**Parameters**:

* **group** 进行操作的群组
* **avatarPath** 群头像文件的本地路径
* **Callback** 上传回调函数

**Return**: BMXErrorCode

### function downloadAvatar

```cpp
virtual BMXErrorCode downloadAvatar(
    BMXGroupPtr group,
    bool thumbnail,
    Callback callback
) =0
```

下载群头像

**Parameters**:

* **group** 进行操作的群组
* **thumbnail** 设置为true下载缩略图，false下载原图
* **callback** 下载回调函数

**Return**: BMXErrorCode

### function addGroupListener

```cpp
virtual void addGroupListener(
    BMXGroupServiceListener * listener
) =0
```

添加群组变化监听者

**Parameters**:

* **listener** 群组变化监听者

### function removeGroupListener

```cpp
virtual void removeGroupListener(
    BMXGroupServiceListener * listener
) =0
```

移除群组变化监听者

**Parameters**:

* **listener** 群组变化监听者

## Protected Functions Documentation

### function BMXGroupService

```cpp
inline BMXGroupService()
```

***

Updated on 2022-01-26 at 17:20:40 +0800
