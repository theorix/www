# floo android

## namespace `floolib`

### Summary

| Members                                                       | Descriptions |
| ------------------------------------------------------------- | ------------ |
| `class` [`BMXRosterItem`](broken-reference)                   | 联系人          |
| `class` [`BMXUserProfile`](broken-reference)                  | 用户Profile    |
| `class` [`BMXGroup`](broken-reference)                        | 群组           |
| `class` [`BMXRosterService`](broken-reference)                | 好友Service    |
| `class` [`ApplicationPage`](broken-reference)                 |              |
| `class` [`BMXMessageConfig`](broken-reference)                | 消息配置         |
| `class` [`BMXBaseObject`](broken-reference)                   |              |
| `class` [`BMXChatManager`](broken-reference)                  | 聊天管理器        |
| `class` [`BMXChatService`](broken-reference)                  | 聊天Service    |
| `class` [`BMXChatServiceListener`](broken-reference)          | 聊天监听者        |
| `class` [`BMXClient`](broken-reference)                       | 客户端          |
| `class` [`BMXConversation`](broken-reference)                 | 会话           |
| `class` [`BMXConversationList`](broken-reference)             |              |
| `class` [`BMXDevice`](broken-reference)                       | 设备信息         |
| `class` [`BMXDeviceList`](broken-reference)                   |              |
| `class` [`BMXError`](broken-reference)                        |              |
| `class` [`BMXFileAttachment`](broken-reference)               | 消息文件附件       |
| `class` [`BMXGroupAnnouncementList`](broken-reference)        |              |
| `class` [`BMXGroupApplicationList`](broken-reference)         |              |
| `class` [`BMXGroupBannedMemberList`](broken-reference)        |              |
| `class` [`BMXGroupBannedMemberResultPage`](broken-reference)  |              |
| `class` [`BMXGroupInvitationList`](broken-reference)          |              |
| `class` [`BMXGroupList`](broken-reference)                    |              |
| `class` [`BMXGroupManager`](broken-reference)                 | 群组管理器        |
| `class` [`BMXGroupMemberList`](broken-reference)              |              |
| `class` [`BMXGroupMemberResultPage`](broken-reference)        |              |
| `class` [`BMXGroupService`](broken-reference)                 | 群组Service    |
| `class` [`BMXGroupServiceListener`](broken-reference)         | 群组变化监听者      |
| `class` [`BMXGroupSharedFileList`](broken-reference)          |              |
| `class` [`BMXHttpClient`](broken-reference)                   |              |
| `class` [`BMXImageAttachment`](broken-reference)              | 图片消息附件       |
| `class` [`BMXLocationAttachment`](broken-reference)           | 位置消息附件       |
| `class` [`BMXMessage`](broken-reference)                      | 消息           |
| `class` [`BMXMessageAttachment`](broken-reference)            | 消息附件         |
| `class` [`BMXMessageList`](broken-reference)                  |              |
| `class` [`BMXMessageListList`](broken-reference)              |              |
| `class` [`BMXMessagePage`](broken-reference)                  |              |
| `class` [`BMXNetworkListener`](broken-reference)              | 网络监听者        |
| `class` [`BMXPushManager`](broken-reference)                  | 推送管理器        |
| `class` [`BMXPushService`](broken-reference)                  |              |
| `class` [`BMXPushServiceListener`](broken-reference)          |              |
| `class` [`BMXPushUserProfile`](broken-reference)              |              |
| `class` [`BMXRosterItemList`](broken-reference)               |              |
| `class` [`BMXRosterManager`](broken-reference)                | 好友管理器        |
| `class` [`BMXRosterServiceApplicationList`](broken-reference) |              |
| `class` [`BMXRosterServiceListener`](broken-reference)        | 好友变化监听者      |
| `class` [`BMXSDKConfig`](broken-reference)                    | SDK设置管理      |
| `class` [`BMXUserManager`](broken-reference)                  | 用户管理器        |
| `class` [`BMXUserService`](broken-reference)                  | 用户Service    |
| `class` [`BMXUserServiceListener`](broken-reference)          | 用户状态监听者      |
| `class` [`BMXVideoAttachment`](broken-reference)              | 视频消息附件       |
| `class` [`BMXVoiceAttachment`](broken-reference)              | 音频消息附件       |
| `class` [`floo`](broken-reference)                            |              |
| `class` [`flooJNI`](broken-reference)                         |              |
| `class` [`GroupApplicationPage`](broken-reference)            |              |
| `class` [`GroupInvitaionPage`](broken-reference)              |              |
| `class` [`ListOfLongLong`](broken-reference)                  |              |
| `class` [`TagList`](broken-reference)                         |              |
| `class` [`UserProfileImpl`](broken-reference)                 |              |

## class `BMXRosterItem` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item"></a>

```
class BMXRosterItem
  : public im.floo.floolib.BMXBaseObject
```

联系人

### Summary

| Members                                                             | Descriptions                   |
| ------------------------------------------------------------------- | ------------------------------ |
| `public transient long swigCPtr`                                    |                                |
| `public inline BMXRosterItem()`                                     |                                |
| `public inline synchronized void delete()`                          |                                |
| `public inline long rosterId()`                                     | 好友Id                           |
| `public inline String username()`                                   | 好友名                            |
| `public inline String nickname()`                                   | 好友昵称                           |
| `public inline String avatarRatelUrl()`                             | 好友头像ratel服务器地址                 |
| `public inline String avatarUrl()`                                  | 好友头像服务器地址                      |
| `public inline String avatarPath()`                                 | 好友头像本地存储路径                     |
| `public inline String avatarThumbnailUrl()`                         | 好友头像缩略图地址                      |
| `public inline String avatarThumbnailPath()`                        | 好友头像缩略图本地存储路径                  |
| `public inline String publicInfo()`                                 | 扩展信息，用户设置的好友可以看到的信息，比如地址，个性签名等 |
| `public inline String alias()`                                      | 用户对好友添加的备注等信息                  |
| `public inline String ext()`                                        | 用户的服务器扩展信息                     |
| `public inline String localExt()`                                   | 用户的本地扩展信息                      |
| `public inline BMXRosterItem.RosterRelation relation()`             | 联系人关系                          |
| `public inline boolean isMuteNotification()`                        | 是否提醒用户消息                       |
| `public inline BMXRosterItem.AddFriendAuthMode addFriendAuthMode()` | roster的好友添加验证方式。               |
| `public inline String authQuestion()`                               | roster的好友验证问题。                 |
| `protected inline BMXRosterItem(long cPtr,boolean cMemoryOwn)`      |                                |
| `protected inline void finalize()`                                  |                                |

### Members

#### `public transient long swigCPtr` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a1995e77fcbf0a71b6d2daef912306cac" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a1995e77fcbf0a71b6d2daef912306cac"></a>

#### `public inline BMXRosterItem()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1ab9a46437f3636f72aea724dfce8f4470" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1ab9a46437f3636f72aea724dfce8f4470"></a>

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1aa7cd4df8f23c3df823ad3e71e0fc5eb6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1aa7cd4df8f23c3df823ad3e71e0fc5eb6"></a>

#### `public inline long rosterId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1ad1eabb0fab2c39ea6cc33e5d59077097" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1ad1eabb0fab2c39ea6cc33e5d59077097"></a>

好友Id

**Returns**

int64\_t

#### `public inline String username()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a579ac0b7ca6a6379d9efa7f8804b6e18" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a579ac0b7ca6a6379d9efa7f8804b6e18"></a>

好友名

**Returns**

std::string

#### `public inline String nickname()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1ac55016a98408846516080738881fb630" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1ac55016a98408846516080738881fb630"></a>

好友昵称

**Returns**

std::string

#### `public inline String avatarRatelUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a650e37c3fa14b09ec0ad7ff05f172a71" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a650e37c3fa14b09ec0ad7ff05f172a71"></a>

好友头像ratel服务器地址

**Returns**

std::string

#### `public inline String avatarUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a0caa3586d0578cc78081936909207f79" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a0caa3586d0578cc78081936909207f79"></a>

好友头像服务器地址

**Returns**

std::string

#### `public inline String avatarPath()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a540f08d4a84796c7c443e81822b3bea2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a540f08d4a84796c7c443e81822b3bea2"></a>

好友头像本地存储路径

**Returns**

std::string

#### `public inline String avatarThumbnailUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a72969c1b447228a6008e80f565f9cb05" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a72969c1b447228a6008e80f565f9cb05"></a>

好友头像缩略图地址

**Returns**

std::string

#### `public inline String avatarThumbnailPath()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a8a26e70c5dfa2c6ca58a5890c3b6764d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a8a26e70c5dfa2c6ca58a5890c3b6764d"></a>

好友头像缩略图本地存储路径

**Returns**

std::string

#### `public inline String publicInfo()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a65c146c78dc380da4388f79b94f34668" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a65c146c78dc380da4388f79b94f34668"></a>

扩展信息，用户设置的好友可以看到的信息，比如地址，个性签名等

**Returns**

JSON(std::string)

#### `public inline String alias()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a02109cec19340180318a65c96808a32a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a02109cec19340180318a65c96808a32a"></a>

用户对好友添加的备注等信息

**Returns**

JSON(std::string)

#### `public inline String ext()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a45572bbd9f2bc120e1325c3d4df03cb7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a45572bbd9f2bc120e1325c3d4df03cb7"></a>

用户的服务器扩展信息

**Returns**

JSON(std::string)

#### `public inline String localExt()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a8a6e26b777aa1d985e757428217135f0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a8a6e26b777aa1d985e757428217135f0"></a>

用户的本地扩展信息

**Returns**

JSON(std::string)

#### `public inline BMXRosterItem.RosterRelation relation()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a0482926e7f0a30b9e6fa09bf10ab679e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a0482926e7f0a30b9e6fa09bf10ab679e"></a>

联系人关系

**Returns**

[RosterRelation](broken-reference)

#### `public inline boolean isMuteNotification()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a0a61fa67bc0f9e002d0e172983616892" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a0a61fa67bc0f9e002d0e172983616892"></a>

是否提醒用户消息

**Returns**

bool

#### `public inline BMXRosterItem.AddFriendAuthMode addFriendAuthMode()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a68bf59c25387e654bb79fa36c94245bc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a68bf59c25387e654bb79fa36c94245bc"></a>

roster的好友添加验证方式。

**Returns**

[AddFriendAuthMode](broken-reference)

#### `public inline String authQuestion()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1ac6e5d5038ac65a096115e42b8483d6c1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1ac6e5d5038ac65a096115e42b8483d6c1"></a>

roster的好友验证问题。

**Returns**

std::string

#### `protected inline BMXRosterItem(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a41f002bb3de504e5d2d8158a98dfb6b4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a41f002bb3de504e5d2d8158a98dfb6b4"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a5baa1eff1f22a0c50dbe697f815fb812" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_1a5baa1eff1f22a0c50dbe697f815fb812"></a>

## class `BMXUserProfile` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile"></a>

```
class BMXUserProfile
  : public im.floo.floolib.BMXBaseObject
```

用户Profile

### Summary

| Members                                                              | Descriptions      |
| -------------------------------------------------------------------- | ----------------- |
| `class` [`AuthQuestion`](broken-reference)                           | 添加好友时的校验问题        |
| `class` [`MessageSetting`](broken-reference)                         | 用户消息设置            |
| `public transient long swigCPtr`                                     |                   |
| `public inline BMXUserProfile()`                                     |                   |
| `public inline synchronized void delete()`                           |                   |
| `public inline long userId()`                                        | 用户ID（唯一）          |
| `public inline BMXUserProfile.UserCategory category()`               | 用户策略              |
| `public inline String username()`                                    | 用户名（唯一）           |
| `public inline String nickname()`                                    | 用户昵称              |
| `public inline String avatarRatelUrl()`                              | 用户头像ratel服务器地址    |
| `public inline String avatarUrl()`                                   | 用户头像              |
| `public inline String avatarPath()`                                  | 用户头像本地存储路径        |
| `public inline String avatarThumbnailPath()`                         | 用户头像缩略图本地存储路径     |
| `public inline String mobilePhone()`                                 | 用户手机              |
| `public inline String email()`                                       | 用户邮箱              |
| `public inline String publicInfo()`                                  | 用户公开扩展信息，好友可见     |
| `public inline String privateInfo()`                                 | 用户私有扩展信息，好友不可见    |
| `public inline BMXUserProfile.AddFriendAuthMode addFriendAuthMode()` | 加好友校验方式           |
| `public inline BMXUserProfile.AuthQuestion authQuestion()`           | 添加好友时的验证问题        |
| `public inline BMXUserProfile.MessageSetting messageSetting()`       | 用户消息设定            |
| `public inline boolean isAutoAcceptGroupInvite()`                    | 收到群组邀请进群时是否自动同意进群 |
| `protected inline BMXUserProfile(long cPtr,boolean cMemoryOwn)`      |                   |
| `protected inline void finalize()`                                   |                   |

### Members

#### `class` [`AuthQuestion`](broken-reference) <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question"></a>

添加好友时的校验问题

#### `class` [`MessageSetting`](broken-reference) <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting"></a>

用户消息设置

#### `public transient long swigCPtr` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1ada21d0ba2d54fd6cce99efe46b79d26c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1ada21d0ba2d54fd6cce99efe46b79d26c"></a>

#### `public inline BMXUserProfile()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a2d60812fb28b7076a3594d281d0c6c06" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a2d60812fb28b7076a3594d281d0c6c06"></a>

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1afa51ea2f7512055cf05cda4ea19309cd" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1afa51ea2f7512055cf05cda4ea19309cd"></a>

#### `public inline long userId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a8dd07e8a552c0d2b7a2ec8bc19406506" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a8dd07e8a552c0d2b7a2ec8bc19406506"></a>

用户ID（唯一）

**Returns**

int64\_t

#### `public inline BMXUserProfile.UserCategory category()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1adb406c55c1f8192c0bcac27ca034f059" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1adb406c55c1f8192c0bcac27ca034f059"></a>

用户策略

**Returns**

[UserCategory](broken-reference)

#### `public inline String username()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1ab27eeb733819add393b8432dd2a5efcb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1ab27eeb733819add393b8432dd2a5efcb"></a>

用户名（唯一）

**Returns**

std::string

#### `public inline String nickname()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1ac72a4b5043d0e110701de7115be1105f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1ac72a4b5043d0e110701de7115be1105f"></a>

用户昵称

**Returns**

std::string

#### `public inline String avatarRatelUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1ac881f28a0ab5eca5e2ea3a8f555ae963" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1ac881f28a0ab5eca5e2ea3a8f555ae963"></a>

用户头像ratel服务器地址

**Returns**

std::string

#### `public inline String avatarUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a7f1511dbe781cb1c0ce6117c6eb73029" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a7f1511dbe781cb1c0ce6117c6eb73029"></a>

用户头像

**Returns**

std::string

#### `public inline String avatarPath()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1ae0c57a95c96ea802394a8ab4dc9d9561" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1ae0c57a95c96ea802394a8ab4dc9d9561"></a>

用户头像本地存储路径

**Returns**

std::string

#### `public inline String avatarThumbnailPath()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a710b06c5723932686af56e83abd140c1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a710b06c5723932686af56e83abd140c1"></a>

用户头像缩略图本地存储路径

**Returns**

std::string

#### `public inline String mobilePhone()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a472619e69c89a3bd83ac27c8834b77e8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a472619e69c89a3bd83ac27c8834b77e8"></a>

用户手机

**Returns**

std::string

#### `public inline String email()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a427e12ce5516cb1eebbab979a307327c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a427e12ce5516cb1eebbab979a307327c"></a>

用户邮箱

**Returns**

std::string

#### `public inline String publicInfo()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a5da2c90ac922c349c09409fbba079865" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a5da2c90ac922c349c09409fbba079865"></a>

用户公开扩展信息，好友可见

**Returns**

JSON(std::string)

#### `public inline String privateInfo()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a7fae7fbf68ab6d92a31cebcbcca47b58" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a7fae7fbf68ab6d92a31cebcbcca47b58"></a>

用户私有扩展信息，好友不可见

**Returns**

JSON(std::string)

#### `public inline BMXUserProfile.AddFriendAuthMode addFriendAuthMode()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a04e2f1440b52ea5e034301e5b66e2ac9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a04e2f1440b52ea5e034301e5b66e2ac9"></a>

加好友校验方式

**Returns**

[AddFriendAuthMode](broken-reference)

#### `public inline BMXUserProfile.AuthQuestion authQuestion()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1aa1f0cc4ea546b667d1d4b31c566406ce" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1aa1f0cc4ea546b667d1d4b31c566406ce"></a>

添加好友时的验证问题

**Returns**

AuthQuestion

#### `public inline BMXUserProfile.MessageSetting messageSetting()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1af450e73493f48faa076e18cf1e0c5a4a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1af450e73493f48faa076e18cf1e0c5a4a"></a>

用户消息设定

**Returns**

MessageSetting

#### `public inline boolean isAutoAcceptGroupInvite()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1ac4bc65fcbbdb1f0821e21133ab2c5d2d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1ac4bc65fcbbdb1f0821e21133ab2c5d2d"></a>

收到群组邀请进群时是否自动同意进群

**Returns**

bool

#### `protected inline BMXUserProfile(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a1f59eb8c911a52272726d46a91b1cf55" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1a1f59eb8c911a52272726d46a91b1cf55"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1ab378d8a43063825e2e93d523b4bbf32c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1ab378d8a43063825e2e93d523b4bbf32c"></a>

## class `AuthQuestion` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question"></a>

添加好友时的校验问题

### Summary

| Members                                                       | Descriptions |
| ------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                    |              |
| `public inline AuthQuestion()`                                |              |
| `public inline void setMQuestion(String value)`               |              |
| `public inline String getMQuestion()`                         |              |
| `public inline void setMAnswer(String value)`                 |              |
| `public inline String getMAnswer()`                           |              |
| `protected transient boolean swigCMemOwn`                     |              |
| `protected inline AuthQuestion(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                            |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1a9ebf37b15ab47edb30a50a38c22315" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1a9ebf37b15ab47edb30a50a38c22315"></a>

#### `public inline AuthQuestion()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1ad3a12189d46cbc0f2027ba76ab9d0e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1ad3a12189d46cbc0f2027ba76ab9d0e"></a>

#### `public inline void setMQuestion(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1a49dc4c15394ab70cf70df65a691af7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1a49dc4c15394ab70cf70df65a691af7"></a>

#### `public inline String getMQuestion()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1a9c025824c47ddc1f792b469216f9f2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1a9c025824c47ddc1f792b469216f9f2"></a>

#### `public inline void setMAnswer(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1a35d57ffead133066f21fea9edb8daa" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1a35d57ffead133066f21fea9edb8daa"></a>

#### `public inline String getMAnswer()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1af26aea6cf59bdf91046d7fc1b2459a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1af26aea6cf59bdf91046d7fc1b2459a"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1ad652afb9eb32ce384c2b97f3b2a881" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1ad652afb9eb32ce384c2b97f3b2a881"></a>

#### `protected inline AuthQuestion(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1aab625e4066f3f8a25921395d7b0398" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1aab625e4066f3f8a25921395d7b0398"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1a99d810cf660e343e73d2f0eb860d76" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_auth_question_1a99d810cf660e343e73d2f0eb860d76"></a>

## class `MessageSetting` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting"></a>

用户消息设置

### Summary

| Members                                                         | Descriptions |
| --------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                      |              |
| `public inline MessageSetting()`                                |              |
| `public inline void setMPushEnabled(boolean value)`             |              |
| `public inline boolean getMPushEnabled()`                       |              |
| `public inline void setMPushDetail(boolean value)`              |              |
| `public inline boolean getMPushDetail()`                        |              |
| `public inline void setMPushNickname(String value)`             |              |
| `public inline String getMPushNickname()`                       |              |
| `public inline void setMNotificationSound(boolean value)`       |              |
| `public inline boolean getMNotificationSound()`                 |              |
| `public inline void setMNotificationVibrate(boolean value)`     |              |
| `public inline boolean getMNotificationVibrate()`               |              |
| `public inline void setMAutoDownloadAttachment(boolean value)`  |              |
| `public inline boolean getMAutoDownloadAttachment()`            |              |
| `public inline void setMSilenceStartTime(int value)`            |              |
| `public inline int getMSilenceStartTime()`                      |              |
| `public inline void setMSilenceEndTime(int value)`              |              |
| `public inline int getMSilenceEndTime()`                        |              |
| `public inline void setMPushStartTime(int value)`               |              |
| `public inline int getMPushStartTime()`                         |              |
| `public inline void setMPushEndTime(int value)`                 |              |
| `public inline int getMPushEndTime()`                           |              |
| `protected transient boolean swigCMemOwn`                       |              |
| `protected inline MessageSetting(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                              |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1acfd13e873d6edbe85127610dee71" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1acfd13e873d6edbe85127610dee71"></a>

#### `public inline MessageSetting()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a9eab8dfa5761dfd743fa59cf22ae" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a9eab8dfa5761dfd743fa59cf22ae"></a>

#### `public inline void setMPushEnabled(boolean value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1ab68878b15b227fbc7eeb304a930d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1ab68878b15b227fbc7eeb304a930d"></a>

#### `public inline boolean getMPushEnabled()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1aa5789350ce44d78c56931dad0375" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1aa5789350ce44d78c56931dad0375"></a>

#### `public inline void setMPushDetail(boolean value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1afe0de61b0f50eac825a4e3980029" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1afe0de61b0f50eac825a4e3980029"></a>

#### `public inline boolean getMPushDetail()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1adbda06e0a2bb12405afb4d421f0a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1adbda06e0a2bb12405afb4d421f0a"></a>

#### `public inline void setMPushNickname(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1ac026f6e0a46fbf5bb513d0fe2c30" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1ac026f6e0a46fbf5bb513d0fe2c30"></a>

#### `public inline String getMPushNickname()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a28547673f2d5a54a30cc1f2f69c5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a28547673f2d5a54a30cc1f2f69c5"></a>

#### `public inline void setMNotificationSound(boolean value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a79906498c0df9dc777217ef9eda0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a79906498c0df9dc777217ef9eda0"></a>

#### `public inline boolean getMNotificationSound()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a60c9242650fc81c7dc419cace8c7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a60c9242650fc81c7dc419cace8c7"></a>

#### `public inline void setMNotificationVibrate(boolean value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1af943ac6a8788c39f55bea99b7f06" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1af943ac6a8788c39f55bea99b7f06"></a>

#### `public inline boolean getMNotificationVibrate()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1afdcec963c46c937f018383d8b622" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1afdcec963c46c937f018383d8b622"></a>

#### `public inline void setMAutoDownloadAttachment(boolean value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a7dd24dd74d95435a2bf228d59621" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a7dd24dd74d95435a2bf228d59621"></a>

#### `public inline boolean getMAutoDownloadAttachment()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1ab968e336bd649bbcaee920a6250d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1ab968e336bd649bbcaee920a6250d"></a>

#### `public inline void setMSilenceStartTime(int value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a695b402a8c94e2a32bae4297a4d6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a695b402a8c94e2a32bae4297a4d6"></a>

#### `public inline int getMSilenceStartTime()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1abc20ed153b03e0986c14cb23a2bb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1abc20ed153b03e0986c14cb23a2bb"></a>

#### `public inline void setMSilenceEndTime(int value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a5163f7dce005d06cdf777d030094" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a5163f7dce005d06cdf777d030094"></a>

#### `public inline int getMSilenceEndTime()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a4b35230afd5f26b972705994a278" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a4b35230afd5f26b972705994a278"></a>

#### `public inline void setMPushStartTime(int value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a4b4aa0f7d24e2911cad1a3f361bc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a4b4aa0f7d24e2911cad1a3f361bc"></a>

#### `public inline int getMPushStartTime()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a16c3132a9a031a2dd10a98deef4b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a16c3132a9a031a2dd10a98deef4b"></a>

#### `public inline void setMPushEndTime(int value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a215cfe7b9ce44dad6f83a0873039" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a215cfe7b9ce44dad6f83a0873039"></a>

#### `public inline int getMPushEndTime()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1aae33b7799b12162496d0885bc8a5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1aae33b7799b12162496d0885bc8a5"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1afeca57cc406c928175b410496c7c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1afeca57cc406c928175b410496c7c"></a>

#### `protected inline MessageSetting(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a459140143227c20e682fed0977c2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a459140143227c20e682fed0977c2"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a91e77287457f30bbe071ebd97efa" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_profile_1_1_message_setting_1a91e77287457f30bbe071ebd97efa"></a>

## class `BMXGroup` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group"></a>

```
class BMXGroup
  : public im.floo.floolib.BMXBaseObject
```

群组

### Summary

| Members                                                   | Descriptions                                     |
| --------------------------------------------------------- | ------------------------------------------------ |
| `class` [`Announcement`](broken-reference)                | 群公告                                              |
| `class` [`Application`](broken-reference)                 | 群申请                                              |
| `class` [`BannedMember`](broken-reference)                | 群禁言成员                                            |
| `class` [`Invitation`](broken-reference)                  | 群邀请                                              |
| `class` [`Member`](broken-reference)                      | 群成员                                              |
| `class` [`SharedFile`](broken-reference)                  | 群共享文件                                            |
| `public transient long swigCPtr`                          |                                                  |
| `public inline BMXGroup()`                                |                                                  |
| `public inline synchronized void delete()`                |                                                  |
| `public inline long groupId()`                            | 群Id                                              |
| `public inline BMXGroup.GroupType groupType()`            | 当前群组的群组类型（Private 私有群组，Public 公开群组，Chatroom 聊天室） |
| `public inline String myNickname()`                       | 在群里的昵称                                           |
| `public inline String name()`                             | 群名称                                              |
| `public inline String description()`                      | 群描述                                              |
| `public inline String avatarRatelUrl()`                   | 群头像ratel地址                                       |
| `public inline String avatarUrl()`                        | 群头像                                              |
| `public inline String avatarPath()`                       | 群头像下载后的本地路径                                      |
| `public inline String avatarThumbnailUrl()`               | 群头像缩略图地址                                         |
| `public inline String avatarThumbnailPath()`              | 群头像缩略图下载后的本地路径                                   |
| `public inline long createTime()`                         | 群创建时间                                            |
| `public inline String extension()`                        | 群扩展信息                                            |
| `public inline long ownerId()`                            | 群Owner                                           |
| `public inline int capacity()`                            | 最大人数                                             |
| `public inline int membersCount()`                        | 群成员数量，包含Owner，admins 和members                    |
| `public inline int adminsCount()`                         | 群管理员数量                                           |
| `public inline int blockListSize()`                       | 黑名单数量                                            |
| `public inline int bannedListSize()`                      | 禁言数量                                             |
| `public inline int sharedFilesCount()`                    | 群共享文件数量                                          |
| `public inline long latestAnnouncementId()`               | 最新群公告id                                          |
| `public inline BMXGroup.MsgPushMode msgPushMode()`        | 群消息通知类型                                          |
| `public inline BMXGroup.ModifyMode modifyMode()`          | 群信息修改模式                                          |
| `public inline BMXGroup.JoinAuthMode joinAuthMode()`      | 入群审批模式                                           |
| `public inline BMXGroup.InviteMode inviteMode()`          | 入群邀请模式                                           |
| `public inline BMXGroup.MsgMuteMode msgMuteMode()`        | 群消息屏蔽模式                                          |
| `public inline BMXGroup.GroupStatus groupStatus()`        | 当前群组的状态。（Normal 正常， Destroyed 以销毁）               |
| `public inline boolean isMember()`                        | Deprecated use roleType instead.                 |
| `public inline boolean enableReadAck()`                   | 是否开启群消息已读功能                                      |
| `public inline boolean historyVisible()`                  | 是否可以加载显示历史聊天记录                                   |
| `public inline BMXGroup.MemberRoleType roleType()`        | 成员在群组内的角色类型                                      |
| `public inline long banExpireTime()`                      | 群组全员禁言到期时间                                       |
| `protected inline BMXGroup(long cPtr,boolean cMemoryOwn)` |                                                  |
| `protected inline void finalize()`                        |                                                  |

### Members

#### `class` [`Announcement`](broken-reference) <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement"></a>

群公告

#### `class` [`Application`](broken-reference) <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application"></a>

群申请

#### `class` [`BannedMember`](broken-reference) <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member"></a>

群禁言成员

#### `class` [`Invitation`](broken-reference) <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation"></a>

群邀请

#### `class` [`Member`](broken-reference) <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member"></a>

群成员

#### `class` [`SharedFile`](broken-reference) <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file"></a>

群共享文件

#### `public transient long swigCPtr` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1af88361c454a8829420a4240f0f614ca6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1af88361c454a8829420a4240f0f614ca6"></a>

#### `public inline BMXGroup()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a910fba9c83714156087084efd433ecff" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a910fba9c83714156087084efd433ecff"></a>

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a29a1fcd5b90c3abc7a3ab880798a59b2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a29a1fcd5b90c3abc7a3ab880798a59b2"></a>

#### `public inline long groupId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a359197ba81b327e65ff7cb970c7f9f05" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a359197ba81b327e65ff7cb970c7f9f05"></a>

群Id

**Returns**

int64\_t

#### `public inline BMXGroup.GroupType groupType()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1acc3d428089144879475227e712f738e5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1acc3d428089144879475227e712f738e5"></a>

当前群组的群组类型（Private 私有群组，Public 公开群组，Chatroom 聊天室）

**Returns**

[GroupType](broken-reference)

#### `public inline String myNickname()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1ae1f60edb3b479ebb7c092a2e22be0bef" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1ae1f60edb3b479ebb7c092a2e22be0bef"></a>

在群里的昵称

**Returns**

std::string

#### `public inline String name()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1af10663967c912567e0f10ac87cf21690" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1af10663967c912567e0f10ac87cf21690"></a>

群名称

**Returns**

std::string

#### `public inline String description()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a7805a9ca0af697d8282af0e9e1ff3f9c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a7805a9ca0af697d8282af0e9e1ff3f9c"></a>

群描述

**Returns**

std::string

#### `public inline String avatarRatelUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1ae88ec67c0bff5ee3e1d8e93a2ae801db" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1ae88ec67c0bff5ee3e1d8e93a2ae801db"></a>

群头像ratel地址

**Returns**

std::string

#### `public inline String avatarUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a1200a97a4d574aaacf0f2bcf07c21580" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a1200a97a4d574aaacf0f2bcf07c21580"></a>

群头像

**Returns**

std::string

#### `public inline String avatarPath()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1aebd02d3ce45f42e0c0ff6b2d4a284b5d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1aebd02d3ce45f42e0c0ff6b2d4a284b5d"></a>

群头像下载后的本地路径

**Returns**

std::string

#### `public inline String avatarThumbnailUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a7f5d7c400c6e3650bf401c6e31f540ec" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a7f5d7c400c6e3650bf401c6e31f540ec"></a>

群头像缩略图地址

**Returns**

std::string

#### `public inline String avatarThumbnailPath()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1ab293e0d2dacffa20cb1bd4fb1d79f288" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1ab293e0d2dacffa20cb1bd4fb1d79f288"></a>

群头像缩略图下载后的本地路径

**Returns**

std::string

#### `public inline long createTime()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a661506785cce1189b2cee22b5eb6b643" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a661506785cce1189b2cee22b5eb6b643"></a>

群创建时间

**Returns**

int64\_t

#### `public inline String extension()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a6b70ec26da3e620aa0cfcb38b1b0ba0b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a6b70ec26da3e620aa0cfcb38b1b0ba0b"></a>

群扩展信息

**Returns**

JSON(std::string)

#### `public inline long ownerId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a239a85a69c0fe050c930683642ad1bcf" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a239a85a69c0fe050c930683642ad1bcf"></a>

群Owner

**Returns**

int64\_t

#### `public inline int capacity()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a8b7859237f08ec78ddc3f1f07ef6649f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a8b7859237f08ec78ddc3f1f07ef6649f"></a>

最大人数

**Returns**

int

#### `public inline int membersCount()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a93a5efbcb46b2e676ec96fa754351fd3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a93a5efbcb46b2e676ec96fa754351fd3"></a>

群成员数量，包含Owner，admins 和members

**Returns**

int

#### `public inline int adminsCount()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1ad389bd7ffea4674128428b61253b012b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1ad389bd7ffea4674128428b61253b012b"></a>

群管理员数量

**Returns**

int

#### `public inline int blockListSize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1aa08859cc840e4070ba71d375064b1635" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1aa08859cc840e4070ba71d375064b1635"></a>

黑名单数量

**Returns**

int

#### `public inline int bannedListSize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1abeba25c489c29054a1fba1b8c9793f8b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1abeba25c489c29054a1fba1b8c9793f8b"></a>

禁言数量

**Returns**

int

#### `public inline int sharedFilesCount()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1aee7fef30bb6f044109ae3996eb6c0c62" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1aee7fef30bb6f044109ae3996eb6c0c62"></a>

群共享文件数量

**Returns**

int

#### `public inline long latestAnnouncementId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1af722eaca18015a009b8f6fe51c8b2e56" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1af722eaca18015a009b8f6fe51c8b2e56"></a>

最新群公告id

**Returns**

int64\_t

#### `public inline BMXGroup.MsgPushMode msgPushMode()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a29840a321abbe2a90fdeab15456c4fb7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a29840a321abbe2a90fdeab15456c4fb7"></a>

群消息通知类型

**Returns**

[MsgPushMode](broken-reference)

#### `public inline BMXGroup.ModifyMode modifyMode()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a96bc96dfaf71a8a8861f5df4bba348ad" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a96bc96dfaf71a8a8861f5df4bba348ad"></a>

群信息修改模式

**Returns**

[ModifyMode](broken-reference)

#### `public inline BMXGroup.JoinAuthMode joinAuthMode()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1ae403ea31fbe47524f9efa59e202e982b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1ae403ea31fbe47524f9efa59e202e982b"></a>

入群审批模式

**Returns**

[JoinAuthMode](broken-reference)

#### `public inline BMXGroup.InviteMode inviteMode()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a66e7dba7802fe140099bc3a79d67b2fb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a66e7dba7802fe140099bc3a79d67b2fb"></a>

入群邀请模式

**Returns**

[InviteMode](broken-reference)

#### `public inline BMXGroup.MsgMuteMode msgMuteMode()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a4dbc610cf417ee6e53fad2b1a8a2912b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a4dbc610cf417ee6e53fad2b1a8a2912b"></a>

群消息屏蔽模式

**Returns**

[MsgMuteMode](broken-reference)

#### `public inline BMXGroup.GroupStatus groupStatus()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a889cbe63754b058b7de39ce61232ce17" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a889cbe63754b058b7de39ce61232ce17"></a>

当前群组的状态。（Normal 正常， Destroyed 以销毁）

**Returns**

[GroupStatus](broken-reference)

#### `public inline boolean isMember()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a300eea3b486b893c6d27071dbb870b7b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a300eea3b486b893c6d27071dbb870b7b"></a>

Deprecated use roleType instead.

当前用户是否是群成员

**Returns**

bool

#### `public inline boolean enableReadAck()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1aa3c9a64562cca776dd27793655ab4f8b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1aa3c9a64562cca776dd27793655ab4f8b"></a>

是否开启群消息已读功能

**Returns**

bool

#### `public inline boolean historyVisible()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1adafbdc91a61d2e854c6a0bcc145bc7a8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1adafbdc91a61d2e854c6a0bcc145bc7a8"></a>

是否可以加载显示历史聊天记录

**Returns**

bool

#### `public inline BMXGroup.MemberRoleType roleType()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a9f4193843e2e88e03afa88cd0ccad46a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a9f4193843e2e88e03afa88cd0ccad46a"></a>

成员在群组内的角色类型

**Returns**

[MemberRoleType](broken-reference)

#### `public inline long banExpireTime()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1adeee651b5cba9793f5bfbea14eecdc77" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1adeee651b5cba9793f5bfbea14eecdc77"></a>

群组全员禁言到期时间

#### `protected inline BMXGroup(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a47b42b869fb7a1c8e866bed031e2787a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1a47b42b869fb7a1c8e866bed031e2787a"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1ae57a7ae22b0f3b41638bce57d914e2b8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1ae57a7ae22b0f3b41638bce57d914e2b8"></a>

## class `Announcement` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement"></a>

群公告

### Summary

| Members                                                       | Descriptions |
| ------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                    |              |
| `public inline Announcement()`                                |              |
| `public inline void setMTitle(String value)`                  |              |
| `public inline String getMTitle()`                            |              |
| `public inline void setMContent(String value)`                |              |
| `public inline String getMContent()`                          |              |
| `public inline void setMAuthor(long value)`                   |              |
| `public inline long getMAuthor()`                             |              |
| `public inline void setMCreateTime(long value)`               |              |
| `public inline long getMCreateTime()`                         |              |
| `public inline void setMId(long value)`                       |              |
| `public inline long getMId()`                                 |              |
| `protected inline Announcement(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                            |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a00399a273d53d969d4de33fcb8c154fb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a00399a273d53d969d4de33fcb8c154fb"></a>

#### `public inline Announcement()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1aa56c100e9ae182f0fb09f3e31229eb15" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1aa56c100e9ae182f0fb09f3e31229eb15"></a>

#### `public inline void setMTitle(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a1803c50452d1eaf88dc3f3e45b1d6bcd" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a1803c50452d1eaf88dc3f3e45b1d6bcd"></a>

#### `public inline String getMTitle()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a8f01a514379cec1bf9ceb8437d0e9f32" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a8f01a514379cec1bf9ceb8437d0e9f32"></a>

#### `public inline void setMContent(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a4381207f23e36867641756372b59454e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a4381207f23e36867641756372b59454e"></a>

#### `public inline String getMContent()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a130732b54d13f681d6a2d530efe3521f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a130732b54d13f681d6a2d530efe3521f"></a>

#### `public inline void setMAuthor(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1ad4c023f96bcd14dd3d7fd7806228801d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1ad4c023f96bcd14dd3d7fd7806228801d"></a>

#### `public inline long getMAuthor()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a14e14fefcc03bf5ead55161d31be28a5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a14e14fefcc03bf5ead55161d31be28a5"></a>

#### `public inline void setMCreateTime(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a0772931faba5b116e11fd1d317557985" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a0772931faba5b116e11fd1d317557985"></a>

#### `public inline long getMCreateTime()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a0cbed92dfddc0e264aacaf3b0c2d007e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a0cbed92dfddc0e264aacaf3b0c2d007e"></a>

#### `public inline void setMId(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1aa5012e8bead1d20e16ec4e9f43578bfd" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1aa5012e8bead1d20e16ec4e9f43578bfd"></a>

#### `public inline long getMId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a73455fe85dfe819a5ec4dc607d8d5291" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a73455fe85dfe819a5ec4dc607d8d5291"></a>

#### `protected inline Announcement(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a59e60d3dd453668fa264dfee037c78fb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1a59e60d3dd453668fa264dfee037c78fb"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1aa2e7bd0464f0754d2bdbd31cfe1a35b4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_announcement_1aa2e7bd0464f0754d2bdbd31cfe1a35b4"></a>

## class `Application` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application"></a>

群申请

### Summary

| Members                                                           | Descriptions |
| ----------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                        |              |
| `public inline Application()`                                     |              |
| `public inline void setMGroupId(long value)`                      |              |
| `public inline long getMGroupId()`                                |              |
| `public inline void setMApplicationId(long value)`                |              |
| `public inline long getMApplicationId()`                          |              |
| `public inline void setMReason(String value)`                     |              |
| `public inline String getMReason()`                               |              |
| `public inline void setMStatus(BMXGroup.ApplicationStatus value)` |              |
| `public inline BMXGroup.ApplicationStatus getMStatus()`           |              |
| `public inline void setMExpired(long value)`                      |              |
| `public inline long getMExpired()`                                |              |
| `protected transient boolean swigCMemOwn`                         |              |
| `protected inline Application(long cPtr,boolean cMemoryOwn)`      |              |
| `protected inline void finalize()`                                |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1aa1ddda48aa0f8bdcc330153d1cae033d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1aa1ddda48aa0f8bdcc330153d1cae033d"></a>

#### `public inline Application()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1a1a888ba06c851c60122529079424573a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1a1a888ba06c851c60122529079424573a"></a>

#### `public inline void setMGroupId(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1ae488f7ba28a2e623a99a15c627388250" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1ae488f7ba28a2e623a99a15c627388250"></a>

#### `public inline long getMGroupId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1aa53b772e3a70f5de89a18c0da9a812e0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1aa53b772e3a70f5de89a18c0da9a812e0"></a>

#### `public inline void setMApplicationId(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1ad4867a2047eaf7e6197e41f8cd87120b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1ad4867a2047eaf7e6197e41f8cd87120b"></a>

#### `public inline long getMApplicationId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1a45dde055246c363f6a0ef9ea422070db" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1a45dde055246c363f6a0ef9ea422070db"></a>

#### `public inline void setMReason(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1a2fe228ef07ddf577240e5d2f666628d8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1a2fe228ef07ddf577240e5d2f666628d8"></a>

#### `public inline String getMReason()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1a8db117172e1fe055432375b6172d90c7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1a8db117172e1fe055432375b6172d90c7"></a>

#### `public inline void setMStatus(BMXGroup.ApplicationStatus value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1a240f932d67ccd819ffdd92451aca3cbf" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1a240f932d67ccd819ffdd92451aca3cbf"></a>

#### `public inline BMXGroup.ApplicationStatus getMStatus()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1a1f8065cb8abd13b8ecd0b908127dab76" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1a1f8065cb8abd13b8ecd0b908127dab76"></a>

#### `public inline void setMExpired(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1ae08af0dfb0717798d21aafae0fb49776" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1ae08af0dfb0717798d21aafae0fb49776"></a>

#### `public inline long getMExpired()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1a74edeefa0ed1c62a04a9ba402bd60d8e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1a74edeefa0ed1c62a04a9ba402bd60d8e"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1a4d354a7422f72269f24c5bbd59caa53c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1a4d354a7422f72269f24c5bbd59caa53c"></a>

#### `protected inline Application(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1aa8a869cdf343352c662c7558a6a9e537" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1aa8a869cdf343352c662c7558a6a9e537"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1aa79f44493e23de335017e4d441b1e7e2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_application_1aa79f44493e23de335017e4d441b1e7e2"></a>

## class `BannedMember` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member"></a>

群禁言成员

### Summary

| Members                                                       | Descriptions |
| ------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                    |              |
| `public inline BannedMember()`                                |              |
| `public inline void setMUid(long value)`                      |              |
| `public inline long getMUid()`                                |              |
| `public inline void setMGroupNickname(String value)`          |              |
| `public inline String getMGroupNickname()`                    |              |
| `public inline void setMCreateTime(long value)`               |              |
| `public inline long getMCreateTime()`                         |              |
| `public inline void setMExpired(long value)`                  |              |
| `public inline long getMExpired()`                            |              |
| `protected transient boolean swigCMemOwn`                     |              |
| `protected inline BannedMember(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                            |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a0a3852c877d4fc5b88b9ef15af69fdf2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a0a3852c877d4fc5b88b9ef15af69fdf2"></a>

#### `public inline BannedMember()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a88318b338acc2760d34f875e0709df67" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a88318b338acc2760d34f875e0709df67"></a>

#### `public inline void setMUid(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1ab6f08addc26dc378a67a8a4a0aedddbb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1ab6f08addc26dc378a67a8a4a0aedddbb"></a>

#### `public inline long getMUid()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a2cae261a5212958daeaf787edaa386c4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a2cae261a5212958daeaf787edaa386c4"></a>

#### `public inline void setMGroupNickname(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a1cfa1b5b718210c65b815fc913b14da2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a1cfa1b5b718210c65b815fc913b14da2"></a>

#### `public inline String getMGroupNickname()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a3b943c5fa3d78f254655ee291cdf988f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a3b943c5fa3d78f254655ee291cdf988f"></a>

#### `public inline void setMCreateTime(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1acce2c4d0f18d2754a8ecdffd03b0670a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1acce2c4d0f18d2754a8ecdffd03b0670a"></a>

#### `public inline long getMCreateTime()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1ad7b13ec9fbfd135c2c2d530a00a96eb4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1ad7b13ec9fbfd135c2c2d530a00a96eb4"></a>

#### `public inline void setMExpired(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a8df0c7dce03a3072d734ea8c07cb3bda" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a8df0c7dce03a3072d734ea8c07cb3bda"></a>

#### `public inline long getMExpired()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a959bc8c23865b747a99eb23057328422" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a959bc8c23865b747a99eb23057328422"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a327a2f307c10c7852785b899cfe0d965" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a327a2f307c10c7852785b899cfe0d965"></a>

#### `protected inline BannedMember(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a66aa88cab183f0c79ae0e3f403ac706f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1a66aa88cab183f0c79ae0e3f403ac706f"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1aab32f3fb06114191dada1c9d651e7db4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_banned_member_1aab32f3fb06114191dada1c9d651e7db4"></a>

## class `Invitation` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation"></a>

群邀请

### Summary

| Members                                                          | Descriptions |
| ---------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                       |              |
| `public inline Invitation()`                                     |              |
| `public inline void setMGroupId(long value)`                     |              |
| `public inline long getMGroupId()`                               |              |
| `public inline void setMInviterId(long value)`                   |              |
| `public inline long getMInviterId()`                             |              |
| `public inline void setMReason(String value)`                    |              |
| `public inline String getMReason()`                              |              |
| `public inline void setMStatus(BMXGroup.InvitationStatus value)` |              |
| `public inline BMXGroup.InvitationStatus getMStatus()`           |              |
| `public inline void setMExpired(long value)`                     |              |
| `public inline long getMExpired()`                               |              |
| `protected transient boolean swigCMemOwn`                        |              |
| `protected inline Invitation(long cPtr,boolean cMemoryOwn)`      |              |
| `protected inline void finalize()`                               |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1a5f898e85a55d0d52bd21828041ae1da8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1a5f898e85a55d0d52bd21828041ae1da8"></a>

#### `public inline Invitation()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1a6abd85058bd41d3ed70d10195117a4d2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1a6abd85058bd41d3ed70d10195117a4d2"></a>

#### `public inline void setMGroupId(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1ad9443aa99130e933ee5bc31579c1967e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1ad9443aa99130e933ee5bc31579c1967e"></a>

#### `public inline long getMGroupId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1ae5d54b326b1e20e13f153384d8f046ce" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1ae5d54b326b1e20e13f153384d8f046ce"></a>

#### `public inline void setMInviterId(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1a2426a21f626e00d519ae2b7e0a9931af" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1a2426a21f626e00d519ae2b7e0a9931af"></a>

#### `public inline long getMInviterId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1ad76f78d3693df328bfe5504221c582da" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1ad76f78d3693df328bfe5504221c582da"></a>

#### `public inline void setMReason(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1aeb3c6d1e94a617ec9dfcb3ab302a28bb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1aeb3c6d1e94a617ec9dfcb3ab302a28bb"></a>

#### `public inline String getMReason()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1a5cdf07ead0e83af37baccd772fdd82a5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1a5cdf07ead0e83af37baccd772fdd82a5"></a>

#### `public inline void setMStatus(BMXGroup.InvitationStatus value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1afaf9f615bb1ccd0f63264079bf0a91e0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1afaf9f615bb1ccd0f63264079bf0a91e0"></a>

#### `public inline BMXGroup.InvitationStatus getMStatus()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1a9546824e191b7441f226040e9a7bd05f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1a9546824e191b7441f226040e9a7bd05f"></a>

#### `public inline void setMExpired(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1a6d0fdac709188e151b27a34df73959b1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1a6d0fdac709188e151b27a34df73959b1"></a>

#### `public inline long getMExpired()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1a794c1f12cca9824fe416f347e551bbec" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1a794c1f12cca9824fe416f347e551bbec"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1ac84fce659791b948f9d79ab10eca7f1c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1ac84fce659791b948f9d79ab10eca7f1c"></a>

#### `protected inline Invitation(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1afd3bab0dc30e0c90c43725438127b255" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1afd3bab0dc30e0c90c43725438127b255"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1a94bdc45f160e62e246b9e2c9a523793f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_invitation_1a94bdc45f160e62e246b9e2c9a523793f"></a>

## class `Member` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member"></a>

群成员

### Summary

| Members                                                          | Descriptions |
| ---------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                       |              |
| `public inline Member(long uid,String nickname,long createTime)` |              |
| `public inline void setMUid(long value)`                         |              |
| `public inline long getMUid()`                                   |              |
| `public inline void setMGroupNickname(String value)`             |              |
| `public inline String getMGroupNickname()`                       |              |
| `public inline void setMCreateTime(long value)`                  |              |
| `public inline long getMCreateTime()`                            |              |
| `protected inline Member(long cPtr,boolean cMemoryOwn)`          |              |
| `protected inline void finalize()`                               |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1a0fe1249867785cd64463edaa0f647edb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1a0fe1249867785cd64463edaa0f647edb"></a>

#### `public inline Member(long uid,String nickname,long createTime)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1aad08b85287b03ae70efb2ddb983a88d4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1aad08b85287b03ae70efb2ddb983a88d4"></a>

#### `public inline void setMUid(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1ae76146510cfc8dfffa0799b7c393cd0e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1ae76146510cfc8dfffa0799b7c393cd0e"></a>

#### `public inline long getMUid()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1a9a8b2eaf94feffd5cd7cc43e74938e86" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1a9a8b2eaf94feffd5cd7cc43e74938e86"></a>

#### `public inline void setMGroupNickname(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1a1b92f05fe96f921226a69dfd41d44255" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1a1b92f05fe96f921226a69dfd41d44255"></a>

#### `public inline String getMGroupNickname()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1a84b623fa188b23cd3d0ef2f7c5ee8896" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1a84b623fa188b23cd3d0ef2f7c5ee8896"></a>

#### `public inline void setMCreateTime(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1ad7c6da2e1abfafabe8805387579b63c2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1ad7c6da2e1abfafabe8805387579b63c2"></a>

#### `public inline long getMCreateTime()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1a4227887755b9d4b9cd101ef27d8169db" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1a4227887755b9d4b9cd101ef27d8169db"></a>

#### `protected inline Member(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1abe398b10157f5e872f25e3c35cb2f58e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1abe398b10157f5e872f25e3c35cb2f58e"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1a408908b37c6d3300226c28e217105837" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_member_1a408908b37c6d3300226c28e217105837"></a>

## class `SharedFile` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file"></a>

群共享文件

### Summary

| Members                                                     | Descriptions |
| ----------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                  |              |
| `public inline SharedFile()`                                |              |
| `public inline void setMFileId(long value)`                 |              |
| `public inline long getMFileId()`                           |              |
| `public inline void setMGroupId(long value)`                |              |
| `public inline long getMGroupId()`                          |              |
| `public inline void setMUploader(long value)`               |              |
| `public inline long getMUploader()`                         |              |
| `public inline void setMSize(int value)`                    |              |
| `public inline int getMSize()`                              |              |
| `public inline void setMCreateTime(long value)`             |              |
| `public inline long getMCreateTime()`                       |              |
| `public inline void setMUpdateTime(long value)`             |              |
| `public inline long getMUpdateTime()`                       |              |
| `public inline void setMRatelUrl(String value)`             |              |
| `public inline String getMRatelUrl()`                       |              |
| `public inline void setMUrl(String value)`                  |              |
| `public inline String getMUrl()`                            |              |
| `public inline void setMPath(String value)`                 |              |
| `public inline String getMPath()`                           |              |
| `public inline void setMDisplayName(String value)`          |              |
| `public inline String getMDisplayName()`                    |              |
| `public inline void setMType(String value)`                 |              |
| `public inline String getMType()`                           |              |
| `protected inline SharedFile(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                          |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a54679a64ab0cac176cfbc4403a0a2b7e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a54679a64ab0cac176cfbc4403a0a2b7e"></a>

#### `public inline SharedFile()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1aa98ded23e2eedd96fb712f7084ab733d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1aa98ded23e2eedd96fb712f7084ab733d"></a>

#### `public inline void setMFileId(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a3da41280799ea9cade190946483ccef4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a3da41280799ea9cade190946483ccef4"></a>

#### `public inline long getMFileId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a5a75b2321e6a15c16143fa32d430fc48" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a5a75b2321e6a15c16143fa32d430fc48"></a>

#### `public inline void setMGroupId(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a22b32d91bf2b4409d2fa7aad09baaabf" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a22b32d91bf2b4409d2fa7aad09baaabf"></a>

#### `public inline long getMGroupId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1aaf01ca1c8328b986e9b9ae1fc6eb060d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1aaf01ca1c8328b986e9b9ae1fc6eb060d"></a>

#### `public inline void setMUploader(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1ad35a1752df1df1c4fa7d6ac4a314b953" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1ad35a1752df1df1c4fa7d6ac4a314b953"></a>

#### `public inline long getMUploader()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1ade74af73e52745408c0b173aaae86d13" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1ade74af73e52745408c0b173aaae86d13"></a>

#### `public inline void setMSize(int value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a6e47a6e6e9f97e3a31099874945195ba" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a6e47a6e6e9f97e3a31099874945195ba"></a>

#### `public inline int getMSize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1af59f477900effff388808317ba0f7977" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1af59f477900effff388808317ba0f7977"></a>

#### `public inline void setMCreateTime(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1ab60066d65272b3111b9e500313a7e579" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1ab60066d65272b3111b9e500313a7e579"></a>

#### `public inline long getMCreateTime()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a6744775aa0e805f12eb00d365a7dd38e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a6744775aa0e805f12eb00d365a7dd38e"></a>

#### `public inline void setMUpdateTime(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1aa9707d8d1a1ff0bbf7c5fb12781881cf" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1aa9707d8d1a1ff0bbf7c5fb12781881cf"></a>

#### `public inline long getMUpdateTime()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a8a1d7a7f6e660a7f09ba9a59bebe6ab5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a8a1d7a7f6e660a7f09ba9a59bebe6ab5"></a>

#### `public inline void setMRatelUrl(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1ad7f6f6d85413290cc78bb92d9f8df9c2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1ad7f6f6d85413290cc78bb92d9f8df9c2"></a>

#### `public inline String getMRatelUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1aba7f825fc2046565ec6ecb700e235af0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1aba7f825fc2046565ec6ecb700e235af0"></a>

#### `public inline void setMUrl(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1ac4f5318748d0cfa332990fa2f39d5c10" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1ac4f5318748d0cfa332990fa2f39d5c10"></a>

#### `public inline String getMUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1ac639afe2cb6770bc044b751cfd9fd13c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1ac639afe2cb6770bc044b751cfd9fd13c"></a>

#### `public inline void setMPath(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a04d3b914da0b21ca2919058bde096cb6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a04d3b914da0b21ca2919058bde096cb6"></a>

#### `public inline String getMPath()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1aa22f7444d8753c88494211a58c41a8cc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1aa22f7444d8753c88494211a58c41a8cc"></a>

#### `public inline void setMDisplayName(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a4d881970abaab3c1d3ff4aabec0f34e2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a4d881970abaab3c1d3ff4aabec0f34e2"></a>

#### `public inline String getMDisplayName()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a65d0fe8e59e6d28a50421db1e839a40a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a65d0fe8e59e6d28a50421db1e839a40a"></a>

#### `public inline void setMType(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a721e56a10678bb5ecb18eefb2cb6f32c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1a721e56a10678bb5ecb18eefb2cb6f32c"></a>

#### `public inline String getMType()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1ad811545fe914e80893ff61601f225bfe" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1ad811545fe914e80893ff61601f225bfe"></a>

#### `protected inline SharedFile(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1ac87cd28175b3385ca47c8bc15a2554a3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1ac87cd28175b3385ca47c8bc15a2554a3"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1af24189ae3766294d29cbaaff2fdc647c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_1_1_shared_file_1af24189ae3766294d29cbaaff2fdc647c"></a>

## class `BMXRosterService` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service"></a>

好友Service

### Summary

| Members                                                                                                                                                                                            | Descriptions                            |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------- |
| `class` [`Application`](broken-reference)                                                                                                                                                          | 好友邀请                                    |
| `public inline synchronized void delete()`                                                                                                                                                         |                                         |
| `public inline` [`BMXErrorCode`](broken-reference) `get(`[`ListOfLongLong`](broken-reference) `list,boolean forceRefresh)`                                                                         | 获取好友列表，如果forceRefresh == true，则强制从服务端拉取 |
| `public inline` [`BMXErrorCode`](broken-reference) `fetchRosterById(long rosterId,boolean forceRefresh,`[`BMXRosterItem`](broken-reference) `item)`                                                | 搜索用户                                    |
| `public inline` [`BMXErrorCode`](broken-reference) `search(long rosterId,boolean forceRefresh,`[`BMXRosterItem`](broken-reference) `item)`                                                         | 搜索用户                                    |
| `public inline` [`BMXErrorCode`](broken-reference) `fetchRosterByName(String name,boolean forceRefresh,`[`BMXRosterItem`](broken-reference) `item)`                                                | 搜索用户                                    |
| `public inline` [`BMXErrorCode`](broken-reference) `search(String name,boolean forceRefresh,`[`BMXRosterItem`](broken-reference) `item)`                                                           | 搜索用户                                    |
| `public inline` [`BMXErrorCode`](broken-reference) `fetchRostersByIdList(`[`ListOfLongLong`](broken-reference) `rosterIdList,`[`BMXRosterItemList`](broken-reference) `list,boolean forceRefresh)` | 批量搜索用户                                  |
| `public inline` [`BMXErrorCode`](broken-reference) `search(`[`ListOfLongLong`](broken-reference) `rosterIdList,`[`BMXRosterItemList`](broken-reference) `list,boolean forceRefresh)`               | 批量搜索用户                                  |
| `public inline` [`BMXErrorCode`](broken-reference) `setItemLocalExtension(`[`BMXRosterItem`](broken-reference) `item,String extension)`                                                            | 更新好友本地扩展信息                              |
| `public inline` [`BMXErrorCode`](broken-reference) `setItemExtension(`[`BMXRosterItem`](broken-reference) `item,String extension)`                                                                 | 更新好友服务器扩展信息                             |
| `public inline` [`BMXErrorCode`](broken-reference) `setItemAlias(`[`BMXRosterItem`](broken-reference) `item,String alias)`                                                                         | 更新好友别名                                  |
| `public inline` [`BMXErrorCode`](broken-reference) `setItemMuteNotification(`[`BMXRosterItem`](broken-reference) `item,boolean status)`                                                            | 设置是否拒收用户消息                              |
| `public inline` [`BMXErrorCode`](broken-reference) `getApplicationList(`[`ApplicationPage`](broken-reference) `result,String cursor,int pageSize)`                                                 | 获取申请添加好友列表                              |
| `public inline` [`BMXErrorCode`](broken-reference) `apply(long rosterId,String message,String authAnswer)`                                                                                         |                                         |
| `public inline` [`BMXErrorCode`](broken-reference) `apply(long rosterId,String message)`                                                                                                           | 申请添加好友                                  |
| `public inline` [`BMXErrorCode`](broken-reference) `remove(long rosterId)`                                                                                                                         | 删除好友                                    |
| `public inline` [`BMXErrorCode`](broken-reference) `accept(long rosterId)`                                                                                                                         | 接受加好友申请                                 |
| `public inline` [`BMXErrorCode`](broken-reference) `decline(long rosterId,String reason)`                                                                                                          | 拒绝加好友申请                                 |
| `public inline` [`BMXErrorCode`](broken-reference) `block(long rosterId)`                                                                                                                          | 加入黑名单                                   |
| `public inline` [`BMXErrorCode`](broken-reference) `unblock(long rosterId)`                                                                                                                        | 从黑名单移除                                  |
| `public inline` [`BMXErrorCode`](broken-reference) `getBlockList(`[`ListOfLongLong`](broken-reference) `list,boolean forceRefresh)`                                                                | 获取黑名单，如果forceRefresh == true，则强制从服务端拉取  |
| `public inline` [`BMXErrorCode`](broken-reference) `downloadAvatar(`[`BMXRosterItem`](broken-reference) `item,boolean thumbnail,`[`FileProgressListener`](broken-reference) `listener)`            | 下载头像                                    |
| `public inline void addRosterListener(`[`BMXRosterServiceListener`](broken-reference) `listener)`                                                                                                  | 添加好友变化监听者                               |
| `public inline void removeRosterListener(`[`BMXRosterServiceListener`](broken-reference) `listener)`                                                                                               | 移除好友变化监听者                               |
| `protected transient boolean swigCMemOwn`                                                                                                                                                          |                                         |
| `protected inline BMXRosterService(long cPtr,boolean cMemoryOwn)`                                                                                                                                  |                                         |
| `protected inline void finalize()`                                                                                                                                                                 |                                         |

### Members

#### `class` [`Application`](broken-reference) <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application"></a>

好友邀请

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1ac974b2d160838d7b30598eec2495c651" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1ac974b2d160838d7b30598eec2495c651"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `get(`[`ListOfLongLong`](broken-reference) `list,boolean forceRefresh)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1afdfa651b8c6a6e88431e75b633c318e8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1afdfa651b8c6a6e88431e75b633c318e8"></a>

获取好友列表，如果forceRefresh == true，则强制从服务端拉取

**Parameters**

* `list` 好友id列表，传入空列表函数返回后从此处获取返回的好友id列表
* `forceRefresh` 是否从服务器读取数据，true为强制从服务器获取，false情况下本地读取列表为空的情况下会自动从服务器读取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `fetchRosterById(long rosterId,boolean forceRefresh,`[`BMXRosterItem`](broken-reference) `item)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a30e814165f2632476f546fb82d2fe3c9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a30e814165f2632476f546fb82d2fe3c9"></a>

搜索用户

**Parameters**

* `rosterId` 搜索的好友id
* `forceRefresh` 为true强制从服务器获取，为false情况下查询结果为空时自动从服务器获取。
* `item` 查询返回的用户的信息，传入指向为空的shared\_ptr对象函数执行后会自动赋值。

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `search(long rosterId,boolean forceRefresh,`[`BMXRosterItem`](broken-reference) `item)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a26fbc8e5d5cb72ff8e569e9a46fb0426" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a26fbc8e5d5cb72ff8e569e9a46fb0426"></a>

搜索用户

**Parameters**

* `rosterId` 搜索的好友id
* `forceRefresh` 为true强制从服务器获取，为false情况下查询结果为空时自动从服务器获取。
* `item` 查询返回的用户的信息，传入指向为空的shared\_ptr对象函数执行后会自动赋值。

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `fetchRosterByName(String name,boolean forceRefresh,`[`BMXRosterItem`](broken-reference) `item)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a15351be6677d071165cdbfd7675feaa3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a15351be6677d071165cdbfd7675feaa3"></a>

搜索用户

**Parameters**

* `name` 搜索的用户名
* `forceRefresh` 为true强制从服务器获取，为false情况下查询结果为空时自动从服务器获取。
* `item` 查询返回的用户的信息，传入指向为空的shared\_ptr对象函数执行后会自动赋值。

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `search(String name,boolean forceRefresh,`[`BMXRosterItem`](broken-reference) `item)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a7ff40296049196fbef600c98c12eb1fb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a7ff40296049196fbef600c98c12eb1fb"></a>

搜索用户

**Parameters**

* `name` 搜索的用户名
* `forceRefresh` 为true强制从服务器获取，为false情况下查询结果为空时自动从服务器获取。
* `item` 查询返回的用户的信息，传入指向为空的shared\_ptr对象函数执行后会自动赋值。

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `fetchRostersByIdList(`[`ListOfLongLong`](broken-reference) `rosterIdList,`[`BMXRosterItemList`](broken-reference) `list,boolean forceRefresh)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a7f5e7eef2d0bec38a0134afb986effc8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a7f5e7eef2d0bec38a0134afb986effc8"></a>

批量搜索用户

**Parameters**

* `rosterIdList` 需要搜索的用户id列表
* `list` 返回的好友信息列表，传入空列表函数返回后从此处获取返回的好友信息列表
* `forceRefresh` 是否强制从服务器获取，为true则强制从服务器获取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `search(`[`ListOfLongLong`](broken-reference) `rosterIdList,`[`BMXRosterItemList`](broken-reference) `list,boolean forceRefresh)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a70ab7213260ed40b921fb708f55f19d6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a70ab7213260ed40b921fb708f55f19d6"></a>

批量搜索用户

**Parameters**

* `rosterIdList` 需要搜索的用户id列表
* `list` 返回的好友信息列表，传入空列表函数返回后从此处获取返回的好友信息列表
* `forceRefresh` 是否强制从服务器获取，为true则强制从服务器获取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setItemLocalExtension(`[`BMXRosterItem`](broken-reference) `item,String extension)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a367d09b2ca0925cf78e62c2014c51371" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a367d09b2ca0925cf78e62c2014c51371"></a>

更新好友本地扩展信息

**Parameters**

* `item` 用户信息
* `extension` 本地扩展信息

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setItemExtension(`[`BMXRosterItem`](broken-reference) `item,String extension)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a2464d57daf6d2b76bfe7ab3fcfa7ea18" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a2464d57daf6d2b76bfe7ab3fcfa7ea18"></a>

更新好友服务器扩展信息

**Parameters**

* `item` 用户信息
* `extension` 服务器扩展信息

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setItemAlias(`[`BMXRosterItem`](broken-reference) `item,String alias)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a0911f1aa6ac62b046983057a27dae358" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a0911f1aa6ac62b046983057a27dae358"></a>

更新好友别名

**Parameters**

* `item` 用户信息
* `alias` 好友别名

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setItemMuteNotification(`[`BMXRosterItem`](broken-reference) `item,boolean status)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a0fac5ccd622b81a8ee2b504ded9101ee" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a0fac5ccd622b81a8ee2b504ded9101ee"></a>

设置是否拒收用户消息

**Parameters**

* `item` 用户信息
* `status` 是否拒收用户消息，true拒收，false不拒收

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getApplicationList(`[`ApplicationPage`](broken-reference) `result,String cursor,int pageSize)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a0fb804cb11825d68a0d03287c2b9e921" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a0fb804cb11825d68a0d03287c2b9e921"></a>

获取申请添加好友列表

**Parameters**

* `result` 返回的申请好友列表信息，传入指向为空的shared\_ptr对象函数执行后会自动赋值。
* `cursor` 分页获取的起始cursor，第一次传入为空，后续传入上次操作返回的result中的cursor
* `pageSize` 分页大小

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `apply(long rosterId,String message,String authAnswer)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a49e06345d8f86a7d3fb582f4c7edc6f2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a49e06345d8f86a7d3fb582f4c7edc6f2"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `apply(long rosterId,String message)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a643b190b6773e03fdb4e938b3810cdf0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a643b190b6773e03fdb4e938b3810cdf0"></a>

申请添加好友

**Parameters**

* `rosterId` 申请添加的用户id
* `message` 好友申请信息

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `remove(long rosterId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a10831cb770bd2e3cede944646e3deb65" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a10831cb770bd2e3cede944646e3deb65"></a>

删除好友

**Parameters**

* `rosterId` 删除的好友id

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `accept(long rosterId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a70895807f1db3d068872e4319fcca59f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a70895807f1db3d068872e4319fcca59f"></a>

接受加好友申请

**Parameters**

* `rosterId` 申请加为好友的用户id

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `decline(long rosterId,String reason)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a4b7402410678a76f799cc64f2243ff58" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a4b7402410678a76f799cc64f2243ff58"></a>

拒绝加好友申请

**Parameters**

* `rosterId` 申请加为好友的用户id
* `reason` 拒绝的原因

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `block(long rosterId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a22e264fc31e395952ce6a2253c841e8b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a22e264fc31e395952ce6a2253c841e8b"></a>

加入黑名单

**Parameters**

* `rosterId` 加入黑名单的用户id

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `unblock(long rosterId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1abbb5ca7f8d763d35eeb70526a4a87a08" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1abbb5ca7f8d763d35eeb70526a4a87a08"></a>

从黑名单移除

**Parameters**

* `rosterId` 从黑名单移除的用户id

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getBlockList(`[`ListOfLongLong`](broken-reference) `list,boolean forceRefresh)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1ab13d96dd6f8431bd1ef99093b1b203a8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1ab13d96dd6f8431bd1ef99093b1b203a8"></a>

获取黑名单，如果forceRefresh == true，则强制从服务端拉取

**Parameters**

* `list` 好友id列表，传入空列表函数返回后从此处获取返回的黑名单id列表
* `forceRefresh` 是否从服务器读取数据，true为强制从服务器获取，false情况下本地读取列表为空的情况下会自动从服务器读取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `downloadAvatar(`[`BMXRosterItem`](broken-reference) `item,boolean thumbnail,`[`FileProgressListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a80f506c46a18d383f8223235387a069f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a80f506c46a18d383f8223235387a069f"></a>

下载头像

**Parameters**

* `item` 用户信息
* `thumbnail` 是否下载缩略图，ture为缩略图，false为原图
* `listener` 下载回调函数

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline void addRosterListener(`[`BMXRosterServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1acda61ab06cba0814b88fec49faa41d68" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1acda61ab06cba0814b88fec49faa41d68"></a>

添加好友变化监听者

**Parameters**

* `listener` 好友变化监听者

#### `public inline void removeRosterListener(`[`BMXRosterServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a6350f8f2223cf28775f756fe3b3cbbbc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a6350f8f2223cf28775f756fe3b3cbbbc"></a>

移除好友变化监听者

**Parameters**

* `listener` 好友变化监听者

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a9f822b238c5fcef9ab0d3eed965aef86" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a9f822b238c5fcef9ab0d3eed965aef86"></a>

#### `protected inline BMXRosterService(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a3f26baedb92027bc685b9e0942e9223c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a3f26baedb92027bc685b9e0942e9223c"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a780f050f13762ed53696d965ed2b6b91" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1a780f050f13762ed53696d965ed2b6b91"></a>

## class `Application` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application"></a>

好友邀请

### Summary

| Members                                                                   | Descriptions |
| ------------------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                                |              |
| `public inline Application()`                                             |              |
| `public inline void setMRosterId(long value)`                             |              |
| `public inline long getMRosterId()`                                       |              |
| `public inline void setMReason(String value)`                             |              |
| `public inline String getMReason()`                                       |              |
| `public inline void setMStatus(BMXRosterService.ApplicationStatus value)` |              |
| `public inline BMXRosterService.ApplicationStatus getMStatus()`           |              |
| `public inline void setMExpire(long value)`                               |              |
| `public inline long getMExpire()`                                         |              |
| `protected transient boolean swigCMemOwn`                                 |              |
| `protected inline Application(long cPtr,boolean cMemoryOwn)`              |              |
| `protected inline void finalize()`                                        |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1ad7c3ea07e0c527365baa5b50be6106" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1ad7c3ea07e0c527365baa5b50be6106"></a>

#### `public inline Application()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a88b169887e7ed2d48022f0d7aafaae" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a88b169887e7ed2d48022f0d7aafaae"></a>

#### `public inline void setMRosterId(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a90716c8523a3388989ee64ee5a233a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a90716c8523a3388989ee64ee5a233a"></a>

#### `public inline long getMRosterId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a461bda0df78231e5798a956f1a25fe" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a461bda0df78231e5798a956f1a25fe"></a>

#### `public inline void setMReason(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a4bc1d5d4a3833c3cfe630ee786d7c4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a4bc1d5d4a3833c3cfe630ee786d7c4"></a>

#### `public inline String getMReason()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a203979595800e32bf9d0c7cb04ff13" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a203979595800e32bf9d0c7cb04ff13"></a>

#### `public inline void setMStatus(BMXRosterService.ApplicationStatus value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a313bac7c86857d4ca415456c47db01" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a313bac7c86857d4ca415456c47db01"></a>

#### `public inline BMXRosterService.ApplicationStatus getMStatus()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a6df79d28acfdabb1951df75d8ce8c1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a6df79d28acfdabb1951df75d8ce8c1"></a>

#### `public inline void setMExpire(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1ae1a1865e1173d1ce5050502087c985" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1ae1a1865e1173d1ce5050502087c985"></a>

#### `public inline long getMExpire()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a9eb03a31b3b327aec3474b34f126ab" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a9eb03a31b3b327aec3474b34f126ab"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a190dbeb7d81c670ef5eb251d2f6978" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a190dbeb7d81c670ef5eb251d2f6978"></a>

#### `protected inline Application(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a1110fdeee1ccae739c465cf8224e00" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a1110fdeee1ccae739c465cf8224e00"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a4bbabc0338229a61a5649065cce498" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_1_1_application_1a4bbabc0338229a61a5649065cce498"></a>

## class `ApplicationPage` <a href="#classim_1_1floo_1_1floolib_1_1_application_page" id="classim_1_1floo_1_1floolib_1_1_application_page"></a>

```
class ApplicationPage
  : public im.floo.floolib.BMXBaseObject
```

### Summary

| Members                                                                                                       | Descriptions |
| ------------------------------------------------------------------------------------------------------------- | ------------ |
| `public transient long swigCPtr`                                                                              |              |
| `public inline synchronized void delete()`                                                                    |              |
| `public inline ApplicationPage()`                                                                             |              |
| `public inline ApplicationPage(`[`BMXRosterServiceApplicationList`](broken-reference) `result,long offset)`   |              |
| `public inline ApplicationPage(`[`BMXRosterServiceApplicationList`](broken-reference) `result,String cursor)` |              |
| `public inline ApplicationPage(`[`ApplicationPage`](broken-reference) `from)`                                 |              |
| `public inline long count()`                                                                                  |              |
| `public inline long offset()`                                                                                 |              |
| `public inline String cursor()`                                                                               |              |
| `public inline` [`BMXRosterServiceApplicationList`](broken-reference) `result()`                              |              |
| `protected inline ApplicationPage(long cPtr,boolean cMemoryOwn)`                                              |              |
| `protected inline void finalize()`                                                                            |              |

### Members

#### `public transient long swigCPtr` <a href="#classim_1_1floo_1_1floolib_1_1_application_page_1a40e96c015c532b6951a90d533d929683" id="classim_1_1floo_1_1floolib_1_1_application_page_1a40e96c015c532b6951a90d533d929683"></a>

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_application_page_1a619f9764f70e66642ad50de8baaec219" id="classim_1_1floo_1_1floolib_1_1_application_page_1a619f9764f70e66642ad50de8baaec219"></a>

#### `public inline ApplicationPage()` <a href="#classim_1_1floo_1_1floolib_1_1_application_page_1a3b4dabc6acc7536cdf304a2ea70ca0b6" id="classim_1_1floo_1_1floolib_1_1_application_page_1a3b4dabc6acc7536cdf304a2ea70ca0b6"></a>

#### `public inline ApplicationPage(`[`BMXRosterServiceApplicationList`](broken-reference) `result,long offset)` <a href="#classim_1_1floo_1_1floolib_1_1_application_page_1a303487e2b2ce12853aaf0191a4bf75a6" id="classim_1_1floo_1_1floolib_1_1_application_page_1a303487e2b2ce12853aaf0191a4bf75a6"></a>

#### `public inline ApplicationPage(`[`BMXRosterServiceApplicationList`](broken-reference) `result,String cursor)` <a href="#classim_1_1floo_1_1floolib_1_1_application_page_1a13f378974fa56aea03574c2442a03cc4" id="classim_1_1floo_1_1floolib_1_1_application_page_1a13f378974fa56aea03574c2442a03cc4"></a>

#### `public inline ApplicationPage(`[`ApplicationPage`](broken-reference) `from)` <a href="#classim_1_1floo_1_1floolib_1_1_application_page_1a90bd25f8481ccc8b77c5eda3115788d5" id="classim_1_1floo_1_1floolib_1_1_application_page_1a90bd25f8481ccc8b77c5eda3115788d5"></a>

#### `public inline long count()` <a href="#classim_1_1floo_1_1floolib_1_1_application_page_1a27638d9018b8ae083b446844ae31db71" id="classim_1_1floo_1_1floolib_1_1_application_page_1a27638d9018b8ae083b446844ae31db71"></a>

#### `public inline long offset()` <a href="#classim_1_1floo_1_1floolib_1_1_application_page_1a64cf59ca539ad1aac45f2b3cc89dcb94" id="classim_1_1floo_1_1floolib_1_1_application_page_1a64cf59ca539ad1aac45f2b3cc89dcb94"></a>

#### `public inline String cursor()` <a href="#classim_1_1floo_1_1floolib_1_1_application_page_1a43ca6baeefce86ecb075193101a7d07d" id="classim_1_1floo_1_1floolib_1_1_application_page_1a43ca6baeefce86ecb075193101a7d07d"></a>

#### `public inline` [`BMXRosterServiceApplicationList`](broken-reference) `result()` <a href="#classim_1_1floo_1_1floolib_1_1_application_page_1a9021203569c01edf33e22a80a1b1b75b" id="classim_1_1floo_1_1floolib_1_1_application_page_1a9021203569c01edf33e22a80a1b1b75b"></a>

#### `protected inline ApplicationPage(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_application_page_1aaaf387ce93e484506be292a38a7789cb" id="classim_1_1floo_1_1floolib_1_1_application_page_1aaaf387ce93e484506be292a38a7789cb"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_application_page_1acc34594d39fcfa2270449f3c79d1f8c7" id="classim_1_1floo_1_1floolib_1_1_application_page_1acc34594d39fcfa2270449f3c79d1f8c7"></a>

## class `BMXMessageConfig` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config"></a>

```
class BMXMessageConfig
  : public im.floo.floolib.BMXBaseObject
```

消息配置

### Summary

| Members                                                                                         | Descriptions        |
| ----------------------------------------------------------------------------------------------- | ------------------- |
| `public inline synchronized void delete()`                                                      |                     |
| `public inline void setMentionAll(boolean mentionAll)`                                          | 设置是否@全员             |
| `public inline boolean getMentionAll()`                                                         | 获取是否@全员             |
| `public inline void setMentionList(`[`ListOfLongLong`](broken-reference) `mentionList)`         | 设置通知成员id列表          |
| `public inline` [`ListOfLongLong`](broken-reference) `getMentionList()`                         | 获取@成员列表             |
| `public inline void setMentionedMessage(String mentionedMessage)`                               | 设置@消息               |
| `public inline String getMentionedMessage()`                                                    | 获取@消息               |
| `public inline void setPushMessage(String pushMessage)`                                         | 设置推送消息              |
| `public inline String getPushMessage()`                                                         | 获取推送消息              |
| `public inline void setSenderNickname(String senderNickname)`                                   | 设置发送者昵称             |
| `public inline String getSenderNickname()`                                                      | 获取发送者昵称             |
| `public inline void setGroupMemberList(`[`ListOfLongLong`](broken-reference) `groupMemberList)` | 设置需要群已读消息的群成员id列表   |
| `public inline` [`ListOfLongLong`](broken-reference) `getGroupMemberList()`                     | 获取需要群已读消息的群成员id列表   |
| `public inline void addGroupMember(long id)`                                                    | 添加群已读消息的群成员id列表成员   |
| `public inline void removeGroupMember(long id)`                                                 | 清除需要群已读消息的群成员id列表成员 |
| `public inline void clearGroupMemberList()`                                                     | 清空群已读消息的群成员id列表     |
| `public inline void setIOSConfig(String iosConfig)`                                             |                     |
| `public inline String getIOSConfig()`                                                           | 获取iOS消息配置           |
| `public inline void setAndroidConfig(String androidConfig)`                                     |                     |
| `public inline String getAndroidConfig()`                                                       | 获取Android消息配置       |
| `public inline void setPushShowBeginTime(int beginTime)`                                        |                     |
| `public inline int getPushShowBeginTime()`                                                      | 获取推送消息开始展示时间        |
| `public inline void setPushShowEndTime(int endTime)`                                            |                     |
| `public inline int getPushShowEndTime()`                                                        | 获取推送消息结束展示时间        |
| `public inline void setPushTitle(String pushTitle)`                                             |                     |
| `public inline String getPushTitle()`                                                           | 获取推送消息标题            |
| `public inline boolean isSilence()`                                                             |                     |
| `public inline BMXMessageConfig.BadgeCountType getBadgeCountType()`                             |                     |
| `public inline int getBadgeCount(int count)`                                                    |                     |
| `public inline String getUsername()`                                                            | 获取消息发送者用户名          |
| `public inline String serialize()`                                                              | 序列化操作               |
| `protected inline BMXMessageConfig(long cPtr,boolean cMemoryOwn)`                               |                     |
| `protected inline void finalize()`                                                              |                     |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a7cc25883c2c59e28abd93baea3a65f11" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a7cc25883c2c59e28abd93baea3a65f11"></a>

#### `public inline void setMentionAll(boolean mentionAll)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a77ad20591783ec24059221f761c92432" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a77ad20591783ec24059221f761c92432"></a>

设置是否@全员

**Parameters**

* `mentionAll`

#### `public inline boolean getMentionAll()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a33e74941a32d986029fb21f09823d66e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a33e74941a32d986029fb21f09823d66e"></a>

获取是否@全员

**Returns**

bool

#### `public inline void setMentionList(`[`ListOfLongLong`](broken-reference) `mentionList)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a1dc89a8980fea733328c26795390faf8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a1dc89a8980fea733328c26795390faf8"></a>

设置通知成员id列表

**Parameters**

* `mentionList`

#### `public inline` [`ListOfLongLong`](broken-reference) `getMentionList()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a464a995b51a69e68bfae03883dfc9036" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a464a995b51a69e68bfae03883dfc9036"></a>

获取@成员列表

**Returns**

std::vector\<int64\_t>

#### `public inline void setMentionedMessage(String mentionedMessage)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a3e7518a72967bee85795e27f33e236f3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a3e7518a72967bee85795e27f33e236f3"></a>

设置@消息

**Parameters**

* `mentionedMessage`

#### `public inline String getMentionedMessage()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a17131b1361dd7bb2b49446b2c405b109" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a17131b1361dd7bb2b49446b2c405b109"></a>

获取@消息

**Returns**

std::string

#### `public inline void setPushMessage(String pushMessage)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a5f34007d0d7e6513b88f0b20c1db7629" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a5f34007d0d7e6513b88f0b20c1db7629"></a>

设置推送消息

**Parameters**

* `pushMessage`

#### `public inline String getPushMessage()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1aa4fa9ee03b311935ac1060a1f153fff5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1aa4fa9ee03b311935ac1060a1f153fff5"></a>

获取推送消息

**Returns**

std::string

#### `public inline void setSenderNickname(String senderNickname)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1adf3998388bb54395530004c5915855bd" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1adf3998388bb54395530004c5915855bd"></a>

设置发送者昵称

**Parameters**

* `senderNickname`

#### `public inline String getSenderNickname()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1adc3f893a67000eb4208a5ca516c0440e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1adc3f893a67000eb4208a5ca516c0440e"></a>

获取发送者昵称

**Returns**

std::string

#### `public inline void setGroupMemberList(`[`ListOfLongLong`](broken-reference) `groupMemberList)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a9ced11c20e5b8baf7ecdd1b32d756d42" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a9ced11c20e5b8baf7ecdd1b32d756d42"></a>

设置需要群已读消息的群成员id列表

**Parameters**

* `groupMemberList`

#### `public inline` [`ListOfLongLong`](broken-reference) `getGroupMemberList()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a882d0b564cf800fcf78e111617eddb1b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a882d0b564cf800fcf78e111617eddb1b"></a>

获取需要群已读消息的群成员id列表

**Returns**

std::vector\<int64\_t>

#### `public inline void addGroupMember(long id)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a87c78819ea0cc5396c70cf47b9ede369" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a87c78819ea0cc5396c70cf47b9ede369"></a>

添加群已读消息的群成员id列表成员

#### `public inline void removeGroupMember(long id)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a300d01db7592b0fb888e1afe72149873" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a300d01db7592b0fb888e1afe72149873"></a>

清除需要群已读消息的群成员id列表成员

#### `public inline void clearGroupMemberList()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1aa0fb6ab1a6e69b988e113531e367479e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1aa0fb6ab1a6e69b988e113531e367479e"></a>

清空群已读消息的群成员id列表

#### `public inline void setIOSConfig(String iosConfig)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1addd59c526f48b621beb0b4364bbfdff6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1addd59c526f48b621beb0b4364bbfdff6"></a>

#### `public inline String getIOSConfig()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a5647450185de9163b88cf9cf553e3cf0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a5647450185de9163b88cf9cf553e3cf0"></a>

获取iOS消息配置

#### `public inline void setAndroidConfig(String androidConfig)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1aac76182e7b9e59e9ec0e068f914cca74" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1aac76182e7b9e59e9ec0e068f914cca74"></a>

#### `public inline String getAndroidConfig()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a5e5579f11817ebca1e58adf2efbea330" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a5e5579f11817ebca1e58adf2efbea330"></a>

获取Android消息配置

#### `public inline void setPushShowBeginTime(int beginTime)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a50c3de9368d139e7d91fd3528a8a7b1e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a50c3de9368d139e7d91fd3528a8a7b1e"></a>

#### `public inline int getPushShowBeginTime()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a8d3ee9c130447bd53ae4b93f8175780a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a8d3ee9c130447bd53ae4b93f8175780a"></a>

获取推送消息开始展示时间

#### `public inline void setPushShowEndTime(int endTime)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a09f850f66b1d8f5cce7badfc4f42792c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a09f850f66b1d8f5cce7badfc4f42792c"></a>

#### `public inline int getPushShowEndTime()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a4a49eb8f5163b922653b8d4b9aca6428" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a4a49eb8f5163b922653b8d4b9aca6428"></a>

获取推送消息结束展示时间

#### `public inline void setPushTitle(String pushTitle)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1aa3eee468e703326f8f2e9ca674451766" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1aa3eee468e703326f8f2e9ca674451766"></a>

#### `public inline String getPushTitle()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1acb56e3a6a841169ac55a019f089b056c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1acb56e3a6a841169ac55a019f089b056c"></a>

获取推送消息标题

#### `public inline boolean isSilence()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a336c9e07d031a01e032db9096d78997e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a336c9e07d031a01e032db9096d78997e"></a>

#### `public inline BMXMessageConfig.BadgeCountType getBadgeCountType()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a82ca55f42d56f7f9a6b161423321ed1d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a82ca55f42d56f7f9a6b161423321ed1d"></a>

#### `public inline int getBadgeCount(int count)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a6d685e81b3c0badef85435a2ce192112" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a6d685e81b3c0badef85435a2ce192112"></a>

#### `public inline String getUsername()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a41924e828858576260166e136cceacde" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a41924e828858576260166e136cceacde"></a>

获取消息发送者用户名

#### `public inline String serialize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a6934b7464b7109b05a5abfd88512a03e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a6934b7464b7109b05a5abfd88512a03e"></a>

序列化操作

**Returns**

std::string

#### `protected inline BMXMessageConfig(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a46f81359ab6d19643430a92146955afa" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a46f81359ab6d19643430a92146955afa"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a094febd541e9634d37bc4a6be0075b5f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_config_1a094febd541e9634d37bc4a6be0075b5f"></a>

## class `BMXBaseObject` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_base_object" id="classim_1_1floo_1_1floolib_1_1_b_m_x_base_object"></a>

### Summary

| Members                                                        | Descriptions |
| -------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                     |              |
| `public inline BMXBaseObject()`                                |              |
| `public inline boolean equals(Object o)`                       |              |
| `public inline int hashCode()`                                 |              |
| `protected transient boolean swigCMemOwn`                      |              |
| `protected inline BMXBaseObject(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                             |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_base_object_1a2cdce1357a1ea45ac87afa36a6e13dde" id="classim_1_1floo_1_1floolib_1_1_b_m_x_base_object_1a2cdce1357a1ea45ac87afa36a6e13dde"></a>

#### `public inline BMXBaseObject()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_base_object_1a25634d6343274693806540133025a0be" id="classim_1_1floo_1_1floolib_1_1_b_m_x_base_object_1a25634d6343274693806540133025a0be"></a>

#### `public inline boolean equals(Object o)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_base_object_1a05e97a6a807c7eaeb9f356f38a972295" id="classim_1_1floo_1_1floolib_1_1_b_m_x_base_object_1a05e97a6a807c7eaeb9f356f38a972295"></a>

#### `public inline int hashCode()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_base_object_1ad2f8ae24d87eea2ceae6f6941c6c61c9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_base_object_1ad2f8ae24d87eea2ceae6f6941c6c61c9"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_base_object_1a4b0254ebbcceaaf81dc53154d52fc2cf" id="classim_1_1floo_1_1floolib_1_1_b_m_x_base_object_1a4b0254ebbcceaaf81dc53154d52fc2cf"></a>

#### `protected inline BMXBaseObject(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_base_object_1ac9984d5574999f165137444004470412" id="classim_1_1floo_1_1floolib_1_1_b_m_x_base_object_1ac9984d5574999f165137444004470412"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_base_object_1ac10480d033839513def7db06ece97030" id="classim_1_1floo_1_1floolib_1_1_b_m_x_base_object_1ac10480d033839513def7db06ece97030"></a>

## class `BMXChatManager` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager"></a>

聊天管理器

### Summary

| Members                                                                                                                                                                                                             | Descriptions                                                          |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `public inline BMXChatManager(`[`BMXChatService`](broken-reference) `service)`                                                                                                                                      |                                                                       |
| `public inline void sendMessage(final` [`BMXMessage`](broken-reference) `msg)`                                                                                                                                      | 发送消息，消息状态变化会通过listener通知                                              |
| `public inline void resendMessage(final` [`BMXMessage`](broken-reference) `msg)`                                                                                                                                    | 重新发送消息，消息状态变化会通过listener通知                                            |
| `public inline void recallMessage(final` [`BMXMessage`](broken-reference) `msg)`                                                                                                                                    | 撤回消息，消息状态变化会通过listener通知                                              |
| `public inline void forwardMessage(final` [`BMXMessageList`](broken-reference)`list,final`[`BMXConversation`](broken-reference)`to,final`[`BMXMessage`](broken-reference) `newMsg,final BMXCallBack callBack)`      | 合并转发消息                                                                |
| `public inline void forwardMessage(final` [`BMXMessage`](broken-reference) `msg)`                                                                                                                                   | 简单转发消息，用户应当通过BMXMessage::createForwardMessage()先创建转发消息                |
| `public inline void readAllMessage(final` [`BMXMessage`](broken-reference) `msg)`                                                                                                                                   | 标记此消息及之前全部消息为已读，该消息同步到当前用户的所有设备                                       |
| `public inline void removeMessage(final` [`BMXMessage`](broken-reference) `msg,final boolean synchronize)`                                                                                                          | 删除此消息，该消息同步到当前用户的其它设备                                                 |
| `public inline void removeMessage(final` [`BMXMessage`](broken-reference) `msg)`                                                                                                                                    |                                                                       |
| `public inline void ackMessage(final` [`BMXMessage`](broken-reference) `msg)`                                                                                                                                       | 发送已读回执                                                                |
| `public inline void readCancel(final` [`BMXMessage`](broken-reference) `msg)`                                                                                                                                       | 设置未读                                                                  |
| `public inline void downloadThumbnail(final` [`BMXMessage`](broken-reference) `msg)`                                                                                                                                | 下载缩略图，下载状态变化和进度通过listener通知 缩略图生成策略，1 - 第三方服务器生成， 2 - 本地服务器生成，默认值是 1。 |
| `public inline void downloadAttachment(final` [`BMXMessage`](broken-reference) `msg)`                                                                                                                               | 下载附件，下载状态变化和进度通过listener通知                                            |
| `public inline void cancelDownloadAttachment(final` [`BMXMessage`](broken-reference) `msg)`                                                                                                                         | 取消下载附件                                                                |
| `public inline int transferingNum()`                                                                                                                                                                                | 正在上传或下载中的文件数                                                          |
| `public inline void insertMessages(final` [`BMXMessageList`](broken-reference) `list,final BMXCallBack callBack)`                                                                                                   | 插入消息                                                                  |
| `public inline void getMessage(final long msgId,final BMXDataCallBack<` [`BMXMessage`](broken-reference) `> callBack)`                                                                                              | 读取一条消息                                                                |
| `public inline void deleteConversation(final long conversationId,final Boolean sync)`                                                                                                                               | 删除会话                                                                  |
| `public inline void openConversation(final long conversationId,final BMXConversation.Type type,final boolean createIfNotExist,final BMXDataCallBack<` [`BMXConversation`](broken-reference) `> callBack)`           | 打开一个会话                                                                |
| `public inline void getAllConversations(final BMXDataCallBack<` [`BMXConversationList`](broken-reference) `> callBack)`                                                                                             | 获取所有会话                                                                |
| `public inline void getAllConversationsUnreadCount(final BMXDataCallBack< Integer > callBack)`                                                                                                                      | 获取所有会话的全部未读数（标记为屏蔽的个人和群组的未读数不统计在内）                                    |
| `public inline void retrieveHistoryMessages(final` [`BMXConversation`](broken-reference)`conversation,final long refMsgId,final long size,final BMXDataCallBack<`[`BMXMessageList`](broken-reference) `> callBack)` | 拉取历史消息                                                                |
| `public inline void searchMessages(final String keywords,final long refTime,final long size,final BMXConversation.Direction arg4,final BMXDataCallBack<` [`BMXMessageListList`](broken-reference) `> callBack)`     | 搜索消息                                                                  |
| `public inline void searchMessages(final String keywords,final long refTime,final long size,final BMXDataCallBack<` [`BMXMessageListList`](broken-reference) `> callBack)`                                          |                                                                       |
| `public inline void getGroupAckMessageUserIdList(final` [`BMXMessage`](broken-reference)`msg,final BMXDataCallBack<`[`ListOfLongLong`](broken-reference) `> callBack)`                                              | 获取发送的群组消息已读用户id列表                                                     |
| `public inline void addChatListener(`[`BMXChatServiceListener`](broken-reference) `listener)`                                                                                                                       | 添加聊天监听者                                                               |
| `public inline void removeChatListener(`[`BMXChatServiceListener`](broken-reference) `listener)`                                                                                                                    | 移除聊天监听者                                                               |

### Members

#### `public inline BMXChatManager(`[`BMXChatService`](broken-reference) `service)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a0140df50523b2c572cbfe3c2edc3beb8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a0140df50523b2c572cbfe3c2edc3beb8"></a>

#### `public inline void sendMessage(final` [`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1ac80af10a0095a9ea467f9287ccc0eefe" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1ac80af10a0095a9ea467f9287ccc0eefe"></a>

发送消息，消息状态变化会通过listener通知

**Parameters**

* `msg` 发送的消息

#### `public inline void resendMessage(final` [`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1ab66f5c37e4fdfdb63b0c89bfac412678" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1ab66f5c37e4fdfdb63b0c89bfac412678"></a>

重新发送消息，消息状态变化会通过listener通知

**Parameters**

* `msg` 重新发送的消息

#### `public inline void recallMessage(final` [`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a3e41fa93c30ce58dadd98badf4b5c2e4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a3e41fa93c30ce58dadd98badf4b5c2e4"></a>

撤回消息，消息状态变化会通过listener通知

**Parameters**

* `msg` 撤回的消息

#### `public inline void forwardMessage(final` [`BMXMessageList`](broken-reference)`list,final`[`BMXConversation`](broken-reference)`to,final`[`BMXMessage`](broken-reference) `newMsg,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a30fa31c2188efb80eda1b8a7cba5dc7c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a30fa31c2188efb80eda1b8a7cba5dc7c"></a>

合并转发消息

**Parameters**

* `list` 转发的消息列表
* `to` 消息被转发到的会话
* `newMsg` 转发的消息列表合并后生成的新的单条转发消息
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void forwardMessage(final` [`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a5e4c3c57986aa9e66b9321a98f1eee0a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a5e4c3c57986aa9e66b9321a98f1eee0a"></a>

简单转发消息，用户应当通过BMXMessage::createForwardMessage()先创建转发消息

**Parameters**

* `msg` 转发的消息

#### `public inline void readAllMessage(final` [`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a2cd9fffa73fe514c74126231c2c53823" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a2cd9fffa73fe514c74126231c2c53823"></a>

标记此消息及之前全部消息为已读，该消息同步到当前用户的所有设备

**Parameters**

* `msg` 需要标记为此消息以前全部消息为已读的消息

#### `public inline void removeMessage(final` [`BMXMessage`](broken-reference) `msg,final boolean synchronize)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a6dd47add156215b17f2bf3047a8dc910" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a6dd47add156215b17f2bf3047a8dc910"></a>

删除此消息，该消息同步到当前用户的其它设备

**Parameters**

* `msg` 需要删除的消息
* `synchronize` 是否同步到其它设备，不同步的情况下只会删除本地存储的该条消息

#### `public inline void removeMessage(final` [`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a533e03ecd1a7baa095140a1bd171b878" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a533e03ecd1a7baa095140a1bd171b878"></a>

#### `public inline void ackMessage(final` [`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1ae3260d929525c2c06241dba55ebf3c7b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1ae3260d929525c2c06241dba55ebf3c7b"></a>

发送已读回执

#### `public inline void readCancel(final` [`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1ac5bb1d75f936d7545d756142461a6298" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1ac5bb1d75f936d7545d756142461a6298"></a>

设置未读

#### `public inline void downloadThumbnail(final` [`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a71a137a660e4366a86b4ce68a93a9e1b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a71a137a660e4366a86b4ce68a93a9e1b"></a>

下载缩略图，下载状态变化和进度通过listener通知 缩略图生成策略，1 - 第三方服务器生成， 2 - 本地服务器生成，默认值是 1。

**Parameters**

* `msg` 需要下载缩略图的消息

#### `public inline void downloadAttachment(final` [`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a32b64366ca6ba95f7cbb71d28a0ea017" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a32b64366ca6ba95f7cbb71d28a0ea017"></a>

下载附件，下载状态变化和进度通过listener通知

**Parameters**

* `msg` 需要下载附件的消息

#### `public inline void cancelDownloadAttachment(final` [`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a6aed559b449e5cf30b1ba37a96f5ecb2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a6aed559b449e5cf30b1ba37a96f5ecb2"></a>

取消下载附件

**Parameters**

* `msg` 需要下载附件的消息

#### `public inline int transferingNum()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a7121808913d2180e261963747797e731" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a7121808913d2180e261963747797e731"></a>

正在上传或下载中的文件数

**Returns**

传输中的文件数

#### `public inline void insertMessages(final` [`BMXMessageList`](broken-reference) `list,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a92ae0b87f8526932ad0a7cefc0cc833d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a92ae0b87f8526932ad0a7cefc0cc833d"></a>

插入消息

**Parameters**

* `list` 插入消息列表
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void getMessage(final long msgId,final BMXDataCallBack<` [`BMXMessage`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1aa888a9ae76b085dd5a71daee19b59958" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1aa888a9ae76b085dd5a71daee19b59958"></a>

读取一条消息

**Parameters**

* `msgId` 需要获取消息的消息id
* `callBack` [BMXMessage](broken-reference)

#### `public inline void deleteConversation(final long conversationId,final Boolean sync)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1aa434d7416ae7a29918f6ab68c83c4abf" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1aa434d7416ae7a29918f6ab68c83c4abf"></a>

删除会话

**Parameters**

* `conversationId` 需要删除会话的会话id
* `sync` 是否同步删除其它设备该会话，默认为false，仅删除本设备会话

#### `public inline void openConversation(final long conversationId,final BMXConversation.Type type,final boolean createIfNotExist,final BMXDataCallBack<` [`BMXConversation`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a4291f5b61c6437e88c3d5dd0822eed18" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a4291f5b61c6437e88c3d5dd0822eed18"></a>

打开一个会话

**Parameters**

* `conversationId` 需要打开的会话的会话id
* `type` 会话的类型，单聊还是群聊。
* `createIfNotExist` 会话不存在的情况下是否要创建本地会话，默认为创建
* `callBack` [BMXConversation](broken-reference)

#### `public inline void getAllConversations(final BMXDataCallBack<` [`BMXConversationList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a08fc692a1107a8b0f4bfffc20b604069" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a08fc692a1107a8b0f4bfffc20b604069"></a>

获取所有会话

**Parameters**

* `callBack` [BMXConversationList](broken-reference)

#### `public inline void getAllConversationsUnreadCount(final BMXDataCallBack< Integer > callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1ae96ac844133cccc27e8086aaad5786dd" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1ae96ac844133cccc27e8086aaad5786dd"></a>

获取所有会话的全部未读数（标记为屏蔽的个人和群组的未读数不统计在内）

**Parameters**

* `callBack` 未读数

#### `public inline void retrieveHistoryMessages(final` [`BMXConversation`](broken-reference)`conversation,final long refMsgId,final long size,final BMXDataCallBack<`[`BMXMessageList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a67d74c772230829303dcadb1a224f555" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a67d74c772230829303dcadb1a224f555"></a>

拉取历史消息

**Parameters**

* `conversation` 需要拉取历史消息的会话
* `refMsgId` 拉取会话消息的起始消息Id
* `size` 拉取的最大消息条数
* `callBack` BMXErrorCode，拉取操作获取的消息列表

#### `public inline void searchMessages(final String keywords,final long refTime,final long size,final BMXConversation.Direction arg4,final BMXDataCallBack<` [`BMXMessageListList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a51b94ad5077ff81decff695bee8e1a79" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a51b94ad5077ff81decff695bee8e1a79"></a>

搜索消息

**Parameters**

* `keywords` 搜索的关键字
* `refTime` 搜索消息的起始时间
* `size` 搜索的最大消息条数
* `arg4` 消息搜索方向，默认（Direction::Up）是从更早的消息中搜索
* `callBack` BMXErrorCode，搜索到的消息结果列表

#### `public inline void searchMessages(final String keywords,final long refTime,final long size,final BMXDataCallBack<` [`BMXMessageListList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1aeaa250ddfc30158bea99ab34c83f8f6b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1aeaa250ddfc30158bea99ab34c83f8f6b"></a>

#### `public inline void getGroupAckMessageUserIdList(final` [`BMXMessage`](broken-reference)`msg,final BMXDataCallBack<`[`ListOfLongLong`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a5558d24c57808832f444f9e7f2c117b1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a5558d24c57808832f444f9e7f2c117b1"></a>

获取发送的群组消息已读用户id列表

**Parameters**

* `msg` 需要获取已读用户id列表的消息
* `callBack` [BMXErrorCode](broken-reference),对该条消息已读的用户id列表

#### `public inline void addChatListener(`[`BMXChatServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a753762bab4965ac58322a8632cc99bd8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a753762bab4965ac58322a8632cc99bd8"></a>

添加聊天监听者

**Parameters**

* `listener` 聊天监听者

#### `public inline void removeChatListener(`[`BMXChatServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a284cede37b4c6e552d37251311bb827f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_manager_1a284cede37b4c6e552d37251311bb827f"></a>

移除聊天监听者

**Parameters**

* `listener` 聊天监听者

## class `BMXChatService` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service"></a>

聊天Service

### Summary

| Members                                                                                                                                                                                                  | Descriptions                                                          |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `public inline synchronized void delete()`                                                                                                                                                               |                                                                       |
| `public inline void sendMessage(`[`BMXMessage`](broken-reference) `msg)`                                                                                                                                 | 发送消息，消息状态变化会通过listener通知                                              |
| `public inline void resendMessage(`[`BMXMessage`](broken-reference) `msg)`                                                                                                                               | 重新发送消息，消息状态变化会通过listener通知                                            |
| `public inline void recallMessage(`[`BMXMessage`](broken-reference) `msg)`                                                                                                                               | 撤回消息，消息状态变化会通过listener通知                                              |
| `public inline` [`BMXErrorCode`](broken-reference) `forwardMessage(`[`BMXMessageList`](broken-reference) `list,`[`BMXConversation`](broken-reference) `to,`[`BMXMessage`](broken-reference) `newMsg)`    | 合并转发消息                                                                |
| `public inline void forwardMessage(`[`BMXMessage`](broken-reference) `msg)`                                                                                                                              | 简单转发消息，用户应当通过BMXMessage::createForwardMessage()先创建转发消息                |
| `public inline void ackMessage(`[`BMXMessage`](broken-reference) `msg)`                                                                                                                                  | 发送已读回执                                                                |
| `public inline void ackMessageDelivered(`[`BMXMessage`](broken-reference) `msg)`                                                                                                                         | 发送送达回执                                                                |
| `public inline void ackPlayMessage(`[`BMXMessage`](broken-reference) `msg)`                                                                                                                              | 发送已播放回执                                                               |
| `public inline void readCancel(`[`BMXMessage`](broken-reference) `msg)`                                                                                                                                  | 标记此消息为未读，该消息同步到当前用户的所有设备                                              |
| `public inline void readAllMessage(`[`BMXMessage`](broken-reference) `msg)`                                                                                                                              | 标记此消息及之前全部消息为已读，该消息同步到当前用户的所有设备                                       |
| `public inline void removeMessage(`[`BMXMessage`](broken-reference) `msg,boolean synchronize)`                                                                                                           | 删除此消息，该消息同步到当前用户的其它设备                                                 |
| `public inline void removeMessage(`[`BMXMessage`](broken-reference) `msg)`                                                                                                                               |                                                                       |
| `public inline void downloadThumbnail(`[`BMXMessage`](broken-reference) `msg,BMXChatService.ThumbnailStrategy strategy)`                                                                                 | 下载缩略图，下载状态变化和进度通过listener通知 缩略图生成策略，1 - 第三方服务器生成， 2 - 本地服务器生成，默认值是 1。 |
| `public inline void downloadThumbnail(`[`BMXMessage`](broken-reference) `msg)`                                                                                                                           |                                                                       |
| `public inline void downloadAttachment(`[`BMXMessage`](broken-reference) `msg)`                                                                                                                          | 下载附件，下载状态变化和进度通过listener通知                                            |
| `public inline void downloadAttachmentByUrl(long msgId,String url,String path)`                                                                                                                          | 下载附件，下载状态变化和进度通过listener通知                                            |
| `public inline void cancelUploadAttachment(`[`BMXMessage`](broken-reference) `msg)`                                                                                                                      | 取消上传附件                                                                |
| `public inline void cancelDownloadAttachment(`[`BMXMessage`](broken-reference) `msg)`                                                                                                                    | 取消上传附件                                                                |
| `public inline int transferingNum()`                                                                                                                                                                     | 上传或下载中的文件数                                                            |
| `public inline` [`BMXErrorCode`](broken-reference) `insertMessages(`[`BMXMessageList`](broken-reference) `list)`                                                                                         | 插入消息                                                                  |
| `public inline` [`BMXMessage`](broken-reference) `getMessage(long msgId)`                                                                                                                                | 读取一条消息                                                                |
| `public inline void deleteConversation(long conversationId,boolean synchronize)`                                                                                                                         | 删除会话                                                                  |
| `public inline void deleteConversation(long conversationId)`                                                                                                                                             |                                                                       |
| `public inline` [`BMXConversation`](broken-reference) `openConversation(long conversationId,BMXConversation.Type type,boolean createIfNotExist)`                                                         | 打开一个会话                                                                |
| `public inline` [`BMXConversation`](broken-reference) `openConversation(long conversationId,BMXConversation.Type type)`                                                                                  |                                                                       |
| `public inline String attachmentDir()`                                                                                                                                                                   | 获取附件保存路径                                                              |
| `public inline String attachmentDirForConversation(long conversationId)`                                                                                                                                 | 获取会话的附件保存路径                                                           |
| `public inline` [`BMXConversationList`](broken-reference) `getAllConversations()`                                                                                                                        | 获取所有会话                                                                |
| `public inline int getAllConversationsUnreadCount()`                                                                                                                                                     | 获取所有会话的全部未读数（标记为屏蔽的个人和群组的未读数不统计在内）                                    |
| `public inline` [`BMXErrorCode`](broken-reference) `retrieveHistoryMessages(`[`BMXConversation`](broken-reference) `conversation,long refMsgId,long size,`[`BMXMessageList`](broken-reference) `result)` | 拉取历史消息                                                                |
| `public inline` [`BMXErrorCode`](broken-reference) `searchMessagesByKeyWords(String keywords,long refTime,long size,`[`BMXMessageListList`](broken-reference) `result,BMXConversation.Direction arg4)`   | 搜索消息                                                                  |
| `public inline` [`BMXErrorCode`](broken-reference) `searchMessagesByKeyWords(String keywords,long refTime,long size,`[`BMXMessageListList`](broken-reference) `result)`                                  |                                                                       |
| `public inline` [`BMXErrorCode`](broken-reference) `searchMessages(String keywords,long refTime,long size,`[`BMXMessageListList`](broken-reference) `result,BMXConversation.Direction arg4)`             | 搜索消息                                                                  |
| `public inline` [`BMXErrorCode`](broken-reference) `searchMessages(String keywords,long refTime,long size,`[`BMXMessageListList`](broken-reference) `result)`                                            |                                                                       |
| `public inline` [`BMXErrorCode`](broken-reference) `getGroupAckMessageUserIdList(`[`BMXMessage`](broken-reference) `msg,`[`ListOfLongLong`](broken-reference) `groupMemberIdList)`                       | 获取发送的群组消息已读用户id列表                                                     |
| `public inline` [`BMXErrorCode`](broken-reference) `getGroupAckMessageUnreadUserIdList(`[`BMXMessage`](broken-reference) `msg,`[`ListOfLongLong`](broken-reference) `groupMemberIdList)`                 | 获取发送的群组消息未读用户id列表                                                     |
| `public inline` [`BMXErrorCode`](broken-reference) `getGroupPlayAckMessageUserIdList(`[`BMXMessage`](broken-reference) `msg,`[`ListOfLongLong`](broken-reference) `groupMemberIdList)`                   | 获取发送的群组消息已播放用户id列表                                                    |
| `public inline` [`BMXErrorCode`](broken-reference) `getGroupUnPlayAckMessageUserIdList(`[`BMXMessage`](broken-reference) `msg,`[`ListOfLongLong`](broken-reference) `groupMemberIdList)`                 | 获取发送的群组消息未播放用户id列表                                                    |
| `public inline void addChatListener(`[`BMXChatServiceListener`](broken-reference) `listener)`                                                                                                            | 添加聊天监听者                                                               |
| `public inline void removeChatListener(`[`BMXChatServiceListener`](broken-reference) `listener)`                                                                                                         | 移除聊天监听者                                                               |
| `protected transient boolean swigCMemOwn`                                                                                                                                                                |                                                                       |
| `protected inline BMXChatService(long cPtr,boolean cMemoryOwn)`                                                                                                                                          |                                                                       |
| `protected inline void finalize()`                                                                                                                                                                       |                                                                       |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a894ef7b461868dc7fb257279f5e38dd0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a894ef7b461868dc7fb257279f5e38dd0"></a>

#### `public inline void sendMessage(`[`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a82648ee73c176918237b7041f8cffe8b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a82648ee73c176918237b7041f8cffe8b"></a>

发送消息，消息状态变化会通过listener通知

**Parameters**

* `msg` 发送的消息

#### `public inline void resendMessage(`[`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1ad816525c6a08b4b3f8f2ab22236376c5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1ad816525c6a08b4b3f8f2ab22236376c5"></a>

重新发送消息，消息状态变化会通过listener通知

**Parameters**

* `msg` 重新发送的消息

#### `public inline void recallMessage(`[`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1af061f80d1538aa3bb9c0b8cef7707190" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1af061f80d1538aa3bb9c0b8cef7707190"></a>

撤回消息，消息状态变化会通过listener通知

**Parameters**

* `msg` 撤回的消息

#### `public inline` [`BMXErrorCode`](broken-reference) `forwardMessage(`[`BMXMessageList`](broken-reference) `list,`[`BMXConversation`](broken-reference) `to,`[`BMXMessage`](broken-reference) `newMsg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a3b6a26bdc6503e7b70505fec0d264328" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a3b6a26bdc6503e7b70505fec0d264328"></a>

合并转发消息

**Parameters**

* `list` 转发的消息列表
* `to` 消息被转发到的会话
* `newMsg` 转发的消息列表合并后生成的新的单条转发消息

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline void forwardMessage(`[`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a2249d0409a7b7c98243d92583b2e326e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a2249d0409a7b7c98243d92583b2e326e"></a>

简单转发消息，用户应当通过BMXMessage::createForwardMessage()先创建转发消息

**Parameters**

* `msg` 转发的消息

#### `public inline void ackMessage(`[`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a431689b08677be5dd54f678c0f3a70d1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a431689b08677be5dd54f678c0f3a70d1"></a>

发送已读回执

**Parameters**

* `msg` 需要发送已读回执的消息

#### `public inline void ackMessageDelivered(`[`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a987a62c7da222881605998766d6e0de8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a987a62c7da222881605998766d6e0de8"></a>

发送送达回执

**Parameters**

* `msg` 需要发送送达回执的消息

#### `public inline void ackPlayMessage(`[`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1abd7120c7be7254be2ec93cb50f63f84c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1abd7120c7be7254be2ec93cb50f63f84c"></a>

发送已播放回执

**Parameters**

* `msg` 需要发送已读回播放的消息

#### `public inline void readCancel(`[`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a6418b5551921359be7dce4a210a303c2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a6418b5551921359be7dce4a210a303c2"></a>

标记此消息为未读，该消息同步到当前用户的所有设备

**Parameters**

* `msg` 需要发送消息已读取消的消息

#### `public inline void readAllMessage(`[`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a9b064365da01497a26dfb410358a3429" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a9b064365da01497a26dfb410358a3429"></a>

标记此消息及之前全部消息为已读，该消息同步到当前用户的所有设备

**Parameters**

* `msg` 需要标记为此消息以前全部消息为已读的消息

#### `public inline void removeMessage(`[`BMXMessage`](broken-reference) `msg,boolean synchronize)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a8135df0b850024109c7433dda12070eb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a8135df0b850024109c7433dda12070eb"></a>

删除此消息，该消息同步到当前用户的其它设备

**Parameters**

* `msg` 需要删除的消息
* `synchronize` 是否同步到其它设备，不同步的情况下只会删除本地存储的该条消息

#### `public inline void removeMessage(`[`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1ac5b56f2d202dfb788aa7fae84f430739" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1ac5b56f2d202dfb788aa7fae84f430739"></a>

#### `public inline void downloadThumbnail(`[`BMXMessage`](broken-reference) `msg,BMXChatService.ThumbnailStrategy strategy)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1af8e3a245002dcbe0505ec6ce344445a4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1af8e3a245002dcbe0505ec6ce344445a4"></a>

下载缩略图，下载状态变化和进度通过listener通知 缩略图生成策略，1 - 第三方服务器生成， 2 - 本地服务器生成，默认值是 1。

**Parameters**

* `msg` 需要下载缩略图的消息
* `strategy` 缩略图生成策略，1 - 第三方服务器生成， 2 - 本地服务器生成，默认值是 1。

#### `public inline void downloadThumbnail(`[`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a71b1376ffa2e9f22c0e8d7a37b7f320b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a71b1376ffa2e9f22c0e8d7a37b7f320b"></a>

#### `public inline void downloadAttachment(`[`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a71b8ddcb5bf27ae47e186a1844983e79" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a71b8ddcb5bf27ae47e186a1844983e79"></a>

下载附件，下载状态变化和进度通过listener通知

**Parameters**

* `msg` 需要下载附件的消息

#### `public inline void downloadAttachmentByUrl(long msgId,String url,String path)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a27bd1d00ccb6eeb6b046b5a92b8843d8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a27bd1d00ccb6eeb6b046b5a92b8843d8"></a>

下载附件，下载状态变化和进度通过listener通知

**Parameters**

* `msgId` 需要下载附件的消息
* `url` 文件远程地址
* `path` 文件本地路径

#### `public inline void cancelUploadAttachment(`[`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1acc4c15fe45baf05fe1db6b4eeef1a338" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1acc4c15fe45baf05fe1db6b4eeef1a338"></a>

取消上传附件

**Parameters**

* `msg` 需要取消上传附件的消息

#### `public inline void cancelDownloadAttachment(`[`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1ad7960acb19b0103c98b0fdda40f619ab" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1ad7960acb19b0103c98b0fdda40f619ab"></a>

取消上传附件

**Parameters**

* `msg` 需要取消上传附件的消息

#### `public inline int transferingNum()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1ab5ad5ae8a13fab995926fd61c9c74de1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1ab5ad5ae8a13fab995926fd61c9c74de1"></a>

上传或下载中的文件数

**Returns**

文件数

#### `public inline` [`BMXErrorCode`](broken-reference) `insertMessages(`[`BMXMessageList`](broken-reference) `list)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1adf2dbecadba236c5f781ca34685098fd" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1adf2dbecadba236c5f781ca34685098fd"></a>

插入消息

**Parameters**

* `list` 插入消息列表

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXMessage`](broken-reference) `getMessage(long msgId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1aa55f868c85d657af63d9a3838c30396a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1aa55f868c85d657af63d9a3838c30396a"></a>

读取一条消息

**Parameters**

* `msgId` 需要获取消息的消息id

**Returns**

[BMXMessage](broken-reference)

#### `public inline void deleteConversation(long conversationId,boolean synchronize)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1af1235c5c0e54ffc5b80f5a8721797d85" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1af1235c5c0e54ffc5b80f5a8721797d85"></a>

删除会话

**Parameters**

* `conversationId` 需要删除会话的会话id
* `synchronize` 是否同步删除其它设备该会话，默认为false，仅删除本设备会话

#### `public inline void deleteConversation(long conversationId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a0dd82b7017e1f4c7afdb6f6fc02fdcbe" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a0dd82b7017e1f4c7afdb6f6fc02fdcbe"></a>

#### `public inline` [`BMXConversation`](broken-reference) `openConversation(long conversationId,BMXConversation.Type type,boolean createIfNotExist)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a0d762f1a3d5ca894ba9fee8f9fc01848" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a0d762f1a3d5ca894ba9fee8f9fc01848"></a>

打开一个会话

**Parameters**

* `conversationId` 需要打开的会话的会话id
* `type` 会话的类型，单聊还是群聊。
* `createIfNotExist` 会话不存在的情况下是否要创建本地会话，默认为创建

**Returns**

[BMXConversation](broken-reference)

#### `public inline` [`BMXConversation`](broken-reference) `openConversation(long conversationId,BMXConversation.Type type)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1ac7570afa9c990d8da42928678dc2c00c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1ac7570afa9c990d8da42928678dc2c00c"></a>

#### `public inline String attachmentDir()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a735f4ffb29bfbce2cbf7b64c002e970e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a735f4ffb29bfbce2cbf7b64c002e970e"></a>

获取附件保存路径

**Returns**

std::string

#### `public inline String attachmentDirForConversation(long conversationId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1aa2d69dcbc3282e0faed5ff4f8cdc6649" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1aa2d69dcbc3282e0faed5ff4f8cdc6649"></a>

获取会话的附件保存路径

**Parameters**

* `conversationId` 需要获取会话附件路径的会话id

**Returns**

std::string

#### `public inline` [`BMXConversationList`](broken-reference) `getAllConversations()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a4b9ffee3d1cfbf00de1065432054e11b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a4b9ffee3d1cfbf00de1065432054e11b"></a>

获取所有会话

**Returns**

[BMXConversationList](broken-reference)

#### `public inline int getAllConversationsUnreadCount()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1ab1c1cd63faa94d0883bc1209956f997a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1ab1c1cd63faa94d0883bc1209956f997a"></a>

获取所有会话的全部未读数（标记为屏蔽的个人和群组的未读数不统计在内）

**Returns**

int

#### `public inline` [`BMXErrorCode`](broken-reference) `retrieveHistoryMessages(`[`BMXConversation`](broken-reference) `conversation,long refMsgId,long size,`[`BMXMessageList`](broken-reference) `result)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a5ec4720ad96bd9ea91974cb03112f203" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a5ec4720ad96bd9ea91974cb03112f203"></a>

拉取历史消息

**Parameters**

* `conversation` 需要拉取历史消息的会话
* `refMsgId` 拉取会话消息的起始消息Id
* `size` 拉取的最大消息条数
* `result` 拉取操作获取的消息列表，外部初始化传入空列表。

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `searchMessagesByKeyWords(String keywords,long refTime,long size,`[`BMXMessageListList`](broken-reference) `result,BMXConversation.Direction arg4)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a1bf353ad2470e16368b98416a50ec308" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a1bf353ad2470e16368b98416a50ec308"></a>

搜索消息

**Parameters**

* `keywords` 搜索的关键字
* `refTime` 搜索消息的起始时间
* `size` 搜索的最大消息条数
* `result` 搜索到的消息结果列表，外部初始化传入空列表。
* `arg4` 消息搜索方向，默认（Direction::Up）是从更早的消息中搜索

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `searchMessagesByKeyWords(String keywords,long refTime,long size,`[`BMXMessageListList`](broken-reference) `result)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a55884e1af95e5459aaf4d9331b2c6e8a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a55884e1af95e5459aaf4d9331b2c6e8a"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `searchMessages(String keywords,long refTime,long size,`[`BMXMessageListList`](broken-reference) `result,BMXConversation.Direction arg4)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1aa0aad57ebc779d23277796987ee76c88" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1aa0aad57ebc779d23277796987ee76c88"></a>

搜索消息

**Parameters**

* `keywords` 搜索的关键字
* `refTime` 搜索消息的起始时间
* `size` 搜索的最大消息条数
* `result` 搜索到的消息结果列表，外部初始化传入空列表。
* `arg4` 消息搜索方向，默认（Direction::Up）是从更早的消息中搜索

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `searchMessages(String keywords,long refTime,long size,`[`BMXMessageListList`](broken-reference) `result)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1aade7363f9229185a9080d77cc59c0f79" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1aade7363f9229185a9080d77cc59c0f79"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `getGroupAckMessageUserIdList(`[`BMXMessage`](broken-reference) `msg,`[`ListOfLongLong`](broken-reference) `groupMemberIdList)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a404cd1bc0d6cb7bfe7035f3e03d14ea6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a404cd1bc0d6cb7bfe7035f3e03d14ea6"></a>

获取发送的群组消息已读用户id列表

**Parameters**

* `msg` 需要获取已读用户id列表的消息
* `groupMemberIdList` 对该条消息已读的用户id列表，初始传入为空列表

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getGroupAckMessageUnreadUserIdList(`[`BMXMessage`](broken-reference) `msg,`[`ListOfLongLong`](broken-reference) `groupMemberIdList)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a79e692b94a4d3465188f329b25565cca" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a79e692b94a4d3465188f329b25565cca"></a>

获取发送的群组消息未读用户id列表

**Parameters**

* `msg` 需要获取未读用户id列表的消息
* `groupMemberIdList` 对该条消息未读的用户id列表，初始传入为空列表

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getGroupPlayAckMessageUserIdList(`[`BMXMessage`](broken-reference) `msg,`[`ListOfLongLong`](broken-reference) `groupMemberIdList)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1ab873bd32ab82b72d69a7dd001732dc80" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1ab873bd32ab82b72d69a7dd001732dc80"></a>

获取发送的群组消息已播放用户id列表

**Parameters**

* `msg` 需要获取已播放用户id列表的消息
* `groupMemberIdList` 对该条消息已播放的用户id列表，初始传入为空列表

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getGroupUnPlayAckMessageUserIdList(`[`BMXMessage`](broken-reference) `msg,`[`ListOfLongLong`](broken-reference) `groupMemberIdList)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1aee3211242e7c91dbf0509388181f4e5d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1aee3211242e7c91dbf0509388181f4e5d"></a>

获取发送的群组消息未播放用户id列表

**Parameters**

* `msg` 需要获取未播放用户id列表的消息
* `groupMemberIdList` 对该条消息未播放的用户id列表，初始传入为空列表

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline void addChatListener(`[`BMXChatServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1afee3b74dcf8a981539a4ef14cddc79ff" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1afee3b74dcf8a981539a4ef14cddc79ff"></a>

添加聊天监听者

**Parameters**

* `listener` 聊天监听者

#### `public inline void removeChatListener(`[`BMXChatServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1ab644b22764cab36906c4af960d30ef0e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1ab644b22764cab36906c4af960d30ef0e"></a>

移除聊天监听者

**Parameters**

* `listener` 聊天监听者

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a67bfbafb25662876cace9f325132b303" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a67bfbafb25662876cace9f325132b303"></a>

#### `protected inline BMXChatService(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a0ea391a1e45b337c076778f6b0964f8e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a0ea391a1e45b337c076778f6b0964f8e"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a8c8a4198d6a430997feba6f1fcccc002" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_1a8c8a4198d6a430997feba6f1fcccc002"></a>

## class `BMXChatServiceListener` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener"></a>

聊天监听者

### Summary

| Members                                                                                                                                       | Descriptions                  |
| --------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------- |
| `public inline synchronized void delete()`                                                                                                    |                               |
| `public inline void swigReleaseOwnership()`                                                                                                   |                               |
| `public inline void swigTakeOwnership()`                                                                                                      |                               |
| `public inline void onStatusChanged(`[`BMXMessage`](broken-reference) `msg,`[`BMXErrorCode`](broken-reference) `error)`                       | 消息发送状态发生变化                    |
| `public inline void onAttachmentUploadProgressChanged(`[`BMXMessage`](broken-reference) `msg,int percent)`                                    | 附件上传进度发送变化                    |
| `public inline void onRecallStatusChanged(`[`BMXMessage`](broken-reference) `msg,`[`BMXErrorCode`](broken-reference) `error)`                 | 消息撤回状态发送变化                    |
| `public inline void onReceive(`[`BMXMessageList`](broken-reference) `list)`                                                                   | 收到消息                          |
| `public inline void onReceiveCommandMessages(`[`BMXMessageList`](broken-reference) `list)`                                                    | 收到命令消息                        |
| `public inline void onReceiveSystemMessages(`[`BMXMessageList`](broken-reference) `list)`                                                     | 收到系统通知消息                      |
| `public inline void onReceiveReadAcks(`[`BMXMessageList`](broken-reference) `list)`                                                           | 收到消息已读回执                      |
| `public inline void onReceiveDeliverAcks(`[`BMXMessageList`](broken-reference) `list)`                                                        | 收到消息已送达回执                     |
| `public inline void onReceiveRecallMessages(`[`BMXMessageList`](broken-reference) `list)`                                                     | 收到撤回消息                        |
| `public inline void onReceiveReadCancels(`[`BMXMessageList`](broken-reference) `list)`                                                        | 收到消息已读取消（多设备其他设备同步消息已读状态变为未读） |
| `public inline void onReceiveReadAllMessages(`[`BMXMessageList`](broken-reference) `list)`                                                    | 收到消息全部已读（多设备同步某消息之前消息全部设置为已读） |
| `public inline void onReceiveDeleteMessages(`[`BMXMessageList`](broken-reference) `list)`                                                     | 收到删除消息 （多设备同步删除消息）            |
| `public inline void onReceivePlayAcks(`[`BMXMessageList`](broken-reference) `list)`                                                           | 收到消息已播放回执                     |
| `public inline void onAttachmentStatusChanged(`[`BMXMessage`](broken-reference) `msg,`[`BMXErrorCode`](broken-reference) `error,int percent)` | 附件下载状态发生变化                    |
| `public inline void onAttachmentDownloadByUrlStatusChanged(long msgId,`[`BMXErrorCode`](broken-reference) `error,int percent)`                | 附件下载状态发生变化                    |
| `public inline void onRetrieveHistoryMessages(`[`BMXConversation`](broken-reference) `conversation)`                                          | 拉取历史消息                        |
| `public inline void onLoadAllConversation()`                                                                                                  | 已经加载完未读会话列表                   |
| `public inline void onConversationCreate(`[`BMXConversation`](broken-reference) `conversation,`[`BMXMessage`](broken-reference) `msg)`        | 本地创建新会话                       |
| `public inline void onConversationDelete(long conversationId,`[`BMXErrorCode`](broken-reference) `error)`                                     | 删除会话                          |
| `public inline void onTotalUnreadCountChanged(int unreadCount)`                                                                               | 更新总未读数                        |
| `public inline BMXChatServiceListener()`                                                                                                      |                               |
| `public inline void registerChatService(`[`BMXChatService`](broken-reference) `service)`                                                      |                               |
| `protected transient boolean swigCMemOwn`                                                                                                     |                               |
| `protected inline BMXChatServiceListener(long cPtr,boolean cMemoryOwn)`                                                                       |                               |
| `protected inline void finalize()`                                                                                                            |                               |
| `protected inline void swigDirectorDisconnect()`                                                                                              |                               |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a1e7aef6a19593930a5bd678b2b50152e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a1e7aef6a19593930a5bd678b2b50152e"></a>

#### `public inline void swigReleaseOwnership()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a1f2ef9354d476c2863ce6ba742f4e2c7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a1f2ef9354d476c2863ce6ba742f4e2c7"></a>

#### `public inline void swigTakeOwnership()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a82f30bba2963f3f702a3caea1c8c7718" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a82f30bba2963f3f702a3caea1c8c7718"></a>

#### `public inline void onStatusChanged(`[`BMXMessage`](broken-reference) `msg,`[`BMXErrorCode`](broken-reference) `error)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a0f2cd4082548f9fb383001202524606b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a0f2cd4082548f9fb383001202524606b"></a>

消息发送状态发生变化

**Parameters**

* `msg` 发生状态变化的消息
* `error` 状态错误码

#### `public inline void onAttachmentUploadProgressChanged(`[`BMXMessage`](broken-reference) `msg,int percent)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1ac9d5b8d1a4500dedbef07d2b43ae214e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1ac9d5b8d1a4500dedbef07d2b43ae214e"></a>

附件上传进度发送变化

**Parameters**

* `msg` 上传附件的消息
* `percent` 附件上传的进度

#### `public inline void onRecallStatusChanged(`[`BMXMessage`](broken-reference) `msg,`[`BMXErrorCode`](broken-reference) `error)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a346899f6d59d854e5ed6dc317dae7604" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a346899f6d59d854e5ed6dc317dae7604"></a>

消息撤回状态发送变化

**Parameters**

* `msg` 撤回状态发生变化的消息
* `error` 状态错误码

#### `public inline void onReceive(`[`BMXMessageList`](broken-reference) `list)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a33d4900b09b552095c99951a4755d8cb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a33d4900b09b552095c99951a4755d8cb"></a>

收到消息

**Parameters**

* `list` 接收到的消息列表

#### `public inline void onReceiveCommandMessages(`[`BMXMessageList`](broken-reference) `list)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a58fd3759d17f7505997efd471872b009" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a58fd3759d17f7505997efd471872b009"></a>

收到命令消息

**Parameters**

* `list` 接收到的消息列表

#### `public inline void onReceiveSystemMessages(`[`BMXMessageList`](broken-reference) `list)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a84f91bc8a9c819e3b0cf737e93692ff4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a84f91bc8a9c819e3b0cf737e93692ff4"></a>

收到系统通知消息

**Parameters**

* `list` 接收到的系统消息列表

#### `public inline void onReceiveReadAcks(`[`BMXMessageList`](broken-reference) `list)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a82b270de53f70cdcc62c15ecb09d83f3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a82b270de53f70cdcc62c15ecb09d83f3"></a>

收到消息已读回执

**Parameters**

* `list` 接收到的已读回执消息列表

#### `public inline void onReceiveDeliverAcks(`[`BMXMessageList`](broken-reference) `list)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a4346696ebb658d21e2836692b31e236e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a4346696ebb658d21e2836692b31e236e"></a>

收到消息已送达回执

**Parameters**

* `list` 接收到的已送达回执消息列表

#### `public inline void onReceiveRecallMessages(`[`BMXMessageList`](broken-reference) `list)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a4818849bfba9c114c675eb7f87adf574" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a4818849bfba9c114c675eb7f87adf574"></a>

收到撤回消息

**Parameters**

* `list` 接收到的撤回消息列表

#### `public inline void onReceiveReadCancels(`[`BMXMessageList`](broken-reference) `list)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1aa53cbbde4491060d6d6124d410bb78e0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1aa53cbbde4491060d6d6124d410bb78e0"></a>

收到消息已读取消（多设备其他设备同步消息已读状态变为未读）

**Parameters**

* `list` 接收到的消息已读取消消息列表

#### `public inline void onReceiveReadAllMessages(`[`BMXMessageList`](broken-reference) `list)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1afdb0bf47ab3f291cf515a073a82a7053" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1afdb0bf47ab3f291cf515a073a82a7053"></a>

收到消息全部已读（多设备同步某消息之前消息全部设置为已读）

**Parameters**

* `list` 接收到的消息全部已读消息列表

#### `public inline void onReceiveDeleteMessages(`[`BMXMessageList`](broken-reference) `list)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1abfb2cc7121e08c356fe51621b5e821e7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1abfb2cc7121e08c356fe51621b5e821e7"></a>

收到删除消息 （多设备同步删除消息）

**Parameters**

* `list` 接收到的删除消息列表

#### `public inline void onReceivePlayAcks(`[`BMXMessageList`](broken-reference) `list)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a0c7c3931cffac4118386978d18e4283e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a0c7c3931cffac4118386978d18e4283e"></a>

收到消息已播放回执

**Parameters**

* `list` 接收到的已读回执消息列表

#### `public inline void onAttachmentStatusChanged(`[`BMXMessage`](broken-reference) `msg,`[`BMXErrorCode`](broken-reference) `error,int percent)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a10e204bcce4e75da22eb7ee5751d1f53" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a10e204bcce4e75da22eb7ee5751d1f53"></a>

附件下载状态发生变化

**Parameters**

* `msg` 发生下载状态变化的消息
* `error` 状态错误码
* `percent` 附件下载的进度

#### `public inline void onAttachmentDownloadByUrlStatusChanged(long msgId,`[`BMXErrorCode`](broken-reference) `error,int percent)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a2e83c66e6bd2ee5d29390c20d93e801b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a2e83c66e6bd2ee5d29390c20d93e801b"></a>

附件下载状态发生变化

**Parameters**

* `msgId` 发生下载状态变化的消息ID
* `error` 状态错误码
* `percent` 附件下载的进度

#### `public inline void onRetrieveHistoryMessages(`[`BMXConversation`](broken-reference) `conversation)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a7543db6c25e9a87dff383883e8b11ad3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a7543db6c25e9a87dff383883e8b11ad3"></a>

拉取历史消息

**Parameters**

* `conversation` 发生了拉取指历史消息的会话

#### `public inline void onLoadAllConversation()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a02bd5006c088cb7018debbcc494f28b8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a02bd5006c088cb7018debbcc494f28b8"></a>

已经加载完未读会话列表

#### `public inline void onConversationCreate(`[`BMXConversation`](broken-reference) `conversation,`[`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a53426e3ad28d79a1d04643c147d64a11" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a53426e3ad28d79a1d04643c147d64a11"></a>

本地创建新会话

**Parameters**

* `conversation` 新创建的本地会话
* `msg` 会话的最新消息，存在返回不存在返回为空

#### `public inline void onConversationDelete(long conversationId,`[`BMXErrorCode`](broken-reference) `error)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a9b1f2ee05b4c399d29f9c0458aef8c93" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a9b1f2ee05b4c399d29f9c0458aef8c93"></a>

删除会话

**Parameters**

* `conversationId` 删除的本地会话id
* `error` 状态错误码

#### `public inline void onTotalUnreadCountChanged(int unreadCount)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1aebdebd60d3a29dfc69533102a111f1f2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1aebdebd60d3a29dfc69533102a111f1f2"></a>

更新总未读数

**Parameters**

* `unreadCount` 本地全部会话未读总数

#### `public inline BMXChatServiceListener()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a9d9b8c5f664756924c83a4796a783255" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a9d9b8c5f664756924c83a4796a783255"></a>

#### `public inline void registerChatService(`[`BMXChatService`](broken-reference) `service)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a02cfca3b747eb512431eafd4a5aa3962" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a02cfca3b747eb512431eafd4a5aa3962"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a39c2a108eaccd77fe7b48af49c4d8969" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a39c2a108eaccd77fe7b48af49c4d8969"></a>

#### `protected inline BMXChatServiceListener(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a22547183addf9111dd867a8a1bbc79df" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a22547183addf9111dd867a8a1bbc79df"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1ada6ca9efe242150bbb63d9dc6ce25825" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1ada6ca9efe242150bbb63d9dc6ce25825"></a>

#### `protected inline void swigDirectorDisconnect()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a1b5f74ac0786d37c7b532f46c213a0b5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_chat_service_listener_1a1b5f74ac0786d37c7b532f46c213a0b5"></a>

## class `BMXClient` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client"></a>

```
class BMXClient
  : public im.floo.floolib.BMXNetworkListener
```

客户端

### Summary

| Members                                                                                                                                                      | Descriptions                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------- |
| `public inline synchronized void delete()`                                                                                                                   |                                                                                                                 |
| `public inline` [`BMXSDKConfig`](broken-reference) `getSDKConfig()`                                                                                          | 获取SDK设置                                                                                                         |
| `public inline` [`BMXUserService`](broken-reference) `getUserService()`                                                                                      | 获取用户Service                                                                                                     |
| `public inline` [`BMXChatService`](broken-reference) `getChatService()`                                                                                      | 获取聊天Service                                                                                                     |
| `public inline` [`BMXGroupService`](broken-reference) `getGroupService()`                                                                                    | 获取群组Service                                                                                                     |
| `public inline` [`BMXRosterService`](broken-reference) `getRosterService()`                                                                                  | 获取好友Service                                                                                                     |
| `public inline` [`BMXPushService`](broken-reference) `getPushService()`                                                                                      | 获取推送Service                                                                                                     |
| `public inline` [`BMXUserManager`](broken-reference) `getUserManager()`                                                                                      | 获取用户Manager                                                                                                     |
| `public inline` [`BMXChatManager`](broken-reference) `getChatManager()`                                                                                      | 获取聊天Manager                                                                                                     |
| `public inline` [`BMXGroupManager`](broken-reference) `getGroupManager()`                                                                                    | 获取群组Manager                                                                                                     |
| `public inline` [`BMXRosterManager`](broken-reference) `getRosterManager()`                                                                                  | 获取好友Manager                                                                                                     |
| `public inline` [`BMXPushManager`](broken-reference) `getPushManager()`                                                                                      | 获取推送Manager                                                                                                     |
| `public inline` [`BMXErrorCode`](broken-reference) `signUpNewUser(String username,String password,`[`BMXUserProfile`](broken-reference) `bmxUserProfilePtr)` | 注册新用户，username和password是必填参数                                                                                    |
| `public inline` [`BMXErrorCode`](broken-reference) `signInByName(String name,String password)`                                                               | 通过用户名登录                                                                                                         |
| `public inline` [`BMXErrorCode`](broken-reference) `signInById(long arg0,String password)`                                                                   | 通过用户ID登录                                                                                                        |
| `public inline` [`BMXErrorCode`](broken-reference) `fastSignInByName(String name,String password)`                                                           | 通过用户名快速登录（要求之前成功登录过，登录速度较快）                                                                                     |
| `public inline` [`BMXErrorCode`](broken-reference) `fastSignInById(long uid,String password)`                                                                | 通过用户ID快速登录（要求之前成功登录过，登录速度较快）                                                                                    |
| `public inline` [`BMXErrorCode`](broken-reference) `signOut(long uid,boolean ignoreUnbindDevice)`                                                            | 退出登录                                                                                                            |
| `public inline` [`BMXErrorCode`](broken-reference) `signOut(long uid)`                                                                                       |                                                                                                                 |
| `public inline` [`BMXErrorCode`](broken-reference) `signOut()`                                                                                               |                                                                                                                 |
| `public inline` [`BMXConnectStatus`](broken-reference) `connectStatus()`                                                                                     | 获取当前和服务器的连接状态                                                                                                   |
| `public inline` [`BMXSignInStatus`](broken-reference) `signInStatus()`                                                                                       | 获取当前的登录状态                                                                                                       |
| `public inline void reconnect()`                                                                                                                             | 强制重新连接                                                                                                          |
| `public inline void onNetworkChanged(`[`BMXNetworkType`](broken-reference) `type,boolean reconnect)`                                                         | 处理网络状态发送变化                                                                                                      |
| `public inline void disconnect()`                                                                                                                            | 断开网络连接                                                                                                          |
| `public inline` [`BMXErrorCode`](broken-reference) `changeAppId(String appId,String appSecret)`                                                              | 更改SDK的appId，本操作会同时更新BMXConfig中的appId。                                                                           |
| `public inline` [`BMXErrorCode`](broken-reference) `changeAppId(String appId)`                                                                               | 更改SDK的appId，本操作会同时更新BMXConfig中的appId。                                                                           |
| `public inline` [`BMXErrorCode`](broken-reference) `initializeServerConfig(boolean isLocal)`                                                                 | 获取app的服务器网络配置，在初始化SDK之后登陆之前调用，可以提前获取服务器配置加快登陆速度。                                                                |
| `public inline void sendMessage(`[`BMXMessage`](broken-reference) `msg)`                                                                                     | 发送消息，消息状态变化会通过listener通知，在发送群组消息且指定的群组为开启群组已读回执的情况下， 该接口会自动获取群成员列表id并且填充到message config中去，无需客户端自己进行群组成员列表的填充操作。 |
| `protected inline BMXClient(long cPtr,boolean cMemoryOwn)`                                                                                                   |                                                                                                                 |
| `protected inline void finalize()`                                                                                                                           |                                                                                                                 |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a79240cbefb8e5b6f1bcda31cb33e4214" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a79240cbefb8e5b6f1bcda31cb33e4214"></a>

#### `public inline` [`BMXSDKConfig`](broken-reference) `getSDKConfig()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1aa33100f31e2a943e54a2bcb5dbcbc2a2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1aa33100f31e2a943e54a2bcb5dbcbc2a2"></a>

获取SDK设置

**Returns**

BMXSDKConfigPtr

#### `public inline` [`BMXUserService`](broken-reference) `getUserService()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1ae596845b930f2ac5dcf6ef6b4dfdb710" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1ae596845b930f2ac5dcf6ef6b4dfdb710"></a>

获取用户Service

**Returns**

[BMXUserService](broken-reference)

#### `public inline` [`BMXChatService`](broken-reference) `getChatService()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1af49596083d81afb1a656f994e630d98c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1af49596083d81afb1a656f994e630d98c"></a>

获取聊天Service

**Returns**

[BMXChatService](broken-reference)

#### `public inline` [`BMXGroupService`](broken-reference) `getGroupService()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a0bac1db6b2e15ce4cad0590825572cfe" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a0bac1db6b2e15ce4cad0590825572cfe"></a>

获取群组Service

**Returns**

[BMXGroupService](broken-reference)

#### `public inline` [`BMXRosterService`](broken-reference) `getRosterService()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a56d66c67100e8dade9785dcfa9b503ca" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a56d66c67100e8dade9785dcfa9b503ca"></a>

获取好友Service

**Returns**

[BMXRosterService](broken-reference)

#### `public inline` [`BMXPushService`](broken-reference) `getPushService()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a99bfb6a86f4f7625e933dfc330cd033a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a99bfb6a86f4f7625e933dfc330cd033a"></a>

获取推送Service

**Returns**

[BMXPushService](broken-reference)

#### `public inline` [`BMXUserManager`](broken-reference) `getUserManager()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a3cec1583c9a5a2aa756598309e9a8a09" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a3cec1583c9a5a2aa756598309e9a8a09"></a>

获取用户Manager

**Returns**

[BMXUserManager](broken-reference)

#### `public inline` [`BMXChatManager`](broken-reference) `getChatManager()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1ac582c3b19725b7f9934d6d9d1915fdce" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1ac582c3b19725b7f9934d6d9d1915fdce"></a>

获取聊天Manager

**Returns**

[BMXChatManager](broken-reference)

#### `public inline` [`BMXGroupManager`](broken-reference) `getGroupManager()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a7780da87833c08c852614de44b1da70d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a7780da87833c08c852614de44b1da70d"></a>

获取群组Manager

**Returns**

[BMXGroupManager](broken-reference)

#### `public inline` [`BMXRosterManager`](broken-reference) `getRosterManager()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a2f10b158d07d8845e4c02d9c88296e2b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a2f10b158d07d8845e4c02d9c88296e2b"></a>

获取好友Manager

**Returns**

[BMXRosterManager](broken-reference)

#### `public inline` [`BMXPushManager`](broken-reference) `getPushManager()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1ad6b303720557a1e1a6f26835b5242795" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1ad6b303720557a1e1a6f26835b5242795"></a>

获取推送Manager

**Returns**

[BMXPushManager](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `signUpNewUser(String username,String password,`[`BMXUserProfile`](broken-reference) `bmxUserProfilePtr)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1aaf2d725ad772f61240a744eed15cd77c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1aaf2d725ad772f61240a744eed15cd77c"></a>

注册新用户，username和password是必填参数

**Parameters**

* `username` 用户名
* `password` 用户密码
* `bmxUserProfilePtr` 注册成功后从该函数处获取新注册用户的Profile信息，初始传入指向为空的shared\_ptr对象即可。

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `signInByName(String name,String password)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1aeaa586e616dbce6df490261fecb9430d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1aeaa586e616dbce6df490261fecb9430d"></a>

通过用户名登录

**Parameters**

* `name` 用户名
* `password` 用户密码

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `signInById(long arg0,String password)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a969d5aacddcbe4941df3840a1f9d8caf" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a969d5aacddcbe4941df3840a1f9d8caf"></a>

通过用户ID登录

**Parameters**

* `arg0` 用户id
* `password` 用户密码

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `fastSignInByName(String name,String password)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a7241f0c5e19a880f158387f7cb871b6c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a7241f0c5e19a880f158387f7cb871b6c"></a>

通过用户名快速登录（要求之前成功登录过，登录速度较快）

**Parameters**

* `name` 用户名
* `password` 用户密码(用于sdk在内部token到期时自动更新用户token)

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `fastSignInById(long uid,String password)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1aed26bfe75460472cc42e7c49c78d7b18" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1aed26bfe75460472cc42e7c49c78d7b18"></a>

通过用户ID快速登录（要求之前成功登录过，登录速度较快）

**Parameters**

* `uid` 用户id
* `password` 用户密码(用于sdk在内部token到期时自动更新用户token)

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `signOut(long uid,boolean ignoreUnbindDevice)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a46fb6009994783aa52fcff91e306ef0e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a46fb6009994783aa52fcff91e306ef0e"></a>

退出登录

**Parameters**

* `uid` 退出用户的uid（默认输入0则退出当前登陆用户）
* `ignoreUnbindDevice` 用户退出时是否忽略解绑定设备操作。对应某些服务器不可访问的情况下忽略服务器解绑定设备操作直接强制退出时设置为true

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `signOut(long uid)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a3e63ffda0180a5756eb080a86b51f903" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a3e63ffda0180a5756eb080a86b51f903"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `signOut()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a2eede9a5e25b0cb535baad5dbaf57dd4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a2eede9a5e25b0cb535baad5dbaf57dd4"></a>

#### `public inline` [`BMXConnectStatus`](broken-reference) `connectStatus()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1af0dc29d7646c63b85537fe89c1591b57" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1af0dc29d7646c63b85537fe89c1591b57"></a>

获取当前和服务器的连接状态

**Returns**

[BMXConnectStatus](broken-reference)

#### `public inline` [`BMXSignInStatus`](broken-reference) `signInStatus()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1ac30292fc9fc90e6dda892d954eade9b4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1ac30292fc9fc90e6dda892d954eade9b4"></a>

获取当前的登录状态

**Returns**

[BMXSignInStatus](broken-reference)

#### `public inline void reconnect()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a94a91c531f7bd088f73399ffd19a7f05" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a94a91c531f7bd088f73399ffd19a7f05"></a>

强制重新连接

#### `public inline void onNetworkChanged(`[`BMXNetworkType`](broken-reference) `type,boolean reconnect)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1aff9b29220c89450b59ed8bf69a666c21" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1aff9b29220c89450b59ed8bf69a666c21"></a>

处理网络状态发送变化

**Parameters**

* `type` 变化后的网络类型
* `reconnect` 网络是否需要重连

#### `public inline void disconnect()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1ab1f55b3c80b61f7a79b968b78c767bd7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1ab1f55b3c80b61f7a79b968b78c767bd7"></a>

断开网络连接

#### `public inline` [`BMXErrorCode`](broken-reference) `changeAppId(String appId,String appSecret)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1aa8e17c4bc5c644c9090cf050860107d2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1aa8e17c4bc5c644c9090cf050860107d2"></a>

更改SDK的appId，本操作会同时更新BMXConfig中的appId。

**Parameters**

* `appId` 新变更的appId
* `appSecret` 新变更的appSecret

#### `public inline` [`BMXErrorCode`](broken-reference) `changeAppId(String appId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1ac8b2ab9c190a1c7063f770a6e4575175" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1ac8b2ab9c190a1c7063f770a6e4575175"></a>

更改SDK的appId，本操作会同时更新BMXConfig中的appId。

**Parameters**

* `appId` 新变更的appId

#### `public inline` [`BMXErrorCode`](broken-reference) `initializeServerConfig(boolean isLocal)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1ac349ce1e224bb5f550496697da947a46" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1ac349ce1e224bb5f550496697da947a46"></a>

获取app的服务器网络配置，在初始化SDK之后登陆之前调用，可以提前获取服务器配置加快登陆速度。

**Parameters**

* `isLocal` 为true则使用本地缓存的dns配置，为false则从服务器获取最新的配置。

#### `public inline void sendMessage(`[`BMXMessage`](broken-reference) `msg)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1af1f9006392fa5cf3fa535d6e1f327f8d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1af1f9006392fa5cf3fa535d6e1f327f8d"></a>

发送消息，消息状态变化会通过listener通知，在发送群组消息且指定的群组为开启群组已读回执的情况下， 该接口会自动获取群成员列表id并且填充到message config中去，无需客户端自己进行群组成员列表的填充操作。

**Parameters**

* `msg` 发送的消息

#### `protected inline BMXClient(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a326568e776c20eaa89572fa951f3b272" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1a326568e776c20eaa89572fa951f3b272"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_client_1ace0e44c62cbfc2d4a820fa31837c685b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_client_1ace0e44c62cbfc2d4a820fa31837c685b"></a>

## class `BMXConversation` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation"></a>

```
class BMXConversation
  : public im.floo.floolib.BMXBaseObject
```

会话

### Summary

| Members                                                                                                                                                                                                                 | Descriptions                                 |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------- |
| `public inline synchronized void delete()`                                                                                                                                                                              |                                              |
| `public inline long conversationId()`                                                                                                                                                                                   | 会话Id                                         |
| `public inline BMXConversation.Type type()`                                                                                                                                                                             | 会话类型                                         |
| `public inline` [`BMXMessage`](broken-reference) `lastMsg()`                                                                                                                                                            | 最新消息                                         |
| `public inline int unreadNumber()`                                                                                                                                                                                      | 未读消息数                                        |
| `public inline int messageCount()`                                                                                                                                                                                      | 会话中所有消息的数量                                   |
| `public inline boolean isMuteNotification()`                                                                                                                                                                            | 是否提醒用户消息,不提醒的情况下会话总未读数不会统计该会话计数。             |
| `public inline String extension()`                                                                                                                                                                                      | 扩展信息                                         |
| `public inline` [`BMXErrorCode`](broken-reference) `setExtension(String ext)`                                                                                                                                           | 设置扩展信息                                       |
| `public inline String editMessage()`                                                                                                                                                                                    | 编辑消息                                         |
| `public inline` [`BMXErrorCode`](broken-reference) `setEditMessage(String editMessage)`                                                                                                                                 | 设置编辑消息                                       |
| `public inline` [`BMXErrorCode`](broken-reference) `searchMessagesByKeyWords(String keywords,long refTime,long size,`[`BMXMessageList`](broken-reference) `result,BMXConversation.Direction arg4)`                      | 搜索消息，如果不指定则从最新消息开始                           |
| `public inline` [`BMXErrorCode`](broken-reference) `searchMessagesByKeyWords(String keywords,long refTime,long size,`[`BMXMessageList`](broken-reference) `result)`                                                     |                                              |
| `public inline` [`BMXErrorCode`](broken-reference) `searchMessagesByType(BMXMessage.ContentType type,long refTime,long size,`[`BMXMessageList`](broken-reference) `result,BMXConversation.Direction arg4)`              | 按照类型搜索消息，如果不指定则从最新消息开始                       |
| `public inline` [`BMXErrorCode`](broken-reference) `searchMessagesByType(BMXMessage.ContentType type,long refTime,long size,`[`BMXMessageList`](broken-reference) `result)`                                             |                                              |
| `public inline void setMessagePlayedStatus(final` [`BMXMessage`](broken-reference) `msg,final boolean status,final BMXCallBack callBack)`                                                                               | 设置消息播放状态（只对语音/视频消息有效）                        |
| `public inline void setMessageReadStatus(final` [`BMXMessage`](broken-reference) `msg,final boolean status,final BMXCallBack callBack)`                                                                                 | 设置消息未读状态，更新未读消息数                             |
| `public inline void setAllMessagesRead(final BMXCallBack callBack)`                                                                                                                                                     | 把所有消息设置为已读，更新未读消息数                           |
| `public inline void updateMessageExtension(final` [`BMXMessage`](broken-reference) `msg,final BMXCallBack callBack)`                                                                                                    | 更新一条数据库存储消息的扩展字段信息                           |
| `public inline void insertMessage(final` [`BMXMessage`](broken-reference) `msg,final BMXCallBack callBack)`                                                                                                             | 插入一条消息                                       |
| `public inline void loadMessage(final long msgId,final BMXDataCallBack<` [`BMXMessage`](broken-reference) `> callBack)`                                                                                                 | 读取一条消息                                       |
| `public inline void removeAllMessages(final BMXCallBack callBack)`                                                                                                                                                      | 删除会话中的所有消息                                   |
| `public inline void loadMessages(final long refMsgId,final long size,final BMXConversation.Direction arg3,final BMXDataCallBack<` [`BMXMessageList`](broken-reference) `> callBack)`                                    | 加载消息，如果不指定则从最新消息开始                           |
| `public inline void loadMessages(final long refMsgId,final long size,final BMXDataCallBack<` [`BMXMessageList`](broken-reference) `> callBack)`                                                                         |                                              |
| `public inline void searchMessages(final String keywords,final long refTime,final long size,final BMXConversation.Direction arg4,final BMXDataCallBack<` [`BMXMessageList`](broken-reference) `> callBack)`             | 搜索消息，如果不指定则从最新消息开始                           |
| `public inline void searchMessages(final String keywords,final long refTime,final long size,final BMXDataCallBack<` [`BMXMessageList`](broken-reference) `> callBack)`                                                  |                                              |
| `public inline void searchMessages(final BMXMessage.ContentType type,final long refTime,final long size,final BMXConversation.Direction arg4,final BMXDataCallBack<` [`BMXMessageList`](broken-reference) `> callBack)` | 按照类型搜索消息，如果不指定则从最新消息开始                       |
| `public inline void searchMessages(final BMXMessage.ContentType type,final long refTime,final long size,final BMXDataCallBack<` [`BMXMessageList`](broken-reference) `> callBack)`                                      |                                              |
| `public inline void refreshConversation(final BMXCallBack callBack)`                                                                                                                                                    | 读取数据库当前会话所有消息数量，强制更新conversation的消息总数和未读消息数。 |
| `protected inline BMXConversation(long cPtr,boolean cMemoryOwn)`                                                                                                                                                        |                                              |
| `protected inline void finalize()`                                                                                                                                                                                      |                                              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a4b165a2e1fad7fbd3dae9466a087f142" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a4b165a2e1fad7fbd3dae9466a087f142"></a>

#### `public inline long conversationId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a57d7be520594c0b7fb309f6994a4b12a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a57d7be520594c0b7fb309f6994a4b12a"></a>

会话Id

**Returns**

int64\_t

#### `public inline BMXConversation.Type type()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a80cb5f1f9fa3781a379d9800f702e3ca" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a80cb5f1f9fa3781a379d9800f702e3ca"></a>

会话类型

**Returns**

[Type](broken-reference)

#### `public inline` [`BMXMessage`](broken-reference) `lastMsg()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a603b5e782caae778386d923d3f0ae822" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a603b5e782caae778386d923d3f0ae822"></a>

最新消息

**Returns**

BMXMessagePtr

#### `public inline int unreadNumber()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1ad9cdd0fb4fb0292a4be91bb834d35c75" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1ad9cdd0fb4fb0292a4be91bb834d35c75"></a>

未读消息数

**Returns**

int32\_t

#### `public inline int messageCount()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1aa23b2f6ff430530c46df721bb0bad11c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1aa23b2f6ff430530c46df721bb0bad11c"></a>

会话中所有消息的数量

**Returns**

int32\_t

#### `public inline boolean isMuteNotification()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a1730ee2705789f9dc27a0180be83e8b0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a1730ee2705789f9dc27a0180be83e8b0"></a>

是否提醒用户消息,不提醒的情况下会话总未读数不会统计该会话计数。

**Returns**

bool

#### `public inline String extension()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1aaf9825306529766889613ab17d52b077" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1aaf9825306529766889613ab17d52b077"></a>

扩展信息

**Returns**

JSON(std::string)

#### `public inline` [`BMXErrorCode`](broken-reference) `setExtension(String ext)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a963ae4d9c8a4756f317fa5a270984d94" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a963ae4d9c8a4756f317fa5a270984d94"></a>

设置扩展信息

**Parameters**

* `ext` 会话扩展消息

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline String editMessage()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1ae49a6fe7c696eca413295b756759ee34" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1ae49a6fe7c696eca413295b756759ee34"></a>

编辑消息

**Returns**

std::string

#### `public inline` [`BMXErrorCode`](broken-reference) `setEditMessage(String editMessage)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1af89eefdc6ba9ef61046948c6c2526297" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1af89eefdc6ba9ef61046948c6c2526297"></a>

设置编辑消息

**Parameters**

* `editMessage` 会话正在编辑的文本消息

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `searchMessagesByKeyWords(String keywords,long refTime,long size,`[`BMXMessageList`](broken-reference) `result,BMXConversation.Direction arg4)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a229c6b415380d0e2e27352df3e186c40" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a229c6b415380d0e2e27352df3e186c40"></a>

搜索消息，如果不指定则从最新消息开始

**Parameters**

* `keywords` 搜索消息的关键字
* `refTime` 搜索消息的起始时间
* `size` 最大加载消息条数
* `result` 搜索到的消息结果列表
* `arg4` 消息搜索方向，默认（Direction::Up）是从更早的消息中搜索

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `searchMessagesByKeyWords(String keywords,long refTime,long size,`[`BMXMessageList`](broken-reference) `result)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1aa426114be19251fd83a972c389dfada2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1aa426114be19251fd83a972c389dfada2"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `searchMessagesByType(BMXMessage.ContentType type,long refTime,long size,`[`BMXMessageList`](broken-reference) `result,BMXConversation.Direction arg4)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1ae59698407ef67abf7d5ca8e88900c1ec" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1ae59698407ef67abf7d5ca8e88900c1ec"></a>

按照类型搜索消息，如果不指定则从最新消息开始

**Parameters**

* `type` 搜索消息的类型
* `refTime` 搜索消息的起始时间
* `size` 最大加载消息条数
* `result` 搜索到的消息结果列表
* `arg4` 消息搜索方向，默认（Direction::Up）是从更早的消息中搜索

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `searchMessagesByType(BMXMessage.ContentType type,long refTime,long size,`[`BMXMessageList`](broken-reference) `result)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a1c95c7a684c773ba81dc7cfb2f6cdce8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a1c95c7a684c773ba81dc7cfb2f6cdce8"></a>

#### `public inline void setMessagePlayedStatus(final` [`BMXMessage`](broken-reference) `msg,final boolean status,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a8be0a785521479a9d9415caf33e418a1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a8be0a785521479a9d9415caf33e418a1"></a>

设置消息播放状态（只对语音/视频消息有效）

**Parameters**

* `msg` 需要设置播放状态的消息
* `status` 消息是否已经播放
* `callBack` 回调

#### `public inline void setMessageReadStatus(final` [`BMXMessage`](broken-reference) `msg,final boolean status,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a2f2b4d7612ee84627f6ddc98670931f0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a2f2b4d7612ee84627f6ddc98670931f0"></a>

设置消息未读状态，更新未读消息数

**Parameters**

* `msg` 需要设置消息已读状态的消息
* `status` 消息是否设置已读
* `callBack` 回调

#### `public inline void setAllMessagesRead(final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1afd59d99e7a6100dd1958ac235c8a201c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1afd59d99e7a6100dd1958ac235c8a201c"></a>

把所有消息设置为已读，更新未读消息数

**Parameters**

* `callBack` 回调

#### `public inline void updateMessageExtension(final` [`BMXMessage`](broken-reference) `msg,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1ae35c1fad6552eac42c4bc433b3f4ad84" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1ae35c1fad6552eac42c4bc433b3f4ad84"></a>

更新一条数据库存储消息的扩展字段信息

**Parameters**

* `msg` 需要更改扩展信息的消息此时msg部分已经更新扩展字椴信息
* `callBack` 回调

#### `public inline void insertMessage(final` [`BMXMessage`](broken-reference) `msg,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1af240b9389cfc46ca609e86e0b99f0add" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1af240b9389cfc46ca609e86e0b99f0add"></a>

插入一条消息

**Parameters**

* `msg` 插入的消息
* `callBack` 回调

#### `public inline void loadMessage(final long msgId,final BMXDataCallBack<` [`BMXMessage`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1aa0830fc576ca70615db8a4d3630a442f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1aa0830fc576ca70615db8a4d3630a442f"></a>

读取一条消息

**Parameters**

* `msgId` 需要读取的消息的消息id
* `callBack` 回调

#### `public inline void removeAllMessages(final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1ab44109b9e1136bf48059d9beb3a8a3bf" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1ab44109b9e1136bf48059d9beb3a8a3bf"></a>

删除会话中的所有消息

**Parameters**

* `callBack` 回调

#### `public inline void loadMessages(final long refMsgId,final long size,final BMXConversation.Direction arg3,final BMXDataCallBack<` [`BMXMessageList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a3bf03785114b28503020c9dcb0ad8250" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a3bf03785114b28503020c9dcb0ad8250"></a>

加载消息，如果不指定则从最新消息开始

**Parameters**

* `refMsgId` 加载消息的起始id
* `size` 最大加载消息条数
* `arg3` 加载消息的方向，默认是加载更早的消息
* `callBack` 回调

#### `public inline void loadMessages(final long refMsgId,final long size,final BMXDataCallBack<` [`BMXMessageList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a15449fefd7c78240845eb193bb8e6596" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a15449fefd7c78240845eb193bb8e6596"></a>

#### `public inline void searchMessages(final String keywords,final long refTime,final long size,final BMXConversation.Direction arg4,final BMXDataCallBack<` [`BMXMessageList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a35d21e95c1e01c0e2ffd8e32b6a28512" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a35d21e95c1e01c0e2ffd8e32b6a28512"></a>

搜索消息，如果不指定则从最新消息开始

**Parameters**

* `keywords` 搜索消息的关键字
* `refTime` 搜索消息的起始时间
* `size` 最大加载消息条数
* `arg4` 消息搜索方向，默认（Direction::Up）是从更早的消息中搜索
* `callBack` 回调

#### `public inline void searchMessages(final String keywords,final long refTime,final long size,final BMXDataCallBack<` [`BMXMessageList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1aa5e4670526fdae1ba47179ae34dbee2d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1aa5e4670526fdae1ba47179ae34dbee2d"></a>

#### `public inline void searchMessages(final BMXMessage.ContentType type,final long refTime,final long size,final BMXConversation.Direction arg4,final BMXDataCallBack<` [`BMXMessageList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a5bf343f9dfb071d980be1eaffc819c81" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a5bf343f9dfb071d980be1eaffc819c81"></a>

按照类型搜索消息，如果不指定则从最新消息开始

**Parameters**

* `type` 搜索消息的类型
* `refTime` 搜索消息的起始时间
* `size` 最大加载消息条数
* `arg4` 消息搜索方向，默认（Direction::Up）是从更早的消息中搜索
* `callBack` 回调

#### `public inline void searchMessages(final BMXMessage.ContentType type,final long refTime,final long size,final BMXDataCallBack<` [`BMXMessageList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a3550d994e1a8dbae192facdfe1a465d2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1a3550d994e1a8dbae192facdfe1a465d2"></a>

#### `public inline void refreshConversation(final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1ab2348cee8ffde2edbc6698acccd30a26" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1ab2348cee8ffde2edbc6698acccd30a26"></a>

读取数据库当前会话所有消息数量，强制更新conversation的消息总数和未读消息数。

**Parameters**

* `callBack` 回调

#### `protected inline BMXConversation(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1aa239ecaab3881270044a3a67c938c587" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1aa239ecaab3881270044a3a67c938c587"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1ad22f1b471bd7e019cc32a217046f87f9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_1ad22f1b471bd7e019cc32a217046f87f9"></a>

## class `BMXConversationList` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list"></a>

### Summary

| Members                                                                     | Descriptions |
| --------------------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                                  |              |
| `public inline BMXConversationList()`                                       |              |
| `public inline BMXConversationList(long n)`                                 |              |
| `public inline long size()`                                                 |              |
| `public inline long capacity()`                                             |              |
| `public inline void reserve(long n)`                                        |              |
| `public inline boolean isEmpty()`                                           |              |
| `public inline void clear()`                                                |              |
| `public inline void add(`[`BMXConversation`](broken-reference) `x)`         |              |
| `public inline` [`BMXConversation`](broken-reference) `get(int i)`          |              |
| `public inline void set(int i,`[`BMXConversation`](broken-reference) `val)` |              |
| `protected transient boolean swigCMemOwn`                                   |              |
| `protected inline BMXConversationList(long cPtr,boolean cMemoryOwn)`        |              |
| `protected inline void finalize()`                                          |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1aabfa63755389050f626f26a41f358009" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1aabfa63755389050f626f26a41f358009"></a>

#### `public inline BMXConversationList()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1a79f3757e651e77900fa777e88ebd2907" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1a79f3757e651e77900fa777e88ebd2907"></a>

#### `public inline BMXConversationList(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1af5d5d89234f49b0dc35b8affe748d39c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1af5d5d89234f49b0dc35b8affe748d39c"></a>

#### `public inline long size()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1afe8e5bb0815d5647f67375180ff8d7d4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1afe8e5bb0815d5647f67375180ff8d7d4"></a>

#### `public inline long capacity()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1abf2cf85c9cd6c4d9440c2f08a1f47552" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1abf2cf85c9cd6c4d9440c2f08a1f47552"></a>

#### `public inline void reserve(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1ab34a13437372ca9eca07c1b0ea568b7a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1ab34a13437372ca9eca07c1b0ea568b7a"></a>

#### `public inline boolean isEmpty()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1a8294dd0ee0d3a0e56ad989dcfdb08192" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1a8294dd0ee0d3a0e56ad989dcfdb08192"></a>

#### `public inline void clear()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1a4356424b3d743afb801fd7ffd669979e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1a4356424b3d743afb801fd7ffd669979e"></a>

#### `public inline void add(`[`BMXConversation`](broken-reference) `x)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1a7ac0a026eb5237318308e60132c519ad" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1a7ac0a026eb5237318308e60132c519ad"></a>

#### `public inline` [`BMXConversation`](broken-reference) `get(int i)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1ab7eb27deb9087e387afc58e9264a702e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1ab7eb27deb9087e387afc58e9264a702e"></a>

#### `public inline void set(int i,`[`BMXConversation`](broken-reference) `val)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1abac8ce1a593ec9e089a6297d8a00b35f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1abac8ce1a593ec9e089a6297d8a00b35f"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1aa596d76147f82e5205731b09cd6e4edf" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1aa596d76147f82e5205731b09cd6e4edf"></a>

#### `protected inline BMXConversationList(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1a8e9899851dc023e7faac733319e440c3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1a8e9899851dc023e7faac733319e440c3"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1ae3cfcaa82518dfa61c7c4119acd6ae6f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_conversation_list_1ae3cfcaa82518dfa61c7c4119acd6ae6f"></a>

## class `BMXDevice` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device"></a>

设备信息

### Summary

| Members                                                    | Descriptions |
| ---------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                 |              |
| `public inline int deviceSN()`                             | 设备序列号        |
| `public inline long userId()`                              | 用户id         |
| `public inline int platform()`                             | 软件平台         |
| `public inline String userAgent()`                         | 用户代理信息       |
| `public inline void setUserAgent(String userAgent)`        | 设置用户代理信息     |
| `public inline boolean isCurrentDevice()`                  | 是否是当前设备      |
| `protected inline BMXDevice(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                         |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_1a2a067186f4d5cb74f2c87fd7fac13d70" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_1a2a067186f4d5cb74f2c87fd7fac13d70"></a>

#### `public inline int deviceSN()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_1a638170513d33cdcc3a5dc417d2351650" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_1a638170513d33cdcc3a5dc417d2351650"></a>

设备序列号

**Returns**

int

#### `public inline long userId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_1a1791f243d71fd3d208151a2222a899a8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_1a1791f243d71fd3d208151a2222a899a8"></a>

用户id

**Returns**

int64\_t

#### `public inline int platform()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_1ac9f64905a95a25d8542c392112e24b38" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_1ac9f64905a95a25d8542c392112e24b38"></a>

软件平台

**Returns**

int

#### `public inline String userAgent()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_1ac062df6d89f2d40152f72cd96b702b08" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_1ac062df6d89f2d40152f72cd96b702b08"></a>

用户代理信息

**Returns**

std::string

#### `public inline void setUserAgent(String userAgent)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_1a5bf7aa3decd674f4faa0554c113bfde2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_1a5bf7aa3decd674f4faa0554c113bfde2"></a>

设置用户代理信息

**Parameters**

* `userAgent` 用户代理信息

#### `public inline boolean isCurrentDevice()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_1abee8cceb434bc41d070ceaafbe6fe961" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_1abee8cceb434bc41d070ceaafbe6fe961"></a>

是否是当前设备

**Returns**

bool

#### `protected inline BMXDevice(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_1a4911257e885912d75749d00e9c0b14f4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_1a4911257e885912d75749d00e9c0b14f4"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_1a884688934676cc347fd7074cf59497f2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_1a884688934676cc347fd7074cf59497f2"></a>

## class `BMXDeviceList` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_list" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_list"></a>

### Summary

| Members                                                               | Descriptions |
| --------------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                            |              |
| `public inline BMXDeviceList()`                                       |              |
| `public inline BMXDeviceList(long n)`                                 |              |
| `public inline long size()`                                           |              |
| `public inline long capacity()`                                       |              |
| `public inline void reserve(long n)`                                  |              |
| `public inline boolean isEmpty()`                                     |              |
| `public inline void clear()`                                          |              |
| `public inline void add(`[`BMXDevice`](broken-reference) `x)`         |              |
| `public inline` [`BMXDevice`](broken-reference) `get(int i)`          |              |
| `public inline void set(int i,`[`BMXDevice`](broken-reference) `val)` |              |
| `protected transient boolean swigCMemOwn`                             |              |
| `protected inline BMXDeviceList(long cPtr,boolean cMemoryOwn)`        |              |
| `protected inline void finalize()`                                    |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1a838023896e9dba96cb947abf128bf1c7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1a838023896e9dba96cb947abf128bf1c7"></a>

#### `public inline BMXDeviceList()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1a8a4432ae70cd8e52a9a4d45c106b0637" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1a8a4432ae70cd8e52a9a4d45c106b0637"></a>

#### `public inline BMXDeviceList(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1aafca03fe28243fcd465733ad17ae4538" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1aafca03fe28243fcd465733ad17ae4538"></a>

#### `public inline long size()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1a6f3a56371788d4e1ba7f5370dc8834be" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1a6f3a56371788d4e1ba7f5370dc8834be"></a>

#### `public inline long capacity()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1a0632f37a99b870273838bdc3700225a9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1a0632f37a99b870273838bdc3700225a9"></a>

#### `public inline void reserve(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1ab87584cc67eecd8a7a2426490af9d210" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1ab87584cc67eecd8a7a2426490af9d210"></a>

#### `public inline boolean isEmpty()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1a0a88c6cf011b8d28fcfeaf544b9a9ab5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1a0a88c6cf011b8d28fcfeaf544b9a9ab5"></a>

#### `public inline void clear()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1a5a09928962d296c2aa8bf9d3403dd67d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1a5a09928962d296c2aa8bf9d3403dd67d"></a>

#### `public inline void add(`[`BMXDevice`](broken-reference) `x)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1acf10cac72d7fd0d8f872e43d0002246d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1acf10cac72d7fd0d8f872e43d0002246d"></a>

#### `public inline` [`BMXDevice`](broken-reference) `get(int i)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1ab453087a110e7a67042c9b828cd19133" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1ab453087a110e7a67042c9b828cd19133"></a>

#### `public inline void set(int i,`[`BMXDevice`](broken-reference) `val)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1a5a43de9f5d35de4e09500c42cc7f6424" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1a5a43de9f5d35de4e09500c42cc7f6424"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1ad4d8678ad83e87840c7853f26f4d6874" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1ad4d8678ad83e87840c7853f26f4d6874"></a>

#### `protected inline BMXDeviceList(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1ac886c61cae8df0b4d17fb568cb059f5d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1ac886c61cae8df0b4d17fb568cb059f5d"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1a13c8df0489dc9ec16359faa2874836c0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_device_list_1a13c8df0489dc9ec16359faa2874836c0"></a>

## class `BMXError` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_error" id="classim_1_1floo_1_1floolib_1_1_b_m_x_error"></a>

### Summary

| Members                                                                  | Descriptions |
| ------------------------------------------------------------------------ | ------------ |
| `public inline synchronized void delete()`                               |              |
| `public inline BMXError(`[`BMXErrorCode`](broken-reference) `errorCode)` |              |
| `public inline` [`BMXErrorCode`](broken-reference) `errorCode()`         |              |
| `public inline String description()`                                     |              |
| `protected transient boolean swigCMemOwn`                                |              |
| `protected inline BMXError(long cPtr,boolean cMemoryOwn)`                |              |
| `protected inline void finalize()`                                       |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_error_1a2f61e8eb8e3157f1046d86a83115f35e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_error_1a2f61e8eb8e3157f1046d86a83115f35e"></a>

#### `public inline BMXError(`[`BMXErrorCode`](broken-reference) `errorCode)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_error_1ae906eb33d7e441cc6c7b36f18a8db185" id="classim_1_1floo_1_1floolib_1_1_b_m_x_error_1ae906eb33d7e441cc6c7b36f18a8db185"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `errorCode()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_error_1ab0957f079d54ceca158a76b794291f08" id="classim_1_1floo_1_1floolib_1_1_b_m_x_error_1ab0957f079d54ceca158a76b794291f08"></a>

#### `public inline String description()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_error_1a016e1cb53b1d6e6939d97fbe75a4e687" id="classim_1_1floo_1_1floolib_1_1_b_m_x_error_1a016e1cb53b1d6e6939d97fbe75a4e687"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_error_1a6591818639a693dee14a0c8adab5c23c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_error_1a6591818639a693dee14a0c8adab5c23c"></a>

#### `protected inline BMXError(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_error_1a0cd8a2087aca7745e39a5316ab2adb4b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_error_1a0cd8a2087aca7745e39a5316ab2adb4b"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_error_1a10968e0e3a6ee676e975ea76971fe4a5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_error_1a10968e0e3a6ee676e975ea76971fe4a5"></a>

## class `BMXFileAttachment` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment" id="classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment"></a>

```
class BMXFileAttachment
  : public im.floo.floolib.BMXMessageAttachment
```

消息文件附件

### Summary

| Members                                                                               | Descriptions    |
| ------------------------------------------------------------------------------------- | --------------- |
| `public inline synchronized void delete()`                                            |                 |
| `public inline BMXFileAttachment(String path,String displayName)`                     | 构造函数，构建发送文件消息附件 |
| `public inline BMXFileAttachment(String path)`                                        |                 |
| `public inline BMXFileAttachment(String ratelUrl,String displayName,long fileLength)` | 构造函数，构建接收文件消息附件 |
| `public inline BMXMessageAttachment.Type type()`                                      | 返回文件类型          |
| `public inline` [`BMXMessageAttachment`](broken-reference) `clone()`                  | 克隆函数            |
| `public inline String path()`                                                         | 本地路径            |
| `public inline String displayName()`                                                  | 显示名             |
| `public inline String ratelUrl()`                                                     |                 |
| `public inline String url()`                                                          | 远程URL           |
| `public inline long fileLength()`                                                     | 文件长度            |
| `public inline BMXMessageAttachment.DownloadStatus downloadStatus()`                  | 附件下载状态          |
| `protected inline BMXFileAttachment(long cPtr,boolean cMemoryOwn)`                    |                 |
| `protected inline void finalize()`                                                    |                 |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a325012a06bead3b6953fa2eae7f77a01" id="classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a325012a06bead3b6953fa2eae7f77a01"></a>

#### `public inline BMXFileAttachment(String path,String displayName)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a1e63cce332170d9258b1b00add3854fb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a1e63cce332170d9258b1b00add3854fb"></a>

构造函数，构建发送文件消息附件

**Parameters**

* `path` 文件的本地路径
* `displayName` 文件展示名

#### `public inline BMXFileAttachment(String path)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a8ab2799d2464390755adb2c0f82f86a4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a8ab2799d2464390755adb2c0f82f86a4"></a>

#### `public inline BMXFileAttachment(String ratelUrl,String displayName,long fileLength)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a74c6d13dc6b64f43721f07324a022bd6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a74c6d13dc6b64f43721f07324a022bd6"></a>

构造函数，构建接收文件消息附件

**Parameters**

* `ratelUrl` ratel服务器地址
* `displayName` 文件展示名
* `fileLength` 文件大小

#### `public inline BMXMessageAttachment.Type type()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a84c432b83132ca09ff4f5c0c6a8d8b93" id="classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a84c432b83132ca09ff4f5c0c6a8d8b93"></a>

返回文件类型

**Returns**

Type

#### `public inline` [`BMXMessageAttachment`](broken-reference) `clone()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1acbaee137cdd57d6664c88a1945a6b39c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1acbaee137cdd57d6664c88a1945a6b39c"></a>

克隆函数

**Returns**

BMXMessageAttachmentPtr

#### `public inline String path()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a2f8e5d3032f99c0b13366e22448b6801" id="classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a2f8e5d3032f99c0b13366e22448b6801"></a>

本地路径

**Returns**

std::string

#### `public inline String displayName()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a8761fd797d978fd7665b72307ba38b71" id="classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a8761fd797d978fd7665b72307ba38b71"></a>

显示名

**Returns**

std::string

#### `public inline String ratelUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1adc1148deb83c68b153ee3f21de7c18f2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1adc1148deb83c68b153ee3f21de7c18f2"></a>

#### `public inline String url()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1abfd72daf3b1cb668e5206debe8067520" id="classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1abfd72daf3b1cb668e5206debe8067520"></a>

远程URL

**Returns**

std::string

#### `public inline long fileLength()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a1552782b38b78ce463223e685b72798f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a1552782b38b78ce463223e685b72798f"></a>

文件长度

**Returns**

std::string

#### `public inline BMXMessageAttachment.DownloadStatus downloadStatus()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a5aa8ae303c8518c7236a0b7fa22a1917" id="classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a5aa8ae303c8518c7236a0b7fa22a1917"></a>

附件下载状态

**Returns**

DownloadStatus

#### `protected inline BMXFileAttachment(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1aaccc2f7dc86e93f87d30068276b7b4d7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1aaccc2f7dc86e93f87d30068276b7b4d7"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a7292a67c75d6193bd337b9a3e654cc3c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_file_attachment_1a7292a67c75d6193bd337b9a3e654cc3c"></a>

## class `BMXGroupAnnouncementList` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list"></a>

### Summary

| Members                                                                   | Descriptions |
| ------------------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                                |              |
| `public inline BMXGroupAnnouncementList()`                                |              |
| `public inline BMXGroupAnnouncementList(long n)`                          |              |
| `public inline long size()`                                               |              |
| `public inline long capacity()`                                           |              |
| `public inline void reserve(long n)`                                      |              |
| `public inline boolean isEmpty()`                                         |              |
| `public inline void clear()`                                              |              |
| `public inline void add(BMXGroup.Announcement x)`                         |              |
| `public inline BMXGroup.Announcement get(int i)`                          |              |
| `public inline void set(int i,BMXGroup.Announcement val)`                 |              |
| `protected transient boolean swigCMemOwn`                                 |              |
| `protected inline BMXGroupAnnouncementList(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                                        |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1ac94e7b3d82757d364f05ba7bb3f2af41" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1ac94e7b3d82757d364f05ba7bb3f2af41"></a>

#### `public inline BMXGroupAnnouncementList()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a5145d7acf0be470c09b5537bded2622d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a5145d7acf0be470c09b5537bded2622d"></a>

#### `public inline BMXGroupAnnouncementList(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a1593a65c2f95b7a992e84c82a96f987b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a1593a65c2f95b7a992e84c82a96f987b"></a>

#### `public inline long size()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a922d5695a2d0e1910a7d4896356c2072" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a922d5695a2d0e1910a7d4896356c2072"></a>

#### `public inline long capacity()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a73484c871d2d7fd9ff4a9f5a10448336" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a73484c871d2d7fd9ff4a9f5a10448336"></a>

#### `public inline void reserve(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a7d455ab2ab743f7f446487316afb9df3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a7d455ab2ab743f7f446487316afb9df3"></a>

#### `public inline boolean isEmpty()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a7239328491a7ed2e0c9a564f7ea887d5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a7239328491a7ed2e0c9a564f7ea887d5"></a>

#### `public inline void clear()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a301123f7d9a12c36627428a3daf8acdb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a301123f7d9a12c36627428a3daf8acdb"></a>

#### `public inline void add(BMXGroup.Announcement x)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1aeb26491a07223826fcd14848748d629d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1aeb26491a07223826fcd14848748d629d"></a>

#### `public inline BMXGroup.Announcement get(int i)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1aee09b8bc079badf37ed73599dfe509ee" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1aee09b8bc079badf37ed73599dfe509ee"></a>

#### `public inline void set(int i,BMXGroup.Announcement val)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a60f429566a2c0f644ddb0748bc432a4b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a60f429566a2c0f644ddb0748bc432a4b"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a08414e6db3859ba2a980ff3eee004e08" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a08414e6db3859ba2a980ff3eee004e08"></a>

#### `protected inline BMXGroupAnnouncementList(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a311afe84e010987e81dfe86263b384a3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1a311afe84e010987e81dfe86263b384a3"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1aa5c544c172085eb50663095dcefeed43" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_announcement_list_1aa5c544c172085eb50663095dcefeed43"></a>

## class `BMXGroupApplicationList` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list"></a>

### Summary

| Members                                                                  | Descriptions |
| ------------------------------------------------------------------------ | ------------ |
| `public inline synchronized void delete()`                               |              |
| `public inline BMXGroupApplicationList()`                                |              |
| `public inline BMXGroupApplicationList(long n)`                          |              |
| `public inline long size()`                                              |              |
| `public inline long capacity()`                                          |              |
| `public inline void reserve(long n)`                                     |              |
| `public inline boolean isEmpty()`                                        |              |
| `public inline void clear()`                                             |              |
| `public inline void add(BMXGroup.Application x)`                         |              |
| `public inline BMXGroup.Application get(int i)`                          |              |
| `public inline void set(int i,BMXGroup.Application val)`                 |              |
| `protected transient boolean swigCMemOwn`                                |              |
| `protected inline BMXGroupApplicationList(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                                       |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1ad5e6f05899ee7b07b5bfaf429d01cfd7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1ad5e6f05899ee7b07b5bfaf429d01cfd7"></a>

#### `public inline BMXGroupApplicationList()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a7336fb8f4cd5a3b4ff347e734f60e518" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a7336fb8f4cd5a3b4ff347e734f60e518"></a>

#### `public inline BMXGroupApplicationList(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1ad307e05025094dfbe439280c61d80e12" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1ad307e05025094dfbe439280c61d80e12"></a>

#### `public inline long size()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a16e8700021c94da10f68a4e03219dd69" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a16e8700021c94da10f68a4e03219dd69"></a>

#### `public inline long capacity()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a5ae21f3ec6afaa578ab8edd95c8770c7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a5ae21f3ec6afaa578ab8edd95c8770c7"></a>

#### `public inline void reserve(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a6adec80aa691a421daf2be610550e9a9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a6adec80aa691a421daf2be610550e9a9"></a>

#### `public inline boolean isEmpty()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a7099a66cef15fe0bf7f6c6bc9d49a4c7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a7099a66cef15fe0bf7f6c6bc9d49a4c7"></a>

#### `public inline void clear()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a54e6933336561df1628b8c81a48fdbb0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a54e6933336561df1628b8c81a48fdbb0"></a>

#### `public inline void add(BMXGroup.Application x)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a8798fb800d5336f7ca0aec66a18395f9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a8798fb800d5336f7ca0aec66a18395f9"></a>

#### `public inline BMXGroup.Application get(int i)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a7b828463dcabf5e10534c34b88da647c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a7b828463dcabf5e10534c34b88da647c"></a>

#### `public inline void set(int i,BMXGroup.Application val)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a1818cec8d95f62c72b83d7df407ff4cc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a1818cec8d95f62c72b83d7df407ff4cc"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a20d04322b8464285203d2657ef792e73" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1a20d04322b8464285203d2657ef792e73"></a>

#### `protected inline BMXGroupApplicationList(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1ae5028796a0808f69d0505179efeb3b79" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1ae5028796a0808f69d0505179efeb3b79"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1abf2656f2228795cfa98357b9de4e8f37" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_application_list_1abf2656f2228795cfa98357b9de4e8f37"></a>

## class `BMXGroupBannedMemberList` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list"></a>

### Summary

| Members                                                                   | Descriptions |
| ------------------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                                |              |
| `public inline BMXGroupBannedMemberList()`                                |              |
| `public inline BMXGroupBannedMemberList(long n)`                          |              |
| `public inline long size()`                                               |              |
| `public inline long capacity()`                                           |              |
| `public inline void reserve(long n)`                                      |              |
| `public inline boolean isEmpty()`                                         |              |
| `public inline void clear()`                                              |              |
| `public inline void add(BMXGroup.BannedMember x)`                         |              |
| `public inline BMXGroup.BannedMember get(int i)`                          |              |
| `public inline void set(int i,BMXGroup.BannedMember val)`                 |              |
| `protected transient boolean swigCMemOwn`                                 |              |
| `protected inline BMXGroupBannedMemberList(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                                        |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1a17625ebf64e43e065eb81b916598f5dc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1a17625ebf64e43e065eb81b916598f5dc"></a>

#### `public inline BMXGroupBannedMemberList()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1a42f11cc6384594220546820c83e8c888" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1a42f11cc6384594220546820c83e8c888"></a>

#### `public inline BMXGroupBannedMemberList(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1a35e34587f86589ec5a484afd9134f983" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1a35e34587f86589ec5a484afd9134f983"></a>

#### `public inline long size()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1ac6089f40e70f694f252ae1b201e0d5c7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1ac6089f40e70f694f252ae1b201e0d5c7"></a>

#### `public inline long capacity()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1acbc878571d6d08261291a73deecba085" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1acbc878571d6d08261291a73deecba085"></a>

#### `public inline void reserve(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1a5087d975a08e0995f70f5ab385699274" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1a5087d975a08e0995f70f5ab385699274"></a>

#### `public inline boolean isEmpty()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1ac5105dc153ac586ab8351789a93e4670" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1ac5105dc153ac586ab8351789a93e4670"></a>

#### `public inline void clear()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1a0fe82770e9219270306ab458e1386a6d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1a0fe82770e9219270306ab458e1386a6d"></a>

#### `public inline void add(BMXGroup.BannedMember x)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1a7f22dd1786a0a186a510239096298e52" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1a7f22dd1786a0a186a510239096298e52"></a>

#### `public inline BMXGroup.BannedMember get(int i)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1aac33fdb511c536bdbc343d70efaeadb3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1aac33fdb511c536bdbc343d70efaeadb3"></a>

#### `public inline void set(int i,BMXGroup.BannedMember val)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1ad2669b3b250649886de02986d1d49fa0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1ad2669b3b250649886de02986d1d49fa0"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1ac7c36a6760449db04a16419c17590d68" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1ac7c36a6760449db04a16419c17590d68"></a>

#### `protected inline BMXGroupBannedMemberList(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1a634392483bc90baed8db442278110eb1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1a634392483bc90baed8db442278110eb1"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1af1f29521c727ff2024a9ea5dad874011" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_list_1af1f29521c727ff2024a9ea5dad874011"></a>

## class `BMXGroupBannedMemberResultPage` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page"></a>

```
class BMXGroupBannedMemberResultPage
  : public im.floo.floolib.BMXBaseObject
```

### Summary

| Members                                                                                                               | Descriptions |
| --------------------------------------------------------------------------------------------------------------------- | ------------ |
| `public transient long swigCPtr`                                                                                      |              |
| `public inline synchronized void delete()`                                                                            |              |
| `public inline BMXGroupBannedMemberResultPage()`                                                                      |              |
| `public inline BMXGroupBannedMemberResultPage(`[`BMXGroupBannedMemberList`](broken-reference) `result,long offset)`   |              |
| `public inline BMXGroupBannedMemberResultPage(`[`BMXGroupBannedMemberList`](broken-reference) `result,String cursor)` |              |
| `public inline BMXGroupBannedMemberResultPage(`[`BMXGroupBannedMemberResultPage`](broken-reference) `from)`           |              |
| `public inline long count()`                                                                                          |              |
| `public inline long offset()`                                                                                         |              |
| `public inline String cursor()`                                                                                       |              |
| `public inline` [`BMXGroupBannedMemberList`](broken-reference) `result()`                                             |              |
| `protected inline BMXGroupBannedMemberResultPage(long cPtr,boolean cMemoryOwn)`                                       |              |
| `protected inline void finalize()`                                                                                    |              |

### Members

#### `public transient long swigCPtr` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1a052890764ad48ebf91f80656f5251" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1a052890764ad48ebf91f80656f5251"></a>

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1a37487de3cfd9e37a695af7e382d7c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1a37487de3cfd9e37a695af7e382d7c"></a>

#### `public inline BMXGroupBannedMemberResultPage()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1ae8330cd1c2199cb03406e1c33c881" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1ae8330cd1c2199cb03406e1c33c881"></a>

#### `public inline BMXGroupBannedMemberResultPage(`[`BMXGroupBannedMemberList`](broken-reference) `result,long offset)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1af0b9d3195f57700336aedbcdc0390" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1af0b9d3195f57700336aedbcdc0390"></a>

#### `public inline BMXGroupBannedMemberResultPage(`[`BMXGroupBannedMemberList`](broken-reference) `result,String cursor)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1ad64e2fb3a1670ee9bb23c0064e111" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1ad64e2fb3a1670ee9bb23c0064e111"></a>

#### `public inline BMXGroupBannedMemberResultPage(`[`BMXGroupBannedMemberResultPage`](broken-reference) `from)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1a4b2daa9b981ded49b2663cff5a0ab" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1a4b2daa9b981ded49b2663cff5a0ab"></a>

#### `public inline long count()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1a977be46c4eb4c8ddad5d03e92164f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1a977be46c4eb4c8ddad5d03e92164f"></a>

#### `public inline long offset()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1a8d5ab3afd421f8cfe7790c968ddbe" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1a8d5ab3afd421f8cfe7790c968ddbe"></a>

#### `public inline String cursor()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1a4b5d613e537a1861ded36289e4816" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1a4b5d613e537a1861ded36289e4816"></a>

#### `public inline` [`BMXGroupBannedMemberList`](broken-reference) `result()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1aa9c0165b7da15102d04e46efb4c0d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1aa9c0165b7da15102d04e46efb4c0d"></a>

#### `protected inline BMXGroupBannedMemberResultPage(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1ab798643d8253262b4c99f415ae390" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1ab798643d8253262b4c99f415ae390"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1a4303518667c80720b659e78345fa6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_banned_member_result_page_1a4303518667c80720b659e78345fa6"></a>

## class `BMXGroupInvitationList` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list"></a>

### Summary

| Members                                                                 | Descriptions |
| ----------------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                              |              |
| `public inline BMXGroupInvitationList()`                                |              |
| `public inline BMXGroupInvitationList(long n)`                          |              |
| `public inline long size()`                                             |              |
| `public inline long capacity()`                                         |              |
| `public inline void reserve(long n)`                                    |              |
| `public inline boolean isEmpty()`                                       |              |
| `public inline void clear()`                                            |              |
| `public inline void add(BMXGroup.Invitation x)`                         |              |
| `public inline BMXGroup.Invitation get(int i)`                          |              |
| `public inline void set(int i,BMXGroup.Invitation val)`                 |              |
| `protected transient boolean swigCMemOwn`                               |              |
| `protected inline BMXGroupInvitationList(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                                      |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a0edd08b6c1e9018aec2b91ff50c3dc43" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a0edd08b6c1e9018aec2b91ff50c3dc43"></a>

#### `public inline BMXGroupInvitationList()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1afe0341104cce38e39f225375411d6871" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1afe0341104cce38e39f225375411d6871"></a>

#### `public inline BMXGroupInvitationList(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a6b4babd5963a0432079f3e2acd525f0d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a6b4babd5963a0432079f3e2acd525f0d"></a>

#### `public inline long size()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a1fbaec0c11f1d90759cbe4c6e23923fc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a1fbaec0c11f1d90759cbe4c6e23923fc"></a>

#### `public inline long capacity()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1aa5276812f3a2a7c5db551eb924669fc0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1aa5276812f3a2a7c5db551eb924669fc0"></a>

#### `public inline void reserve(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a1e295466bf38e94d2d89ba0acb71dfe5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a1e295466bf38e94d2d89ba0acb71dfe5"></a>

#### `public inline boolean isEmpty()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a29dfc380cce7fd6418afe4dca29d6c55" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a29dfc380cce7fd6418afe4dca29d6c55"></a>

#### `public inline void clear()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a0d9a2bdc7ab55765d435405e31863f20" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a0d9a2bdc7ab55765d435405e31863f20"></a>

#### `public inline void add(BMXGroup.Invitation x)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a917ee4b755820f7490ac4874b2b84ac6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a917ee4b755820f7490ac4874b2b84ac6"></a>

#### `public inline BMXGroup.Invitation get(int i)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a8cf15ce794af98092f8b4474b395c4c0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a8cf15ce794af98092f8b4474b395c4c0"></a>

#### `public inline void set(int i,BMXGroup.Invitation val)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a9f5702b15d27778afb65809db60ca742" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a9f5702b15d27778afb65809db60ca742"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1ae486d39d53ecdee0553911e545344e80" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1ae486d39d53ecdee0553911e545344e80"></a>

#### `protected inline BMXGroupInvitationList(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1ad76092939ea52731011b7b7eb4f613ae" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1ad76092939ea52731011b7b7eb4f613ae"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a291ca4367dd7b626c850f50291bed218" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_invitation_list_1a291ca4367dd7b626c850f50291bed218"></a>

## class `BMXGroupList` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_list" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_list"></a>

### Summary

| Members                                                              | Descriptions |
| -------------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                           |              |
| `public inline BMXGroupList()`                                       |              |
| `public inline BMXGroupList(long n)`                                 |              |
| `public inline long size()`                                          |              |
| `public inline long capacity()`                                      |              |
| `public inline void reserve(long n)`                                 |              |
| `public inline boolean isEmpty()`                                    |              |
| `public inline void clear()`                                         |              |
| `public inline void add(`[`BMXGroup`](broken-reference) `x)`         |              |
| `public inline` [`BMXGroup`](broken-reference) `get(int i)`          |              |
| `public inline void set(int i,`[`BMXGroup`](broken-reference) `val)` |              |
| `protected transient boolean swigCMemOwn`                            |              |
| `protected inline BMXGroupList(long cPtr,boolean cMemoryOwn)`        |              |
| `protected inline void finalize()`                                   |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a156d21077656975b7f0cbcd3293fb6dd" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a156d21077656975b7f0cbcd3293fb6dd"></a>

#### `public inline BMXGroupList()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a00e2993b4352ad1744ea679b758be4b7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a00e2993b4352ad1744ea679b758be4b7"></a>

#### `public inline BMXGroupList(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a96dc4c5b519e5ba7667be55efa93d5ff" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a96dc4c5b519e5ba7667be55efa93d5ff"></a>

#### `public inline long size()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a28479e327096721f2bb0194a5c120220" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a28479e327096721f2bb0194a5c120220"></a>

#### `public inline long capacity()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a2f6467a7f40752d91a188ab4c9bb674d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a2f6467a7f40752d91a188ab4c9bb674d"></a>

#### `public inline void reserve(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1aa6181cce68e17ccf0ea6b2ae0b542a0e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1aa6181cce68e17ccf0ea6b2ae0b542a0e"></a>

#### `public inline boolean isEmpty()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a581783957ba39ab8b9dce4356bd03d5b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a581783957ba39ab8b9dce4356bd03d5b"></a>

#### `public inline void clear()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a63f2760ef6f4b4dd3f958836daa63f94" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a63f2760ef6f4b4dd3f958836daa63f94"></a>

#### `public inline void add(`[`BMXGroup`](broken-reference) `x)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a6826ff5e8ca79cffd2a5275f3244a1f6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a6826ff5e8ca79cffd2a5275f3244a1f6"></a>

#### `public inline` [`BMXGroup`](broken-reference) `get(int i)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1aff0c435351820d3206ba576678ca5c06" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1aff0c435351820d3206ba576678ca5c06"></a>

#### `public inline void set(int i,`[`BMXGroup`](broken-reference) `val)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a1050b0fd6d92038ec462014f751a4ec9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a1050b0fd6d92038ec462014f751a4ec9"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a33482afc7ddb6441da1bf6065b355433" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a33482afc7ddb6441da1bf6065b355433"></a>

#### `protected inline BMXGroupList(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a367455ab587070b1178f1cb76e3daee5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a367455ab587070b1178f1cb76e3daee5"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a82a397abf39c399cbcc29fc190732645" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_list_1a82a397abf39c399cbcc29fc190732645"></a>

## class `BMXGroupManager` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager"></a>

群组管理器

### Summary

| Members                                                                                                                                                                                                                                            | Descriptions                               |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------ |
| `public inline BMXGroupManager(`[`BMXGroupService`](broken-reference) `service)`                                                                                                                                                                   |                                            |
| `public inline void getGroupList(final boolean forceRefresh,final BMXDataCallBack<` [`BMXGroupList`](broken-reference) `> callBack)`                                                                                                               | 获取群组列表，如果设置了forceRefresh则从服务器拉取            |
| `public inline void getGroupList(final` [`ListOfLongLong`](broken-reference)`groupIdList,final boolean forceRefresh,final BMXDataCallBack<`[`BMXGroupList`](broken-reference) `> callBack)`                                                        | 获取传入群组id的群组信息列表，如果设置了forceRefresh则从服务器拉取   |
| `public inline void getGroupList(final long groupId,final boolean forceUpdate,final BMXDataCallBack<` [`BMXGroup`](broken-reference) `> callBack)`                                                                                                 | 获取群信息，如果设置了forceRefresh则从服务器拉取             |
| `public inline void getInvitationList(final String cursor,final int pageSize,final BMXDataCallBack<` [`GroupInvitaionPage`](broken-reference) `> callBack)`                                                                                        | 分页获取群组邀请列表                                 |
| `public inline void getApplicationList(final` [`BMXGroupList`](broken-reference)`list,final String cursor,final int pageSize,final BMXDataCallBack<`[`GroupApplicationPage`](broken-reference) `> callBack)`                                       | 分页获取群组申请列表                                 |
| `public inline void create(final BMXGroupService.CreateGroupOptions options,final BMXDataCallBack<` [`BMXGroup`](broken-reference) `> callBack)`                                                                                                   | 创建群                                        |
| `public inline void destroy(final` [`BMXGroup`](broken-reference) `group,final BMXCallBack callBack)`                                                                                                                                              | 销毁群                                        |
| `public inline void join(final` [`BMXGroup`](broken-reference) `group,final String message,final BMXCallBack callBack)`                                                                                                                            | 加入一个群，根据群设置可能需要管理员批准                       |
| `public inline void leave(final` [`BMXGroup`](broken-reference) `group,final BMXCallBack callBack)`                                                                                                                                                | 退出群                                        |
| `public inline void getInfo(final` [`BMXGroup`](broken-reference)`group,final BMXDataCallBack<`[`BMXGroup`](broken-reference) `> callBack)`                                                                                                        | 获取群详情，从服务端拉取最新信息                           |
| `public inline void getMembers(final` [`BMXGroup`](broken-reference)`group,final String cursor,final int pageSize,final BMXDataCallBack<`[`BMXGroupMemberResultPage`](broken-reference) `> callBack)`                                              | 获取群成员列表，如果设置了forceRefresh则从服务器拉取，最多拉取1000人 |
| `public inline void getMembers(final` [`BMXGroup`](broken-reference)`group,final boolean forceRefresh,final BMXDataCallBack<`[`BMXGroupMemberList`](broken-reference) `> callBack)`                                                                | 获取群成员列表，如果设置了forceRefresh则从服务器拉取，最多拉取1000人 |
| `public inline void addMembers(final` [`BMXGroup`](broken-reference)`group,final`[`ListOfLongLong`](broken-reference) `members,final String message,final BMXCallBack callBack)`                                                                   | 添加群成员                                      |
| `public inline void removeMembers(final` [`BMXGroup`](broken-reference)`group,final`[`ListOfLongLong`](broken-reference) `members,final String reason,final BMXCallBack callBack)`                                                                 | 删除群成员                                      |
| `public inline void addAdmins(final` [`BMXGroup`](broken-reference)`group,final`[`ListOfLongLong`](broken-reference) `admins,final String message,final BMXCallBack callBack)`                                                                     | 添加管理员                                      |
| `public inline void removeAdmins(final` [`BMXGroup`](broken-reference)`group,final`[`ListOfLongLong`](broken-reference) `admins,final String reason,final BMXCallBack callBack)`                                                                   | 删除管理员                                      |
| `public inline void getAdmins(final` [`BMXGroup`](broken-reference)`group,final boolean forceRefresh,final BMXDataCallBack<`[`BMXGroupMemberList`](broken-reference) `> callBack)`                                                                 | 获取Admins列表，如果设置了forceRefresh则从服务器拉取        |
| `public inline void blockMembers(final` [`BMXGroup`](broken-reference)`group,final`[`ListOfLongLong`](broken-reference) `members,final BMXCallBack callBack)`                                                                                      | 添加黑名单                                      |
| `public inline void unblockMembers(final` [`BMXGroup`](broken-reference)`group,final`[`ListOfLongLong`](broken-reference) `members,final BMXCallBack callBack)`                                                                                    | 从黑名单删除                                     |
| `public inline void getBlockList(final` [`BMXGroup`](broken-reference)`group,final String cursor,final int pageSize,final BMXDataCallBack<`[`BMXGroupMemberResultPage`](broken-reference) `> callBack)`                                            | 获取黑名单                                      |
| `public inline void getBlockList(final` [`BMXGroup`](broken-reference)`group,final boolean forceRefresh,final BMXDataCallBack<`[`BMXGroupMemberList`](broken-reference) `> callBack)`                                                              | 获取黑名单                                      |
| `public inline void banMembers(final` [`BMXGroup`](broken-reference)`group,final`[`ListOfLongLong`](broken-reference) `members,final long duration,final String reason,final BMXCallBack callBack)`                                                | 禁言                                         |
| `public inline void banGroup(final` [`BMXGroup`](broken-reference) `group,final long duration,final BMXCallBack callBack)`                                                                                                                         | 全员禁言                                       |
| `public inline void unbanMembers(final` [`BMXGroup`](broken-reference)`group,final`[`ListOfLongLong`](broken-reference) `members,final BMXCallBack callBack)`                                                                                      | 解除禁言                                       |
| `public inline void unbanGroup(final` [`BMXGroup`](broken-reference) `group,final BMXCallBack callBack)`                                                                                                                                           | 解除全员禁言                                     |
| `public inline void getBannedMembers(final` [`BMXGroup`](broken-reference)`group,final String cursor,final int pageSize,final BMXDataCallBack<`[`BMXGroupBannedMemberResultPage`](broken-reference) `> callBack)`                                  | 获取禁言列表                                     |
| `public inline void getBannedMembers(final` [`BMXGroup`](broken-reference)`group,final BMXDataCallBack<`[`BMXGroupBannedMemberList`](broken-reference) `> callBack)`                                                                               | 获取禁言列表                                     |
| `public inline void muteMessage(final` [`BMXGroup`](broken-reference) `group,final BMXGroup.MsgMuteMode mode,final BMXCallBack callBack)`                                                                                                          | 设置是否屏蔽群消息                                  |
| `public inline void acceptApplication(final` [`BMXGroup`](broken-reference) `group,final long applicantId,final BMXCallBack callBack)`                                                                                                             | 接受入群申请                                     |
| `public inline void declineApplication(final` [`BMXGroup`](broken-reference) `group,final long applicantId,final String reason,final BMXCallBack callBack)`                                                                                        | 拒绝入群申请                                     |
| `public inline void acceptInvitation(final` [`BMXGroup`](broken-reference) `group,final long inviter,final BMXCallBack callBack)`                                                                                                                  | 接受入群邀请                                     |
| `public inline void declineInvitation(final` [`BMXGroup`](broken-reference) `group,final long inviter,final BMXCallBack callBack)`                                                                                                                 | 拒绝入群邀请                                     |
| `public inline void transferOwner(final` [`BMXGroup`](broken-reference) `group,final long newOwnerId,final BMXCallBack callBack)`                                                                                                                  | 转移群主                                       |
| `public inline void uploadSharedFile(final` [`BMXGroup`](broken-reference)`group,final String filePath,final String displayName,final String extensionName,final`[`FileProgressListener`](broken-reference) `listener,final BMXCallBack callBack)` | 添加群共享文件                                    |
| `public inline void removeSharedFile(final` [`BMXGroup`](broken-reference) `group,final BMXGroup.SharedFile sharedFile,final BMXCallBack callBack)`                                                                                                | 移除群共享文件                                    |
| `public inline void downloadSharedFile(final` [`BMXGroup`](broken-reference)`group,final BMXGroup.SharedFile sharedFile,final`[`FileProgressListener`](broken-reference) `listener,final BMXCallBack callBack)`                                    | 下载群共享文件                                    |
| `public inline void getSharedFilesList(final` [`BMXGroup`](broken-reference)`group,final boolean forceRefresh,final BMXDataCallBack<`[`BMXGroupSharedFileList`](broken-reference) `> callBack)`                                                    | 获取群共享文件列表                                  |
| `public inline void changeSharedFileName(final` [`BMXGroup`](broken-reference) `group,final BMXGroup.SharedFile sharedFile,final String name,final BMXCallBack callBack)`                                                                          | 修改群共享文件名称                                  |
| `public inline void getLatestAnnouncement(final` [`BMXGroup`](broken-reference) `group,final boolean forceRefresh,final BMXDataCallBack< BMXGroup.Announcement > callBack)`                                                                        | 获取最新的群公告                                   |
| `public inline void getAnnouncementList(final` [`BMXGroup`](broken-reference)`group,final boolean forceRefresh,final BMXDataCallBack<`[`BMXGroupAnnouncementList`](broken-reference) `> callBack)`                                                 | 获取群公告列表                                    |
| `public inline void editAnnouncement(final` [`BMXGroup`](broken-reference) `group,final String title,final String content,final BMXCallBack callBack)`                                                                                             | 设置群公告                                      |
| `public inline void deleteAnnouncement(final` [`BMXGroup`](broken-reference) `group,final long announcementId,final BMXCallBack callBack)`                                                                                                         | 删除群公告                                      |
| `public inline void setName(final` [`BMXGroup`](broken-reference) `group,final String name,final BMXCallBack callBack)`                                                                                                                            | 设置群名称                                      |
| `public inline void setDescription(final` [`BMXGroup`](broken-reference) `group,final String description,final BMXCallBack callBack)`                                                                                                              | 设置群描述信息                                    |
| `public inline void setExtension(final` [`BMXGroup`](broken-reference) `group,final String extension,final BMXCallBack callBack)`                                                                                                                  | 设置群扩展信息                                    |
| `public inline void setMyNickname(final` [`BMXGroup`](broken-reference) `group,final String nickname,final BMXCallBack callBack)`                                                                                                                  | 设置在群里的昵称                                   |
| `public inline void setMsgPushMode(final` [`BMXGroup`](broken-reference) `group,final BMXGroup.MsgPushMode mode,final BMXCallBack callBack)`                                                                                                       | 设置群消息通知模式                                  |
| `public inline void setJoinAuthMode(final` [`BMXGroup`](broken-reference) `group,final BMXGroup.JoinAuthMode mode,final BMXCallBack callBack)`                                                                                                     | 设置入群审批模式                                   |
| `public inline void setInviteMode(final` [`BMXGroup`](broken-reference) `group,final BMXGroup.InviteMode mode,final BMXCallBack callBack)`                                                                                                         | 设置邀请模式                                     |
| `public inline void setAvatar(final` [`BMXGroup`](broken-reference)`group,final String avatarPath,final`[`FileProgressListener`](broken-reference) `listener,final BMXCallBack callBack)`                                                          | 设置群头像                                      |
| `public inline void downloadAvatar(final` [`BMXGroup`](broken-reference)`group,final`[`FileProgressListener`](broken-reference) `listener,final BMXCallBack callBack)`                                                                             | 下载群头像                                      |
| `public inline void addGroupListener(`[`BMXGroupServiceListener`](broken-reference) `listener)`                                                                                                                                                    | 添加群组变化监听者                                  |
| `public inline void removeGroupListener(`[`BMXGroupServiceListener`](broken-reference) `listener)`                                                                                                                                                 | 移除群组变化监听者                                  |
| `public inline void setEnableReadAck(final` [`BMXGroup`](broken-reference) `group,final boolean enable,final BMXCallBack callBack)`                                                                                                                | 设置是否开启群消息已读功能                              |

### Members

#### `public inline BMXGroupManager(`[`BMXGroupService`](broken-reference) `service)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a215616dd661aa69b33d82b3da5321be7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a215616dd661aa69b33d82b3da5321be7"></a>

#### `public inline void getGroupList(final boolean forceRefresh,final BMXDataCallBack<` [`BMXGroupList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1acb965f8e2c4b7e16d76db814f973a129" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1acb965f8e2c4b7e16d76db814f973a129"></a>

获取群组列表，如果设置了forceRefresh则从服务器拉取

**Parameters**

* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取
* `callBack` [BMXErrorCode](broken-reference),群组id列表

#### `public inline void getGroupList(final` [`ListOfLongLong`](broken-reference)`groupIdList,final boolean forceRefresh,final BMXDataCallBack<`[`BMXGroupList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1adb5d3971c59cf2a74ae367506d2c28ce" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1adb5d3971c59cf2a74ae367506d2c28ce"></a>

获取传入群组id的群组信息列表，如果设置了forceRefresh则从服务器拉取

**Parameters**

* `groupIdList` 群组id列表
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取
* `callBack` [BMXErrorCode](broken-reference),群组详细信息列表

#### `public inline void getGroupList(final long groupId,final boolean forceUpdate,final BMXDataCallBack<` [`BMXGroup`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a6b0c41f37e0b9accd673b7380c3e0f42" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a6b0c41f37e0b9accd673b7380c3e0f42"></a>

获取群信息，如果设置了forceRefresh则从服务器拉取

**Parameters**

* `groupId` 要搜索的群组id
* `forceUpdate` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取
* `callBack` [BMXErrorCode](broken-reference),搜索返回的群组信息

#### `public inline void getInvitationList(final String cursor,final int pageSize,final BMXDataCallBack<` [`GroupInvitaionPage`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a661522363e9de1d8561c941877bb1b2e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a661522363e9de1d8561c941877bb1b2e"></a>

分页获取群组邀请列表

**Parameters**

* `cursor` 分页获取的起始cursor，第一次传入为空，后续传入上次操作返回的result中的cursor
* `pageSize` 分页大小
* `callBack` [BMXErrorCode](broken-reference),分页获取的群组邀请列表

#### `public inline void getApplicationList(final` [`BMXGroupList`](broken-reference)`list,final String cursor,final int pageSize,final BMXDataCallBack<`[`GroupApplicationPage`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1ab98dc8d4e622210bff8d88031dd430fa" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1ab98dc8d4e622210bff8d88031dd430fa"></a>

分页获取群组申请列表

**Parameters**

* `list` 需要获取群组申请列表信息的群组id列表
* `cursor` 分页获取的起始cursor，第一次传入为空，后续传入上次操作返回的result中的cursor
* `pageSize` 分页大小
* `callBack` [BMXErrorCode](broken-reference),分页获取的群组申请列表

#### `public inline void create(final BMXGroupService.CreateGroupOptions options,final BMXDataCallBack<` [`BMXGroup`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1ad1fdc6e98470fe990811379ed1fc9228" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1ad1fdc6e98470fe990811379ed1fc9228"></a>

创建群

**Parameters**

* `options` 创建群组时传入的参数选项
* `callBack` [BMXErrorCode](broken-reference),创建好的群

#### `public inline void destroy(final` [`BMXGroup`](broken-reference) `group,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a3ff7e35bff176e52b770e867dd8f7d08" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a3ff7e35bff176e52b770e867dd8f7d08"></a>

销毁群

**Parameters**

* `callBack` BMXErrorCode，要销毁的群组

#### `public inline void join(final` [`BMXGroup`](broken-reference) `group,final String message,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a387a36b89a84dccfb8ee3ee0f4405c3d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a387a36b89a84dccfb8ee3ee0f4405c3d"></a>

加入一个群，根据群设置可能需要管理员批准

**Parameters**

* `group` 要加入的群组
* `message` 申请入群的信息
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void leave(final` [`BMXGroup`](broken-reference) `group,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1aa6dd475d441ff3c5b825decd565b054e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1aa6dd475d441ff3c5b825decd565b054e"></a>

退出群

**Parameters**

* `group` 要退出的群组
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void getInfo(final` [`BMXGroup`](broken-reference)`group,final BMXDataCallBack<`[`BMXGroup`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1aaccf7cb2ed5558c6285d20c0c0f3d813" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1aaccf7cb2ed5558c6285d20c0c0f3d813"></a>

获取群详情，从服务端拉取最新信息

**Parameters**

* `callBack` [BMXErrorCode](broken-reference),要获取群组最新信息的群组

#### `public inline void getMembers(final` [`BMXGroup`](broken-reference)`group,final String cursor,final int pageSize,final BMXDataCallBack<`[`BMXGroupMemberResultPage`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a3d1af91404d18c6051433f32563468d2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a3d1af91404d18c6051433f32563468d2"></a>

获取群成员列表，如果设置了forceRefresh则从服务器拉取，最多拉取1000人

**Parameters**

* `group` 进行操作的群组
* `cursor` 分页获取的起始cursor，第一次传入为空，后续传入上次操作返回的result中的cursor
* `pageSize` 分页大小
* `callBack` [BMXErrorCode](broken-reference),群成员列表

#### `public inline void getMembers(final` [`BMXGroup`](broken-reference)`group,final boolean forceRefresh,final BMXDataCallBack<`[`BMXGroupMemberList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a1a61e52c47e771ecd655e887852cd6b2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a1a61e52c47e771ecd655e887852cd6b2"></a>

获取群成员列表，如果设置了forceRefresh则从服务器拉取，最多拉取1000人

**Parameters**

* `group` 进行操作的群组
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取
* `callBack` [BMXErrorCode](broken-reference),群成员列表

#### `public inline void addMembers(final` [`BMXGroup`](broken-reference)`group,final`[`ListOfLongLong`](broken-reference) `members,final String message,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a7abf3ac496b7c0f6c28cf4ec1ffcd692" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a7abf3ac496b7c0f6c28cf4ec1ffcd692"></a>

添加群成员

**Parameters**

* `group` 进行操作的群组
* `members` 要添加进群的成员id列表
* `message` 添加成员原因信息
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void removeMembers(final` [`BMXGroup`](broken-reference)`group,final`[`ListOfLongLong`](broken-reference) `members,final String reason,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1afcba3c6fd93381d7d9c7a9f3825a7ac7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1afcba3c6fd93381d7d9c7a9f3825a7ac7"></a>

删除群成员

**Parameters**

* `group` 进行操作的群组
* `members` 要删除的群组成员id列表
* `reason` 删除的原因
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void addAdmins(final` [`BMXGroup`](broken-reference)`group,final`[`ListOfLongLong`](broken-reference) `admins,final String message,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a719575a9bc816ae182d69cf38936794f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a719575a9bc816ae182d69cf38936794f"></a>

添加管理员

**Parameters**

* `group` 进行操作的群组
* `admins` 要添加为管理员的成员id列表
* `message` 添加为管理员的原因
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void removeAdmins(final` [`BMXGroup`](broken-reference)`group,final`[`ListOfLongLong`](broken-reference) `admins,final String reason,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a5f80c667c78212faa373c651a86f35fb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a5f80c667c78212faa373c651a86f35fb"></a>

删除管理员

**Parameters**

* `group` 进行操作的群组
* `admins` 要从管理员移除的成员id列表
* `reason` 要移除管理员的原因
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void getAdmins(final` [`BMXGroup`](broken-reference)`group,final boolean forceRefresh,final BMXDataCallBack<`[`BMXGroupMemberList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a8b0715a7740fe6e15848fadf898faceb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a8b0715a7740fe6e15848fadf898faceb"></a>

获取Admins列表，如果设置了forceRefresh则从服务器拉取

**Parameters**

* `group` 进行操作的群组
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取
* `callBack` [BMXErrorCode](broken-reference),群管理员列表

#### `public inline void blockMembers(final` [`BMXGroup`](broken-reference)`group,final`[`ListOfLongLong`](broken-reference) `members,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1aa107c6f83ebe8bb02e142d75e0396299" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1aa107c6f83ebe8bb02e142d75e0396299"></a>

添加黑名单

**Parameters**

* `group` 进行操作的群组
* `members` 要加入黑名单的群成员id列表
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void unblockMembers(final` [`BMXGroup`](broken-reference)`group,final`[`ListOfLongLong`](broken-reference) `members,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a099e715fc4644183afb88ffe2ef3c617" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a099e715fc4644183afb88ffe2ef3c617"></a>

从黑名单删除

**Parameters**

* `group` 进行操作的群组
* `members` 从黑名单移除的用户id列表
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void getBlockList(final` [`BMXGroup`](broken-reference)`group,final String cursor,final int pageSize,final BMXDataCallBack<`[`BMXGroupMemberResultPage`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a165b4274dd55698b518f37ea79eaf900" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a165b4274dd55698b518f37ea79eaf900"></a>

获取黑名单

**Parameters**

* `group` 进行操作的群组
* `cursor` 分页获取的起始cursor，第一次传入为空，后续传入上次操作返回的result中的cursor
* `pageSize` 分页大小
* `callBack` [BMXErrorCode](broken-reference),群黑名单列表

#### `public inline void getBlockList(final` [`BMXGroup`](broken-reference)`group,final boolean forceRefresh,final BMXDataCallBack<`[`BMXGroupMemberList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a01cd7b7e51bd659ce7b65483805aa3ad" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a01cd7b7e51bd659ce7b65483805aa3ad"></a>

获取黑名单

**Parameters**

* `group` 进行操作的群组
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取
* `callBack` [BMXErrorCode](broken-reference),群黑名单列表

#### `public inline void banMembers(final` [`BMXGroup`](broken-reference)`group,final`[`ListOfLongLong`](broken-reference) `members,final long duration,final String reason,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1aeb6d28f913c76b231c53cae1ad159496" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1aeb6d28f913c76b231c53cae1ad159496"></a>

禁言

**Parameters**

* `group` 进行操作的群组
* `members` 被禁言的群成员id列表
* `duration` 禁言时长
* `reason` 禁言原因
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void banGroup(final` [`BMXGroup`](broken-reference) `group,final long duration,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a9370b0d1d54d589a894f8fd577c1ae4e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a9370b0d1d54d589a894f8fd577c1ae4e"></a>

全员禁言

**Parameters**

* `group` 进行操作的群组
* `duration` 禁言时长
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void unbanMembers(final` [`BMXGroup`](broken-reference)`group,final`[`ListOfLongLong`](broken-reference) `members,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1af29dc2a5e3f8ae3505c9390d4fbe6853" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1af29dc2a5e3f8ae3505c9390d4fbe6853"></a>

解除禁言

**Parameters**

* `group` 进行操作的群组
* `members` 被解除禁言的群成员id列表
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void unbanGroup(final` [`BMXGroup`](broken-reference) `group,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1aecb6ed3b231df9e2692558d9fe224739" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1aecb6ed3b231df9e2692558d9fe224739"></a>

解除全员禁言

**Parameters**

* `group` 进行操作的群组
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void getBannedMembers(final` [`BMXGroup`](broken-reference)`group,final String cursor,final int pageSize,final BMXDataCallBack<`[`BMXGroupBannedMemberResultPage`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a5d80b271d3a0ebfa3df247c659d8d3ca" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a5d80b271d3a0ebfa3df247c659d8d3ca"></a>

获取禁言列表

**Parameters**

* `group` 进行操作的群组
* `cursor` 分页获取的起始cursor，第一次传入为空，后续传入上次操作返回的result中的cursor
* `pageSize` 分页大小
* `callBack` [BMXErrorCode](broken-reference) 群禁言列表

#### `public inline void getBannedMembers(final` [`BMXGroup`](broken-reference)`group,final BMXDataCallBack<`[`BMXGroupBannedMemberList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a7928ca6e4d04250e0d0947b57b33f191" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a7928ca6e4d04250e0d0947b57b33f191"></a>

获取禁言列表

**Parameters**

* `group` 进行操作的群组
* `callBack` [BMXErrorCode](broken-reference) 群禁言列表

#### `public inline void muteMessage(final` [`BMXGroup`](broken-reference) `group,final BMXGroup.MsgMuteMode mode,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a922678a40303aa6dc627caa3a4d95ca6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a922678a40303aa6dc627caa3a4d95ca6"></a>

设置是否屏蔽群消息

**Parameters**

* `group` 进行操作的群组
* `mode` 群屏蔽的模式
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void acceptApplication(final` [`BMXGroup`](broken-reference) `group,final long applicantId,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a8d430fbc26e24718d9ddcf9c70dc157b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a8d430fbc26e24718d9ddcf9c70dc157b"></a>

接受入群申请

**Parameters**

* `group` 进行操作的群组
* `applicantId` 申请进群的用户id
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void declineApplication(final` [`BMXGroup`](broken-reference) `group,final long applicantId,final String reason,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a446513b1111a1ab602bad07fcfa8917d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a446513b1111a1ab602bad07fcfa8917d"></a>

拒绝入群申请

**Parameters**

* `group` 进行操作的群组
* `applicantId` 申请进群的用户id
* `reason` 拒绝的原因
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void acceptInvitation(final` [`BMXGroup`](broken-reference) `group,final long inviter,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a1dd17ff86f5914f5db4a6a4e270270b5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a1dd17ff86f5914f5db4a6a4e270270b5"></a>

接受入群邀请

**Parameters**

* `group` 进行操作的群组
* `inviter` 邀请者id
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void declineInvitation(final` [`BMXGroup`](broken-reference) `group,final long inviter,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a83d96aac9a10031cf05a860e73ca15ce" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a83d96aac9a10031cf05a860e73ca15ce"></a>

拒绝入群邀请

**Parameters**

* `group` 进行操作的群组
* `inviter` 邀请者id
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void transferOwner(final` [`BMXGroup`](broken-reference) `group,final long newOwnerId,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a8277a29704a4c77d7c7d7d94b7229db1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a8277a29704a4c77d7c7d7d94b7229db1"></a>

转移群主

**Parameters**

* `group` 进行操作的群组
* `newOwnerId` 转让为新群主的用户id
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void uploadSharedFile(final` [`BMXGroup`](broken-reference)`group,final String filePath,final String displayName,final String extensionName,final`[`FileProgressListener`](broken-reference) `listener,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1abe2f47c66a422d0a13970801d4916661" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1abe2f47c66a422d0a13970801d4916661"></a>

添加群共享文件

**Parameters**

* `group` 进行操作的群组
* `filePath` 文件的本地路径
* `displayName` 文件的展示名
* `extensionName` 文件的扩展名
* `listener` 上传回调函数
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void removeSharedFile(final` [`BMXGroup`](broken-reference) `group,final BMXGroup.SharedFile sharedFile,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a3f05970d391efffcab7bcfa9691d8f7d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a3f05970d391efffcab7bcfa9691d8f7d"></a>

移除群共享文件

**Parameters**

* `group` 进行操作的群组
* `sharedFile` 删除的群共享文件
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void downloadSharedFile(final` [`BMXGroup`](broken-reference)`group,final BMXGroup.SharedFile sharedFile,final`[`FileProgressListener`](broken-reference) `listener,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1ae8e8ab418b8cac8b7ad9dc75fdbbb335" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1ae8e8ab418b8cac8b7ad9dc75fdbbb335"></a>

下载群共享文件

**Parameters**

* `group` 进行操作的群组
* `sharedFile` 下载的群共享文件
* `listener` 下载回调函数
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void getSharedFilesList(final` [`BMXGroup`](broken-reference)`group,final boolean forceRefresh,final BMXDataCallBack<`[`BMXGroupSharedFileList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a4ffe822892c7aedfdedf201ed44489a2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a4ffe822892c7aedfdedf201ed44489a2"></a>

获取群共享文件列表

**Parameters**

* `group` 进行操作的群组
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取
* `callBack` [BMXErrorCode](broken-reference) 群共享文件列表

#### `public inline void changeSharedFileName(final` [`BMXGroup`](broken-reference) `group,final BMXGroup.SharedFile sharedFile,final String name,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a9cbd608e7d11d78319838a208b1111bc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a9cbd608e7d11d78319838a208b1111bc"></a>

修改群共享文件名称

**Parameters**

* `group` 进行操作的群组
* `sharedFile` 进行更改的群共享文件
* `name` 修改的群共享文件名称
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void getLatestAnnouncement(final` [`BMXGroup`](broken-reference) `group,final boolean forceRefresh,final BMXDataCallBack< BMXGroup.Announcement > callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a845b5a78d3ee780f681f246c61b20ef9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a845b5a78d3ee780f681f246c61b20ef9"></a>

获取最新的群公告

**Parameters**

* `group` 进行操作的群组
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取
* `callBack` [BMXErrorCode](broken-reference) 最新的群组公告

#### `public inline void getAnnouncementList(final` [`BMXGroup`](broken-reference)`group,final boolean forceRefresh,final BMXDataCallBack<`[`BMXGroupAnnouncementList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1aa25134a1474d54fa38f21377726df7ba" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1aa25134a1474d54fa38f21377726df7ba"></a>

获取群公告列表

**Parameters**

* `group` 进行操作的群组
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取
* `callBack` [BMXErrorCode](broken-reference), 群公告列表

#### `public inline void editAnnouncement(final` [`BMXGroup`](broken-reference) `group,final String title,final String content,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a86ffc1b279cbf0e060e968f0994867e6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a86ffc1b279cbf0e060e968f0994867e6"></a>

设置群公告

**Parameters**

* `group` 进行操作的群组
* `title` 群公告的标题
* `content` 群公告的内容
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void deleteAnnouncement(final` [`BMXGroup`](broken-reference) `group,final long announcementId,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1ab72553b64e933968ee9349809b8b93b0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1ab72553b64e933968ee9349809b8b93b0"></a>

删除群公告

**Parameters**

* `group` 进行操作的群组
* `announcementId` 删除的群公告id
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setName(final` [`BMXGroup`](broken-reference) `group,final String name,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a8c5c230037d305d803560b00274f0481" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a8c5c230037d305d803560b00274f0481"></a>

设置群名称

**Parameters**

* `group` 进行操作的群组
* `name` 群组名称
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setDescription(final` [`BMXGroup`](broken-reference) `group,final String description,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a3fad5341adf4d5ed20570089fef84578" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a3fad5341adf4d5ed20570089fef84578"></a>

设置群描述信息

**Parameters**

* `group` 进行操作的群组
* `description` 群组描述
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setExtension(final` [`BMXGroup`](broken-reference) `group,final String extension,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a6554e928487a9a4141a0738bedf0ac16" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a6554e928487a9a4141a0738bedf0ac16"></a>

设置群扩展信息

**Parameters**

* `group` 进行操作的群组
* `extension` 群组的扩展信息
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setMyNickname(final` [`BMXGroup`](broken-reference) `group,final String nickname,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a6d4a56af61d44c598eb1a62b517e7dc5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a6d4a56af61d44c598eb1a62b517e7dc5"></a>

设置在群里的昵称

**Parameters**

* `group` 进行操作的群组
* `nickname` 用户在群组内的昵称
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setMsgPushMode(final` [`BMXGroup`](broken-reference) `group,final BMXGroup.MsgPushMode mode,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a60e322f087e6eb8dd0693b66cf0b7aca" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a60e322f087e6eb8dd0693b66cf0b7aca"></a>

设置群消息通知模式

**Parameters**

* `group` 进行操作的群组
* `mode` 群消息通知模式
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setJoinAuthMode(final` [`BMXGroup`](broken-reference) `group,final BMXGroup.JoinAuthMode mode,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1afe1b2427787b112bca76b46dbf84ff4b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1afe1b2427787b112bca76b46dbf84ff4b"></a>

设置入群审批模式

**Parameters**

* `group` 进行操作的群组
* `mode` 入群审批模式
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setInviteMode(final` [`BMXGroup`](broken-reference) `group,final BMXGroup.InviteMode mode,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a93dce028a2705bbdc87a72058bdc21f9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a93dce028a2705bbdc87a72058bdc21f9"></a>

设置邀请模式

**Parameters**

* `group` 进行操作的群组
* `mode` 群组的邀请模式
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setAvatar(final` [`BMXGroup`](broken-reference)`group,final String avatarPath,final`[`FileProgressListener`](broken-reference) `listener,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a07fee35b6afb88b7ac8d56947dc47a5d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a07fee35b6afb88b7ac8d56947dc47a5d"></a>

设置群头像

**Parameters**

* `group` 进行操作的群组
* `avatarPath` 群头像文件的本地路径
* `listener` 上传回调函数
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void downloadAvatar(final` [`BMXGroup`](broken-reference)`group,final`[`FileProgressListener`](broken-reference) `listener,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a35341d74d2bb0ff1b065186dd46f7bd3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a35341d74d2bb0ff1b065186dd46f7bd3"></a>

下载群头像

**Parameters**

* `group` 进行操作的群组
* `listener` 下载回调函数
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void addGroupListener(`[`BMXGroupServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a5fa76db27a42dedaf28a8dd6877734ca" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a5fa76db27a42dedaf28a8dd6877734ca"></a>

添加群组变化监听者

**Parameters**

* `listener` 群组变化监听者

#### `public inline void removeGroupListener(`[`BMXGroupServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a74c85ecba7d2a3be95a530a653dfe4b5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a74c85ecba7d2a3be95a530a653dfe4b5"></a>

移除群组变化监听者

**Parameters**

* `listener` 群组变化监听者

#### `public inline void setEnableReadAck(final` [`BMXGroup`](broken-reference) `group,final boolean enable,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a0bd5f50d5c2e1c9074d0eea9349e4198" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_manager_1a0bd5f50d5c2e1c9074d0eea9349e4198"></a>

设置是否开启群消息已读功能

**Parameters**

* `group` 进行操作的群组
* `enable` 是否开启
* `callBack` [BMXErrorCode](broken-reference)

## class `BMXGroupMemberList` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list"></a>

### Summary

| Members                                                             | Descriptions |
| ------------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                          |              |
| `public inline BMXGroupMemberList()`                                |              |
| `public inline BMXGroupMemberList(long n)`                          |              |
| `public inline long size()`                                         |              |
| `public inline long capacity()`                                     |              |
| `public inline void reserve(long n)`                                |              |
| `public inline boolean isEmpty()`                                   |              |
| `public inline void clear()`                                        |              |
| `public inline void add(BMXGroup.Member x)`                         |              |
| `public inline BMXGroup.Member get(int i)`                          |              |
| `public inline void set(int i,BMXGroup.Member val)`                 |              |
| `protected transient boolean swigCMemOwn`                           |              |
| `protected inline BMXGroupMemberList(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                                  |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1a4d6cf5bf55f1024ca671a34b41efa674" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1a4d6cf5bf55f1024ca671a34b41efa674"></a>

#### `public inline BMXGroupMemberList()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1a7a442f47a7ea4aeeaebdc081e6f1ef0b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1a7a442f47a7ea4aeeaebdc081e6f1ef0b"></a>

#### `public inline BMXGroupMemberList(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1abbe661dc0739009634cb1c5d59c47d96" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1abbe661dc0739009634cb1c5d59c47d96"></a>

#### `public inline long size()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1a0e7f446ca474189f0b2715abca975bdd" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1a0e7f446ca474189f0b2715abca975bdd"></a>

#### `public inline long capacity()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1a765cce03d5261c251eb62b4de5d1c1eb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1a765cce03d5261c251eb62b4de5d1c1eb"></a>

#### `public inline void reserve(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1ad462125d7b55e545406fcb86ad40357f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1ad462125d7b55e545406fcb86ad40357f"></a>

#### `public inline boolean isEmpty()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1a4dea5a6deeae39d78df7406e57d4a008" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1a4dea5a6deeae39d78df7406e57d4a008"></a>

#### `public inline void clear()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1a41fa69236c3288335b47cb1d64eb138a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1a41fa69236c3288335b47cb1d64eb138a"></a>

#### `public inline void add(BMXGroup.Member x)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1aba254762b4a7f0bd456659257328f15a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1aba254762b4a7f0bd456659257328f15a"></a>

#### `public inline BMXGroup.Member get(int i)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1ac8a828ea8a15a6532c0cc3de6d6e3141" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1ac8a828ea8a15a6532c0cc3de6d6e3141"></a>

#### `public inline void set(int i,BMXGroup.Member val)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1aca43471633703ebcdfef7f0419ad2d60" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1aca43471633703ebcdfef7f0419ad2d60"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1aa0dbb5d85532f51341f1a24c636ee426" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1aa0dbb5d85532f51341f1a24c636ee426"></a>

#### `protected inline BMXGroupMemberList(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1ae20e73e82cdbcece419f0b044e887766" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1ae20e73e82cdbcece419f0b044e887766"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1aaaf153ddd3d433ab0d967774958da55d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_list_1aaaf153ddd3d433ab0d967774958da55d"></a>

## class `BMXGroupMemberResultPage` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page"></a>

```
class BMXGroupMemberResultPage
  : public im.floo.floolib.BMXBaseObject
```

### Summary

| Members                                                                                                   | Descriptions |
| --------------------------------------------------------------------------------------------------------- | ------------ |
| `public transient long swigCPtr`                                                                          |              |
| `public inline synchronized void delete()`                                                                |              |
| `public inline BMXGroupMemberResultPage()`                                                                |              |
| `public inline BMXGroupMemberResultPage(`[`BMXGroupMemberList`](broken-reference) `result,long offset)`   |              |
| `public inline BMXGroupMemberResultPage(`[`BMXGroupMemberList`](broken-reference) `result,String cursor)` |              |
| `public inline BMXGroupMemberResultPage(`[`BMXGroupMemberResultPage`](broken-reference) `from)`           |              |
| `public inline long count()`                                                                              |              |
| `public inline long offset()`                                                                             |              |
| `public inline String cursor()`                                                                           |              |
| `public inline` [`BMXGroupMemberList`](broken-reference) `result()`                                       |              |
| `protected inline BMXGroupMemberResultPage(long cPtr,boolean cMemoryOwn)`                                 |              |
| `protected inline void finalize()`                                                                        |              |

### Members

#### `public transient long swigCPtr` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1a3e69291c2f1096b5aefffc13b4987d80" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1a3e69291c2f1096b5aefffc13b4987d80"></a>

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1aee0c741590f51003ef62016d21157c18" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1aee0c741590f51003ef62016d21157c18"></a>

#### `public inline BMXGroupMemberResultPage()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1af7c6696ba14756884bef1de01ecbbb2f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1af7c6696ba14756884bef1de01ecbbb2f"></a>

#### `public inline BMXGroupMemberResultPage(`[`BMXGroupMemberList`](broken-reference) `result,long offset)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1a506f00717673689ffebfc52ae94f5ca4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1a506f00717673689ffebfc52ae94f5ca4"></a>

#### `public inline BMXGroupMemberResultPage(`[`BMXGroupMemberList`](broken-reference) `result,String cursor)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1a1d7aa5d2eded06d1689b4c9c643356c5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1a1d7aa5d2eded06d1689b4c9c643356c5"></a>

#### `public inline BMXGroupMemberResultPage(`[`BMXGroupMemberResultPage`](broken-reference) `from)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1a0861bed8f34f63317637f533e0097fed" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1a0861bed8f34f63317637f533e0097fed"></a>

#### `public inline long count()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1a457503a3c36adc004382414c5b043dcc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1a457503a3c36adc004382414c5b043dcc"></a>

#### `public inline long offset()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1aa6aea6f68da34eea5e9eb41473086233" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1aa6aea6f68da34eea5e9eb41473086233"></a>

#### `public inline String cursor()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1aceffe89e8b3ec836b2998e27ed2889c5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1aceffe89e8b3ec836b2998e27ed2889c5"></a>

#### `public inline` [`BMXGroupMemberList`](broken-reference) `result()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1afa574db986dbc41794e327621d7bcdbe" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1afa574db986dbc41794e327621d7bcdbe"></a>

#### `protected inline BMXGroupMemberResultPage(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1addbeb52ca5cd3a00f337392bde5ea494" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1addbeb52ca5cd3a00f337392bde5ea494"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1a5c9cfbc10afe63f25475b623c1ea4493" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_member_result_page_1a5c9cfbc10afe63f25475b623c1ea4493"></a>

## class `BMXGroupService` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service"></a>

群组Service

### Summary

| Members                                                                                                                                                                                                                 | Descriptions                                   |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| `class` [`CreateGroupOptions`](broken-reference)                                                                                                                                                                        | 创建群组选项                                         |
| `public inline synchronized void delete()`                                                                                                                                                                              |                                                |
| `public inline` [`BMXErrorCode`](broken-reference) `get(`[`BMXGroupList`](broken-reference) `list,boolean forceRefresh)`                                                                                                | 获取群组列表，如果设置了forceRefresh则从服务器拉取                |
| `public inline` [`BMXErrorCode`](broken-reference) `search(`[`BMXGroupList`](broken-reference) `list,boolean forceRefresh)`                                                                                             | 获取群组列表，如果设置了forceRefresh则从服务器拉取                |
| `public inline` [`BMXErrorCode`](broken-reference) `fetchGroupsByIdList(`[`ListOfLongLong`](broken-reference) `groupIdList,`[`BMXGroupList`](broken-reference) `list,boolean forceRefresh)`                             | 获取传入群组id的群组信息列表，如果设置了forceRefresh则从服务器拉取       |
| `public inline` [`BMXErrorCode`](broken-reference) `search(`[`ListOfLongLong`](broken-reference) `groupIdList,`[`BMXGroupList`](broken-reference) `list,boolean forceRefresh)`                                          | 获取传入群组id的群组信息列表，如果设置了forceRefresh则从服务器拉取       |
| `public inline` [`BMXErrorCode`](broken-reference) `fetchGroupById(long groupId,`[`BMXGroup`](broken-reference) `group,boolean forceRefresh)`                                                                           | 获取群信息，如果设置了forceRefresh则从服务器拉取                 |
| `public inline` [`BMXErrorCode`](broken-reference) `search(long groupId,`[`BMXGroup`](broken-reference) `group,boolean forceUpdate)`                                                                                    | 获取群信息，如果设置了forceRefresh则从服务器拉取                 |
| `public inline` [`BMXErrorCode`](broken-reference) `fetchLocalGroupsByName(`[`BMXGroupList`](broken-reference) `list,String name)`                                                                                      | 通过群名称查询本地群信息，从本地数据库中通过群名称查询获取群组                |
| `public inline` [`BMXErrorCode`](broken-reference) `search(`[`BMXGroupList`](broken-reference) `list,String name)`                                                                                                      | 通过群名称查询本地群信息，从本地数据库中通过群名称查询获取群组                |
| `public inline` [`BMXErrorCode`](broken-reference) `create(BMXGroupService.CreateGroupOptions options,`[`BMXGroup`](broken-reference) `group)`                                                                          | 创建群                                            |
| `public inline` [`BMXErrorCode`](broken-reference) `destroy(`[`BMXGroup`](broken-reference) `group)`                                                                                                                    | 销毁群                                            |
| `public inline` [`BMXErrorCode`](broken-reference) `join(`[`BMXGroup`](broken-reference) `group,String message)`                                                                                                        | 加入一个群，根据群设置可能需要管理员批准                           |
| `public inline` [`BMXErrorCode`](broken-reference) `leave(`[`BMXGroup`](broken-reference) `group)`                                                                                                                      | 退出群                                            |
| `public inline` [`BMXErrorCode`](broken-reference) `getInfo(`[`BMXGroup`](broken-reference) `group)`                                                                                                                    | 获取群详情，从服务端拉取最新信息                               |
| `public inline` [`BMXErrorCode`](broken-reference) `getMembersNickname(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members,`[`BMXGroupMemberList`](broken-reference) `list)`          | 获取群组成员详细信息                                     |
| `public inline` [`BMXErrorCode`](broken-reference) `getInvitationList(`[`GroupInvitaionPage`](broken-reference) `result,String cursor,int pageSize)`                                                                    | 分页获取群组邀请列表                                     |
| `public inline` [`BMXErrorCode`](broken-reference) `getApplicationList(`[`BMXGroupList`](broken-reference) `list,`[`GroupApplicationPage`](broken-reference) `result,String cursor,int pageSize)`                       | 分页获取群组申请列表                                     |
| `public inline` [`BMXErrorCode`](broken-reference) `getMembers(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupMemberResultPage`](broken-reference) `result,String cursor,int pageSize)`                              | 分页获取群成员列表，如果设置了forceRefresh则从服务器拉取，单页最大数量为500. |
| `public inline` [`BMXErrorCode`](broken-reference) `getMembers(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupMemberList`](broken-reference) `list,boolean forceRefresh)`                                            | 获取群成员列表，如果设置了forceRefresh则从服务器拉取，最多拉取1000人     |
| `public inline` [`BMXErrorCode`](broken-reference) `addMembers(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members,String message)`                                                   | 添加群成员                                          |
| `public inline` [`BMXErrorCode`](broken-reference) `removeMembers(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members,String reason)`                                                 | 删除群成员                                          |
| `public inline` [`BMXErrorCode`](broken-reference) `addAdmins(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `admins,String message)`                                                     | 添加管理员                                          |
| `public inline` [`BMXErrorCode`](broken-reference) `removeAdmins(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `admins,String reason)`                                                   | 删除管理员                                          |
| `public inline` [`BMXErrorCode`](broken-reference) `getAdmins(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupMemberList`](broken-reference) `list,boolean forceRefresh)`                                             | 获取Admins列表，如果设置了forceRefresh则从服务器拉取            |
| `public inline` [`BMXErrorCode`](broken-reference) `blockMembers(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members)`                                                                | 添加黑名单                                          |
| `public inline` [`BMXErrorCode`](broken-reference) `unblockMembers(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members)`                                                              | 从黑名单删除                                         |
| `public inline` [`BMXErrorCode`](broken-reference) `getBlockList(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupMemberResultPage`](broken-reference) `result,String cursor,int pageSize)`                            | 分页获取黑名单                                        |
| `public inline` [`BMXErrorCode`](broken-reference) `getBlockList(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupMemberList`](broken-reference) `list,boolean forceRefresh)`                                          | 获取黑名单                                          |
| `public inline` [`BMXErrorCode`](broken-reference) `banMembers(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members,long duration,String reason)`                                      | 禁言                                             |
| `public inline` [`BMXErrorCode`](broken-reference) `banMembers(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members,long duration)`                                                    |                                                |
| `public inline` [`BMXErrorCode`](broken-reference) `banGroup(`[`BMXGroup`](broken-reference) `group,long duration)`                                                                                                     | 全员禁言，当前服务器时间加上禁言时长后计算出全员禁言到期时间（只有管理和群主可以发言）    |
| `public inline` [`BMXErrorCode`](broken-reference) `unbanMembers(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members)`                                                                | 解除禁言                                           |
| `public inline` [`BMXErrorCode`](broken-reference) `unbanGroup(`[`BMXGroup`](broken-reference) `group)`                                                                                                                 | 全员解除禁言                                         |
| `public inline` [`BMXErrorCode`](broken-reference) `getBannedMembers(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupBannedMemberResultPage`](broken-reference) `result,String cursor,int pageSize)`                  | 分页获取禁言列表                                       |
| `public inline` [`BMXErrorCode`](broken-reference) `getBannedMembers(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupBannedMemberList`](broken-reference) `list)`                                                     | 获取禁言列表                                         |
| `public inline` [`BMXErrorCode`](broken-reference) `muteMessage(`[`BMXGroup`](broken-reference) `group,BMXGroup.MsgMuteMode mode)`                                                                                      | 设置是否屏蔽群消息                                      |
| `public inline` [`BMXErrorCode`](broken-reference) `acceptApplication(`[`BMXGroup`](broken-reference) `group,long applicantId)`                                                                                         | 接受入群申请                                         |
| `public inline` [`BMXErrorCode`](broken-reference) `declineApplication(`[`BMXGroup`](broken-reference) `group,long applicantId,String reason)`                                                                          | 拒绝入群申请                                         |
| `public inline` [`BMXErrorCode`](broken-reference) `declineApplication(`[`BMXGroup`](broken-reference) `group,long applicantId)`                                                                                        |                                                |
| `public inline` [`BMXErrorCode`](broken-reference) `acceptInvitation(`[`BMXGroup`](broken-reference) `group,long inviter)`                                                                                              | 接受入群邀请                                         |
| `public inline` [`BMXErrorCode`](broken-reference) `declineInvitation(`[`BMXGroup`](broken-reference) `group,long inviter,String reason)`                                                                               | 拒绝入群邀请                                         |
| `public inline` [`BMXErrorCode`](broken-reference) `declineInvitation(`[`BMXGroup`](broken-reference) `group,long inviter)`                                                                                             |                                                |
| `public inline` [`BMXErrorCode`](broken-reference) `transferOwner(`[`BMXGroup`](broken-reference) `group,long newOwnerId)`                                                                                              | 转移群主                                           |
| `public inline` [`BMXErrorCode`](broken-reference) `uploadSharedFile(`[`BMXGroup`](broken-reference) `group,String filePath,String displayName,String extensionName,`[`FileProgressListener`](broken-reference) `arg4)` | 添加群共享文件                                        |
| `public inline` [`BMXErrorCode`](broken-reference) `cancelUploadSharedFile(`[`BMXGroup`](broken-reference) `group,String filePath)`                                                                                     | 取消上传群共享文件                                      |
| `public inline` [`BMXErrorCode`](broken-reference) `removeSharedFile(`[`BMXGroup`](broken-reference) `group,BMXGroup.SharedFile sharedFile)`                                                                            | 移除群共享文件                                        |
| `public inline` [`BMXErrorCode`](broken-reference) `downloadSharedFile(`[`BMXGroup`](broken-reference) `group,BMXGroup.SharedFile sharedFile,`[`FileProgressListener`](broken-reference) `arg2)`                        | 下载群共享文件                                        |
| `public inline` [`BMXErrorCode`](broken-reference) `cancelDownloadSharedFile(`[`BMXGroup`](broken-reference) `group,BMXGroup.SharedFile sharedFile)`                                                                    | 取消下载群共享文件                                      |
| `public inline` [`BMXErrorCode`](broken-reference) `getSharedFilesList(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupSharedFileList`](broken-reference) `list,boolean forceRefresh)`                                | 获取群共享文件列表                                      |
| `public inline` [`BMXErrorCode`](broken-reference) `changeSharedFileName(`[`BMXGroup`](broken-reference) `group,BMXGroup.SharedFile sharedFile,String name)`                                                            | 修改群共享文件名称                                      |
| `public inline` [`BMXErrorCode`](broken-reference) `getLatestAnnouncement(`[`BMXGroup`](broken-reference) `group,BMXGroup.Announcement announcement,boolean forceRefresh)`                                              | 获取最新的群公告                                       |
| `public inline` [`BMXErrorCode`](broken-reference) `getAnnouncementList(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupAnnouncementList`](broken-reference) `list,boolean forceRefresh)`                             | 获取群公告列表                                        |
| `public inline` [`BMXErrorCode`](broken-reference) `editAnnouncement(`[`BMXGroup`](broken-reference) `group,String title,String content)`                                                                               | 设置群公告                                          |
| `public inline` [`BMXErrorCode`](broken-reference) `deleteAnnouncement(`[`BMXGroup`](broken-reference) `group,long announcementId)`                                                                                     | 删除群公告                                          |
| `public inline` [`BMXErrorCode`](broken-reference) `setName(`[`BMXGroup`](broken-reference) `group,String name)`                                                                                                        | 设置群名称                                          |
| `public inline` [`BMXErrorCode`](broken-reference) `setDescription(`[`BMXGroup`](broken-reference) `group,String description)`                                                                                          | 设置群描述信息                                        |
| `public inline` [`BMXErrorCode`](broken-reference) `setExtension(`[`BMXGroup`](broken-reference) `group,String extension)`                                                                                              | 设置群扩展信息                                        |
| `public inline` [`BMXErrorCode`](broken-reference) `setMyNickname(`[`BMXGroup`](broken-reference) `group,String nickname)`                                                                                              | 设置在群里的昵称                                       |
| `public inline` [`BMXErrorCode`](broken-reference) `setMsgPushMode(`[`BMXGroup`](broken-reference) `group,BMXGroup.MsgPushMode mode)`                                                                                   | 设置群消息通知模式                                      |
| `public inline` [`BMXErrorCode`](broken-reference) `setJoinAuthMode(`[`BMXGroup`](broken-reference) `group,BMXGroup.JoinAuthMode mode)`                                                                                 | 设置入群审批模式                                       |
| `public inline` [`BMXErrorCode`](broken-reference) `setInviteMode(`[`BMXGroup`](broken-reference) `group,BMXGroup.InviteMode mode)`                                                                                     | 设置邀请模式                                         |
| `public inline` [`BMXErrorCode`](broken-reference) `setAllowMemberModify(`[`BMXGroup`](broken-reference) `group,boolean enable)`                                                                                        | 设置是否允许群成员设置群信息                                 |
| `public inline` [`BMXErrorCode`](broken-reference) `setEnableReadAck(`[`BMXGroup`](broken-reference) `group,boolean enable)`                                                                                            | 设置是否开启群消息已读功能                                  |
| `public inline` [`BMXErrorCode`](broken-reference) `setHistoryVisible(`[`BMXGroup`](broken-reference) `group,boolean enable)`                                                                                           | 设置群成员是否开可见群历史聊天记录                              |
| `public inline` [`BMXErrorCode`](broken-reference) `setAvatar(`[`BMXGroup`](broken-reference) `group,String avatarPath,`[`FileProgressListener`](broken-reference) `arg2)`                                              | 设置群头像                                          |
| `public inline` [`BMXErrorCode`](broken-reference) `downloadAvatar(`[`BMXGroup`](broken-reference) `group,boolean thumbnail,`[`FileProgressListener`](broken-reference) `arg2)`                                         | 下载群头像                                          |
| `public inline void addGroupListener(`[`BMXGroupServiceListener`](broken-reference) `listener)`                                                                                                                         | 添加群组变化监听者                                      |
| `public inline void removeGroupListener(`[`BMXGroupServiceListener`](broken-reference) `listener)`                                                                                                                      | 移除群组变化监听者                                      |
| `protected transient boolean swigCMemOwn`                                                                                                                                                                               |                                                |
| `protected inline BMXGroupService(long cPtr,boolean cMemoryOwn)`                                                                                                                                                        |                                                |
| `protected inline void finalize()`                                                                                                                                                                                      |                                                |

### Members

#### `class` [`CreateGroupOptions`](broken-reference) <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options"></a>

创建群组选项

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a360c27037cee40c913bf8f1637c1a918" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a360c27037cee40c913bf8f1637c1a918"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `get(`[`BMXGroupList`](broken-reference) `list,boolean forceRefresh)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a9f848c46fe6f16eb42eb12d088d1ae19" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a9f848c46fe6f16eb42eb12d088d1ae19"></a>

获取群组列表，如果设置了forceRefresh则从服务器拉取

**Parameters**

* `list` 群组id列表，传入空列表函数返回后从此处获取返回的群组id列表
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `search(`[`BMXGroupList`](broken-reference) `list,boolean forceRefresh)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a96d461969e5ae13ca961cf3e9d7447f1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a96d461969e5ae13ca961cf3e9d7447f1"></a>

获取群组列表，如果设置了forceRefresh则从服务器拉取

**Parameters**

* `list` 群组id列表，传入空列表函数返回后从此处获取返回的群组id列表
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `fetchGroupsByIdList(`[`ListOfLongLong`](broken-reference) `groupIdList,`[`BMXGroupList`](broken-reference) `list,boolean forceRefresh)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a21ca3641161497e97ea005848746c399" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a21ca3641161497e97ea005848746c399"></a>

获取传入群组id的群组信息列表，如果设置了forceRefresh则从服务器拉取

**Parameters**

* `groupIdList` 群组id列表
* `list` 群组详细信息列表，传入空列表函数返回后从此处获取返回的群组详细信息列表
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `search(`[`ListOfLongLong`](broken-reference) `groupIdList,`[`BMXGroupList`](broken-reference) `list,boolean forceRefresh)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1ad9cf12c41872f8aba892783c522e46ee" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1ad9cf12c41872f8aba892783c522e46ee"></a>

获取传入群组id的群组信息列表，如果设置了forceRefresh则从服务器拉取

**Parameters**

* `groupIdList` 群组id列表
* `list` 群组详细信息列表，传入空列表函数返回后从此处获取返回的群组详细信息列表
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `fetchGroupById(long groupId,`[`BMXGroup`](broken-reference) `group,boolean forceRefresh)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a6c60a360156268dc3169198dd44d1261" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a6c60a360156268dc3169198dd44d1261"></a>

获取群信息，如果设置了forceRefresh则从服务器拉取

**Parameters**

* `groupId` 要搜索的群组id
* `group` 搜索返回的群组信息，传入指向为空的shared\_ptr对象函数执行后从此获取返回结果
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `search(long groupId,`[`BMXGroup`](broken-reference) `group,boolean forceUpdate)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a553a85042a23734a69e7d9f09eb35f5c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a553a85042a23734a69e7d9f09eb35f5c"></a>

获取群信息，如果设置了forceRefresh则从服务器拉取

**Parameters**

* `groupId` 要搜索的群组id
* `group` 搜索返回的群组信息，传入指向为空的shared\_ptr对象函数执行后从此获取返回结果
* `forceUpdate` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `fetchLocalGroupsByName(`[`BMXGroupList`](broken-reference) `list,String name)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a3406796bc2ea38bf39a3c8c107a1f61f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a3406796bc2ea38bf39a3c8c107a1f61f"></a>

通过群名称查询本地群信息，从本地数据库中通过群名称查询获取群组

**Parameters**

* `list` 搜索结果返回的群列表信息
* `name` 查询的群名称关键字

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `search(`[`BMXGroupList`](broken-reference) `list,String name)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a97785ae0ec471d7cabe56e605e098e7f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a97785ae0ec471d7cabe56e605e098e7f"></a>

通过群名称查询本地群信息，从本地数据库中通过群名称查询获取群组

**Parameters**

* `list` 搜索结果返回的群列表信息
* `name` 查询的群名称关键字

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `create(BMXGroupService.CreateGroupOptions options,`[`BMXGroup`](broken-reference) `group)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a39c3a044094073d6df6e34a9e326830f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a39c3a044094073d6df6e34a9e326830f"></a>

创建群

**Parameters**

* `options` 创建群组时传入的参数选项
* `group` 创建好的群，传入指向为空的shared\_ptr对象函数执行后从此获取返回结果

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `destroy(`[`BMXGroup`](broken-reference) `group)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1aa23cdc36052c77657e7a9e48567c9680" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1aa23cdc36052c77657e7a9e48567c9680"></a>

销毁群

**Parameters**

* `group` 要销毁的群组

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `join(`[`BMXGroup`](broken-reference) `group,String message)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a7b37d9a43269a6470f46606973b4f0d8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a7b37d9a43269a6470f46606973b4f0d8"></a>

加入一个群，根据群设置可能需要管理员批准

**Parameters**

* `group` 要加入的群组
* `message` 申请入群的信息

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `leave(`[`BMXGroup`](broken-reference) `group)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a9f18d4e2952a9b2cdff9dd87293bf3ea" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a9f18d4e2952a9b2cdff9dd87293bf3ea"></a>

退出群

**Parameters**

* `group` 要退出的群组

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getInfo(`[`BMXGroup`](broken-reference) `group)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a84601aaf196448da8a6752756728982d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a84601aaf196448da8a6752756728982d"></a>

获取群详情，从服务端拉取最新信息

**Parameters**

* `group` 要获取群组最新信息的群组

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getMembersNickname(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members,`[`BMXGroupMemberList`](broken-reference) `list)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a3ade79556c4ada4dd3d3b9e334b3ccf2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a3ade79556c4ada4dd3d3b9e334b3ccf2"></a>

获取群组成员详细信息

**Parameters**

* `group` 进行操作的群组
* `members` 要获取群组成员信息详情的群成员id
* `list` 返回的群成员详细，传入空列表在函数操作后从此处获取群成员详细信息列表

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getInvitationList(`[`GroupInvitaionPage`](broken-reference) `result,String cursor,int pageSize)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1ae6b6554353a3dcf51b78713ff65a4ddf" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1ae6b6554353a3dcf51b78713ff65a4ddf"></a>

分页获取群组邀请列表

**Parameters**

* `result` 分页获取的群组邀请列表，传入指向为空的shared\_ptr对象函数执行后从此处获取结果
* `cursor` 分页获取的起始cursor，第一次传入为空，后续传入上次操作返回的result中的cursor
* `pageSize` 分页大小

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getApplicationList(`[`BMXGroupList`](broken-reference) `list,`[`GroupApplicationPage`](broken-reference) `result,String cursor,int pageSize)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a4ea3e5408b4eb685136f1f924c158ce1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a4ea3e5408b4eb685136f1f924c158ce1"></a>

分页获取群组申请列表

**Parameters**

* `list` 需要获取群组申请列表信息的群组id列表
* `result` 分页获取的群组申请列表，传入指向为空的shared\_ptr对象函数执行后从此处获取结果
* `cursor` 分页获取的起始cursor，第一次传入为空，后续传入上次操作返回的result中的cursor
* `pageSize` 分页大小

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getMembers(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupMemberResultPage`](broken-reference) `result,String cursor,int pageSize)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1aa83a50bab7809d89e79f9d68b118d645" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1aa83a50bab7809d89e79f9d68b118d645"></a>

分页获取群成员列表，如果设置了forceRefresh则从服务器拉取，单页最大数量为500.

**Parameters**

* `group` 进行操作的群组
* `result` 分页获取的群成员列表，传入指向为空的shared\_ptr对象函数执行后从此处获取结果
* `cursor` 分页获取的起始cursor，第一次传入为空，后续传入上次操作返回的result中的cursor
* `pageSize` 分页大小

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getMembers(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupMemberList`](broken-reference) `list,boolean forceRefresh)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a22d07de8ada85f5fa8da1d9e09eb740b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a22d07de8ada85f5fa8da1d9e09eb740b"></a>

获取群成员列表，如果设置了forceRefresh则从服务器拉取，最多拉取1000人

**Parameters**

* `group` 进行操作的群组
* `list` 群成员列表，传入空列表函数返回后从此处获取返回的群组详细信息列表
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `addMembers(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members,String message)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1aad188cde782f4809edb7ebce5b6dfaf8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1aad188cde782f4809edb7ebce5b6dfaf8"></a>

添加群成员

**Parameters**

* `group` 进行操作的群组
* `members` 要添加进群的成员id列表
* `message` 添加成员原因信息

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `removeMembers(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members,String reason)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a4dcf1c1c781c9c11cc088fd558f12df2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a4dcf1c1c781c9c11cc088fd558f12df2"></a>

删除群成员

**Parameters**

* `group` 进行操作的群组
* `members` 要删除的群组成员id列表
* `reason` 删除的原因

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `addAdmins(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `admins,String message)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1ab4b7010cc203e9ae0e20fc0092f2ca4a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1ab4b7010cc203e9ae0e20fc0092f2ca4a"></a>

添加管理员

**Parameters**

* `group` 进行操作的群组
* `admins` 要添加为管理员的成员id列表
* `message` 添加为管理员的原因

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `removeAdmins(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `admins,String reason)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1ab121bacf7ade353369eba7d9e1ff0dd4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1ab121bacf7ade353369eba7d9e1ff0dd4"></a>

删除管理员

**Parameters**

* `group` 进行操作的群组
* `admins` 要从管理员移除的成员id列表
* `reason` 要移除管理员的原因

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getAdmins(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupMemberList`](broken-reference) `list,boolean forceRefresh)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a5a0664b3a9523e110c7a8b233d13ee30" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a5a0664b3a9523e110c7a8b233d13ee30"></a>

获取Admins列表，如果设置了forceRefresh则从服务器拉取

**Parameters**

* `group` 进行操作的群组
* `list` 群管理员列表，传入空列表函数返回后从此处获取返回的群组详细信息列表
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `blockMembers(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1abb0843d81a16d2b2259274a2390ee815" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1abb0843d81a16d2b2259274a2390ee815"></a>

添加黑名单

**Parameters**

* `group` 进行操作的群组
* `members` 要加入黑名单的群成员id列表

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `unblockMembers(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a69602eead36ae92f40a70be13661eb87" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a69602eead36ae92f40a70be13661eb87"></a>

从黑名单删除

**Parameters**

* `group` 进行操作的群组
* `members` 从黑名单移除的用户id列表

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getBlockList(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupMemberResultPage`](broken-reference) `result,String cursor,int pageSize)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1ad3924d6718ed481d8f32516564a68f74" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1ad3924d6718ed481d8f32516564a68f74"></a>

分页获取黑名单

**Parameters**

* `group` 进行操作的群组
* `result` 分页获取的黑名单列表，传入指向为空的shared\_ptr对象函数执行后从此处获取结果
* `cursor` 分页获取的起始cursor，第一次传入为空，后续传入上次操作返回的result中的cursor
* `pageSize` 分页大小

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getBlockList(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupMemberList`](broken-reference) `list,boolean forceRefresh)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1acfb8adef27f4763c0361f23f4fbcb1ab" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1acfb8adef27f4763c0361f23f4fbcb1ab"></a>

获取黑名单

**Parameters**

* `group` 进行操作的群组
* `list` 群黑名单列表，传入空列表函数返回后从此处获取返回的群组详细信息列表
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `banMembers(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members,long duration,String reason)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a68e66ab9d98e5d6523aa72147b068439" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a68e66ab9d98e5d6523aa72147b068439"></a>

禁言

**Parameters**

* `group` 进行操作的群组
* `members` 被禁言的群成员id列表
* `duration` 禁言时长
* `reason` 禁言原因

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `banMembers(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members,long duration)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1af3407346be730112479b672ec9878195" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1af3407346be730112479b672ec9878195"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `banGroup(`[`BMXGroup`](broken-reference) `group,long duration)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a620418f4715fa9116508387eb75266a1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a620418f4715fa9116508387eb75266a1"></a>

全员禁言，当前服务器时间加上禁言时长后计算出全员禁言到期时间（只有管理和群主可以发言）

**Parameters**

* `group` 进行操作的群组
* `duration` 禁言时长(分钟)

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `unbanMembers(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a787f3b84810076323127c15ac5521944" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a787f3b84810076323127c15ac5521944"></a>

解除禁言

**Parameters**

* `group` 进行操作的群组
* `members` 被解除禁言的群成员id列表

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `unbanGroup(`[`BMXGroup`](broken-reference) `group)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1aa6877b8d7daea9da23989c9a80a2084f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1aa6877b8d7daea9da23989c9a80a2084f"></a>

全员解除禁言

**Parameters**

* `group` 进行操作的群组

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getBannedMembers(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupBannedMemberResultPage`](broken-reference) `result,String cursor,int pageSize)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a4a81e7b4d11d79a40cf2c461d3d058c7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a4a81e7b4d11d79a40cf2c461d3d058c7"></a>

分页获取禁言列表

**Parameters**

* `group` 进行操作的群组
* `result` 分页获取的禁言列表，传入指向为空的shared\_ptr对象函数执行后从此处获取结果
* `cursor` 分页获取的起始cursor，第一次传入为空，后续传入上次操作返回的result中的cursor
* `pageSize` 分页大小

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getBannedMembers(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupBannedMemberList`](broken-reference) `list)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a32711d93fb764adf9e17e938f942811a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a32711d93fb764adf9e17e938f942811a"></a>

获取禁言列表

**Parameters**

* `group` 进行操作的群组
* `list` 群禁言列表，传入空列表函数返回后从此处获取返回的群组详细信息列表

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `muteMessage(`[`BMXGroup`](broken-reference) `group,BMXGroup.MsgMuteMode mode)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a9bbca5bfeea76c3247acc634ec1f1d7b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a9bbca5bfeea76c3247acc634ec1f1d7b"></a>

设置是否屏蔽群消息

**Parameters**

* `group` 进行操作的群组
* `mode` 群屏蔽的模式

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `acceptApplication(`[`BMXGroup`](broken-reference) `group,long applicantId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a446fa9a991700f981f129f034228fef5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a446fa9a991700f981f129f034228fef5"></a>

接受入群申请

**Parameters**

* `group` 进行操作的群组
* `applicantId` 申请进群的用户id

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `declineApplication(`[`BMXGroup`](broken-reference) `group,long applicantId,String reason)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1af95f95a8c5314627f0c9a7df0a79a416" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1af95f95a8c5314627f0c9a7df0a79a416"></a>

拒绝入群申请

**Parameters**

* `group` 进行操作的群组
* `applicantId` 申请进群的用户id
* `reason` 拒绝的原因

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `declineApplication(`[`BMXGroup`](broken-reference) `group,long applicantId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a34ba7f86fd0af05c4950f424e3a1a886" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a34ba7f86fd0af05c4950f424e3a1a886"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `acceptInvitation(`[`BMXGroup`](broken-reference) `group,long inviter)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a109a390f8606f7c7a3c2947165c4e7c1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a109a390f8606f7c7a3c2947165c4e7c1"></a>

接受入群邀请

**Parameters**

* `group` 进行操作的群组
* `inviter` 邀请者id

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `declineInvitation(`[`BMXGroup`](broken-reference) `group,long inviter,String reason)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a263b2c760f42a9375bc4264f99ecf85f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a263b2c760f42a9375bc4264f99ecf85f"></a>

拒绝入群邀请

**Parameters**

* `group` 进行操作的群组
* `inviter` 邀请者id
* `reason` 拒绝的原因

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `declineInvitation(`[`BMXGroup`](broken-reference) `group,long inviter)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a8357cb424f4d84e8bb0d44922a14ce44" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a8357cb424f4d84e8bb0d44922a14ce44"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `transferOwner(`[`BMXGroup`](broken-reference) `group,long newOwnerId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a1dae34be365c89a447bb5a690c2c2a57" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a1dae34be365c89a447bb5a690c2c2a57"></a>

转移群主

**Parameters**

* `group` 进行操作的群组
* `newOwnerId` 转让为新群主的用户id

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `uploadSharedFile(`[`BMXGroup`](broken-reference) `group,String filePath,String displayName,String extensionName,`[`FileProgressListener`](broken-reference) `arg4)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a321b9b7b0e5d840d03780ccececd56ca" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a321b9b7b0e5d840d03780ccececd56ca"></a>

添加群共享文件

**Parameters**

* `group` 进行操作的群组
* `filePath` 文件的本地路径
* `displayName` 文件的展示名
* `extensionName` 文件的扩展名
* `arg4` 上传回调函数

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `cancelUploadSharedFile(`[`BMXGroup`](broken-reference) `group,String filePath)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1ac671d6c48114b35704130d276a93fad2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1ac671d6c48114b35704130d276a93fad2"></a>

取消上传群共享文件

**Parameters**

* `group` 进行操作的群组
* `filePath` 文件的本地路径

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `removeSharedFile(`[`BMXGroup`](broken-reference) `group,BMXGroup.SharedFile sharedFile)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a664dbde940654b74bfd7e9d3d55cd9cc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a664dbde940654b74bfd7e9d3d55cd9cc"></a>

移除群共享文件

**Parameters**

* `group` 进行操作的群组
* `sharedFile` 删除的群共享文件

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `downloadSharedFile(`[`BMXGroup`](broken-reference) `group,BMXGroup.SharedFile sharedFile,`[`FileProgressListener`](broken-reference) `arg2)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1af6e9cc474778bb911c3372a24aaee240" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1af6e9cc474778bb911c3372a24aaee240"></a>

下载群共享文件

**Parameters**

* `group` 进行操作的群组
* `sharedFile` 下载的群共享文件
* `arg2` 下载回调函数

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `cancelDownloadSharedFile(`[`BMXGroup`](broken-reference) `group,BMXGroup.SharedFile sharedFile)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a147d5130a354d23cb948f06911497dba" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a147d5130a354d23cb948f06911497dba"></a>

取消下载群共享文件

**Parameters**

* `group` 进行操作的群组
* `sharedFile` 下载的群共享文件

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getSharedFilesList(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupSharedFileList`](broken-reference) `list,boolean forceRefresh)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a441dc1b6ece6f13c5ae817601af7ed11" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a441dc1b6ece6f13c5ae817601af7ed11"></a>

获取群共享文件列表

**Parameters**

* `group` 进行操作的群组
* `list` 群共享文件列表，传入空列表函数返回后从此处获取返回的群组详细信息列表
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `changeSharedFileName(`[`BMXGroup`](broken-reference) `group,BMXGroup.SharedFile sharedFile,String name)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a40e720045388e1acfc637de4d43e52b5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a40e720045388e1acfc637de4d43e52b5"></a>

修改群共享文件名称

**Parameters**

* `group` 进行操作的群组
* `sharedFile` 进行更改的群共享文件
* `name` 修改的群共享文件名称

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getLatestAnnouncement(`[`BMXGroup`](broken-reference) `group,BMXGroup.Announcement announcement,boolean forceRefresh)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1afc9a8e33c1bb29bc5261763d8a4d757c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1afc9a8e33c1bb29bc5261763d8a4d757c"></a>

获取最新的群公告

**Parameters**

* `group` 进行操作的群组
* `announcement` 最新的群组公告，传入指向为空的shared\_ptr对象函数返回后从此处获取最新的群组公告
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getAnnouncementList(`[`BMXGroup`](broken-reference) `group,`[`BMXGroupAnnouncementList`](broken-reference) `list,boolean forceRefresh)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a2401970634bdd0d4fd1bca40371bff70" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a2401970634bdd0d4fd1bca40371bff70"></a>

获取群公告列表

**Parameters**

* `group` 进行操作的群组
* `list` 群公告列表，传入空列表函数返回后从此处获取返回的群组详细信息列表
* `forceRefresh` 设置为true强制从服务器获取，本地获取失败的情况sdk会自动从服务器获取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `editAnnouncement(`[`BMXGroup`](broken-reference) `group,String title,String content)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a1a62b6d8f6ab47b3fca6037b54eb6753" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a1a62b6d8f6ab47b3fca6037b54eb6753"></a>

设置群公告

**Parameters**

* `group` 进行操作的群组
* `title` 群公告的标题
* `content` 群公告的内容

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `deleteAnnouncement(`[`BMXGroup`](broken-reference) `group,long announcementId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a9c3ad37b0ac428848a8931ad63c2bcc9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a9c3ad37b0ac428848a8931ad63c2bcc9"></a>

删除群公告

**Parameters**

* `group` 进行操作的群组
* `announcementId` 删除的群公告id

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setName(`[`BMXGroup`](broken-reference) `group,String name)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1aeebd97a463e451a3efd36c89245d9deb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1aeebd97a463e451a3efd36c89245d9deb"></a>

设置群名称

**Parameters**

* `group` 进行操作的群组
* `name` 群组名称

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setDescription(`[`BMXGroup`](broken-reference) `group,String description)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1adc02110dfd716c4bbc63b543de67a20c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1adc02110dfd716c4bbc63b543de67a20c"></a>

设置群描述信息

**Parameters**

* `group` 进行操作的群组
* `description` 群组描述

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setExtension(`[`BMXGroup`](broken-reference) `group,String extension)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a4235d59688fe5b8df56acb5f26cbb4a0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a4235d59688fe5b8df56acb5f26cbb4a0"></a>

设置群扩展信息

**Parameters**

* `group` 进行操作的群组
* `extension` 群组的扩展信息

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setMyNickname(`[`BMXGroup`](broken-reference) `group,String nickname)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1aef5833aa590931839111765450ec8030" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1aef5833aa590931839111765450ec8030"></a>

设置在群里的昵称

**Parameters**

* `group` 进行操作的群组
* `nickname` 用户在群组内的昵称

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setMsgPushMode(`[`BMXGroup`](broken-reference) `group,BMXGroup.MsgPushMode mode)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1afd2a03f057187b9151c10ea9e4c5c500" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1afd2a03f057187b9151c10ea9e4c5c500"></a>

设置群消息通知模式

**Parameters**

* `group` 进行操作的群组
* `mode` 群消息通知模式

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setJoinAuthMode(`[`BMXGroup`](broken-reference) `group,BMXGroup.JoinAuthMode mode)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a0fcba8e8c25e3f222e4c7ca2ac623c9e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a0fcba8e8c25e3f222e4c7ca2ac623c9e"></a>

设置入群审批模式

**Parameters**

* `group` 进行操作的群组
* `mode` 入群审批模式

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setInviteMode(`[`BMXGroup`](broken-reference) `group,BMXGroup.InviteMode mode)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a28c718605cdfc30e880c08c1b8495d7a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a28c718605cdfc30e880c08c1b8495d7a"></a>

设置邀请模式

**Parameters**

* `group` 进行操作的群组
* `mode` 群组的邀请模式

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setAllowMemberModify(`[`BMXGroup`](broken-reference) `group,boolean enable)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1af28f0a5efe6fbe060a9815449ab172c5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1af28f0a5efe6fbe060a9815449ab172c5"></a>

设置是否允许群成员设置群信息

**Parameters**

* `group` 进行操作的群组
* `enable` 是否允许操作

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setEnableReadAck(`[`BMXGroup`](broken-reference) `group,boolean enable)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a4b78838c49c01da72f9fe4c665a5b764" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a4b78838c49c01da72f9fe4c665a5b764"></a>

设置是否开启群消息已读功能

**Parameters**

* `group` 进行操作的群组
* `enable` 是否开启

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setHistoryVisible(`[`BMXGroup`](broken-reference) `group,boolean enable)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1ae769a351860be7b1577409d7f67cdd77" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1ae769a351860be7b1577409d7f67cdd77"></a>

设置群成员是否开可见群历史聊天记录

**Parameters**

* `group` 进行操作的群组
* `enable` 是否开启

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setAvatar(`[`BMXGroup`](broken-reference) `group,String avatarPath,`[`FileProgressListener`](broken-reference) `arg2)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a53263c4f143bd7a2f29f05ee46cf0e21" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a53263c4f143bd7a2f29f05ee46cf0e21"></a>

设置群头像

**Parameters**

* `group` 进行操作的群组
* `avatarPath` 群头像文件的本地路径
* `arg2` 上传回调函数

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `downloadAvatar(`[`BMXGroup`](broken-reference) `group,boolean thumbnail,`[`FileProgressListener`](broken-reference) `arg2)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a8419cbfa99c92aed7e4aedc313b594be" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a8419cbfa99c92aed7e4aedc313b594be"></a>

下载群头像

**Parameters**

* `group` 进行操作的群组
* `thumbnail` 设置为true下载缩略图，false下载原图
* `arg2` 下载回调函数

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline void addGroupListener(`[`BMXGroupServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a05d2faed125872d19a4d381f593da9b3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a05d2faed125872d19a4d381f593da9b3"></a>

添加群组变化监听者

**Parameters**

* `listener` 群组变化监听者

#### `public inline void removeGroupListener(`[`BMXGroupServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a71391bc53795891915e168dd2e5d3adf" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a71391bc53795891915e168dd2e5d3adf"></a>

移除群组变化监听者

**Parameters**

* `listener` 群组变化监听者

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1ab8d90d61353a1642680867956febb673" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1ab8d90d61353a1642680867956febb673"></a>

#### `protected inline BMXGroupService(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a0ed4287802bdf94b14e62168e7e97f41" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a0ed4287802bdf94b14e62168e7e97f41"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a67b4eccc54f4f11c755437077528bb50" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1a67b4eccc54f4f11c755437077528bb50"></a>

## class `CreateGroupOptions` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options"></a>

创建群组选项

### Summary

| Members                                                                                                | Descriptions |
| ------------------------------------------------------------------------------------------------------ | ------------ |
| `public inline synchronized void delete()`                                                             |              |
| `public inline CreateGroupOptions()`                                                                   |              |
| `public inline CreateGroupOptions(String name,String description,boolean isPublic,boolean isChatroom)` |              |
| `public inline CreateGroupOptions(String name,String description,boolean isPublic)`                    |              |
| `public inline CreateGroupOptions(String name,String description)`                                     |              |
| `public inline void setMName(String value)`                                                            |              |
| `public inline String getMName()`                                                                      |              |
| `public inline void setMDescription(String value)`                                                     |              |
| `public inline String getMDescription()`                                                               |              |
| `public inline void setMIsPublic(boolean value)`                                                       |              |
| `public inline boolean getMIsPublic()`                                                                 |              |
| `public inline void setMIsChatroom(boolean value)`                                                     |              |
| `public inline boolean getMIsChatroom()`                                                               |              |
| `public inline void setMMessage(String value)`                                                         |              |
| `public inline String getMMessage()`                                                                   |              |
| `public inline void setMMembers(`[`ListOfLongLong`](broken-reference) `value)`                         |              |
| `public inline` [`ListOfLongLong`](broken-reference) `getMMembers()`                                   |              |
| `protected transient boolean swigCMemOwn`                                                              |              |
| `protected inline CreateGroupOptions(long cPtr,boolean cMemoryOwn)`                                    |              |
| `protected inline void finalize()`                                                                     |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1ac01bb8c793d78ee86a8851" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1ac01bb8c793d78ee86a8851"></a>

#### `public inline CreateGroupOptions()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1ae0c630b79146709ca202f0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1ae0c630b79146709ca202f0"></a>

#### `public inline CreateGroupOptions(String name,String description,boolean isPublic,boolean isChatroom)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1abac977455937f4ebec4fcc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1abac977455937f4ebec4fcc"></a>

#### `public inline CreateGroupOptions(String name,String description,boolean isPublic)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1ac578f4496c5f5a16c9e676" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1ac578f4496c5f5a16c9e676"></a>

#### `public inline CreateGroupOptions(String name,String description)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a8bc1bd5299b433b4e9165c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a8bc1bd5299b433b4e9165c"></a>

#### `public inline void setMName(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a3659b67cb68b7697c6f1f1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a3659b67cb68b7697c6f1f1"></a>

#### `public inline String getMName()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a33a1f82e27043abcfc5b4c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a33a1f82e27043abcfc5b4c"></a>

#### `public inline void setMDescription(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a42336bb251190ef218197e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a42336bb251190ef218197e"></a>

#### `public inline String getMDescription()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a9edbeea71cc942248625f8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a9edbeea71cc942248625f8"></a>

#### `public inline void setMIsPublic(boolean value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a876703928e8bcf67aa0f5e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a876703928e8bcf67aa0f5e"></a>

#### `public inline boolean getMIsPublic()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a977c2aacf0a53bf4f736e9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a977c2aacf0a53bf4f736e9"></a>

#### `public inline void setMIsChatroom(boolean value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a82cded1461bf5a50d56047" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a82cded1461bf5a50d56047"></a>

#### `public inline boolean getMIsChatroom()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a95ae4f4361c3278d697d10" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a95ae4f4361c3278d697d10"></a>

#### `public inline void setMMessage(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1ae5d23a9aface2ade443bf6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1ae5d23a9aface2ade443bf6"></a>

#### `public inline String getMMessage()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a2ef61c8b2bc441a9aab456" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a2ef61c8b2bc441a9aab456"></a>

#### `public inline void setMMembers(`[`ListOfLongLong`](broken-reference) `value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a59382cdf00f9029a7e4f87" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a59382cdf00f9029a7e4f87"></a>

#### `public inline` [`ListOfLongLong`](broken-reference) `getMMembers()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a5f8fbb8e4acd5df994db4a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a5f8fbb8e4acd5df994db4a"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a667f1971c4e7c9c66a1ab9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1a667f1971c4e7c9c66a1ab9"></a>

#### `protected inline CreateGroupOptions(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1abbe95cdaf397a633f81aba" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1abbe95cdaf397a633f81aba"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1ab7037943ef04b4d67b741b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_1_1_create_group_options_1ab7037943ef04b4d67b741b"></a>

## class `BMXGroupServiceListener` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener"></a>

群组变化监听者

### Summary

| Members                                                                                                                                   | Descriptions                                       |
| ----------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------- |
| `public inline synchronized void delete()`                                                                                                |                                                    |
| `public inline void swigReleaseOwnership()`                                                                                               |                                                    |
| `public inline void swigTakeOwnership()`                                                                                                  |                                                    |
| `public inline void onGroupCreate(`[`BMXGroup`](broken-reference) `group)`                                                                | 多设备同步创建群组                                          |
| `public inline void onGroupListUpdate(`[`BMXGroupList`](broken-reference) `list)`                                                         | 群列表更新了                                             |
| `public inline void onGroupJoined(`[`BMXGroup`](broken-reference) `group)`                                                                | 加入了某群                                              |
| `public inline void onGroupLeft(`[`BMXGroup`](broken-reference) `group,String reason)`                                                    | 退出了某群                                              |
| `public inline void onInvitated(long groupId,long inviter,String message)`                                                                | 收到入群邀请                                             |
| `public inline void onInvitationAccepted(`[`BMXGroup`](broken-reference) `group,long inviteeId)`                                          | 入群邀请被接受                                            |
| `public inline void onInvitationDeclined(`[`BMXGroup`](broken-reference) `group,long inviteeId,String reason)`                            | 入群申请被拒绝                                            |
| `public inline void onApplied(`[`BMXGroup`](broken-reference) `group,long applicantId,String message)`                                    | 收到入群申请                                             |
| `public inline void onApplicationAccepted(`[`BMXGroup`](broken-reference) `group,long approver)`                                          | 入群申请被接受                                            |
| `public inline void onApplicationDeclined(`[`BMXGroup`](broken-reference) `group,long approver,String reason)`                            | 入群申请被拒绝                                            |
| `public inline void onMembersBanned(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members,long duration)` | 群成员被禁言                                             |
| `public inline void onMembersUnbanned(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members)`             | 群成员被解除禁言                                           |
| `public inline void onMemberJoined(`[`BMXGroup`](broken-reference) `group,long memberId,long inviter)`                                    | 加入新成员                                              |
| `public inline void onMemberLeft(`[`BMXGroup`](broken-reference) `group,long memberId,String reason)`                                     | 群成员退出                                              |
| `public inline void onAdminsAdded(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members)`                 | 添加了新管理员                                            |
| `public inline void onAdminsRemoved(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members,String reason)` | 移除了管理员                                             |
| `public inline void onOwnerAssigned(`[`BMXGroup`](broken-reference) `group)`                                                              | 成为群主                                               |
| `public inline void onGroupInfoUpdate(`[`BMXGroup`](broken-reference) `group,BMXGroup.UpdateInfoType type)`                               | 群组信息变更                                             |
| `public inline void onMemberChangeNickName(`[`BMXGroup`](broken-reference) `group,long memberId,String nickName)`                         | 群成员更改群内昵称                                          |
| `public inline void onAnnouncementUpdate(`[`BMXGroup`](broken-reference) `group,BMXGroup.Announcement announcement)`                      | 收到群公告                                              |
| `public inline void onSharedFileUploaded(`[`BMXGroup`](broken-reference) `group,BMXGroup.SharedFile sharedFile)`                          | 收到共享文件                                             |
| `public inline void onSharedFileDeleted(`[`BMXGroup`](broken-reference) `group,BMXGroup.SharedFile sharedFile)`                           | 删除了共享文件                                            |
| `public inline void onSharedFileUpdated(`[`BMXGroup`](broken-reference) `group,BMXGroup.SharedFile sharedFile)`                           | 共享文件更新文件名                                          |
| `public inline void onBlockListAdded(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members)`              | 添加黑名单                                              |
| `public inline void onBlockListRemoved(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members)`            | 删除黑名单                                              |
| `public inline void onGroupListUpdate()`                                                                                                  | 客户端从服务器拉取到新群组时触发，用于用户群组列表更新，从SDK调用本地获取群组即可取得全部成员信息 |
| `public inline BMXGroupServiceListener()`                                                                                                 |                                                    |
| `public inline void registerGroupService(`[`BMXGroupService`](broken-reference) `service)`                                                |                                                    |
| `protected transient boolean swigCMemOwn`                                                                                                 |                                                    |
| `protected inline BMXGroupServiceListener(long cPtr,boolean cMemoryOwn)`                                                                  |                                                    |
| `protected inline void finalize()`                                                                                                        |                                                    |
| `protected inline void swigDirectorDisconnect()`                                                                                          |                                                    |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a350e32b0a928e100966e98974314b422" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a350e32b0a928e100966e98974314b422"></a>

#### `public inline void swigReleaseOwnership()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1ac9aa20437a5d84edc5f81c8173a9cc5a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1ac9aa20437a5d84edc5f81c8173a9cc5a"></a>

#### `public inline void swigTakeOwnership()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1aa1cce106de84be67b498d8481fe8aee5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1aa1cce106de84be67b498d8481fe8aee5"></a>

#### `public inline void onGroupCreate(`[`BMXGroup`](broken-reference) `group)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a04f2514f3050b914090681fc9d4fc460" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a04f2514f3050b914090681fc9d4fc460"></a>

多设备同步创建群组

**Parameters**

* `group` 新创建的群组

#### `public inline void onGroupListUpdate(`[`BMXGroupList`](broken-reference) `list)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a2802fa1771952bd77b398aa4e86a6d1d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a2802fa1771952bd77b398aa4e86a6d1d"></a>

群列表更新了

**Parameters**

* `list` 更新的群组列表

#### `public inline void onGroupJoined(`[`BMXGroup`](broken-reference) `group)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1ab0948cded84e53b07a2c14d4e976443a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1ab0948cded84e53b07a2c14d4e976443a"></a>

加入了某群

**Parameters**

* `group` 加入的群组

#### `public inline void onGroupLeft(`[`BMXGroup`](broken-reference) `group,String reason)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a64c997bf0b0e778a682dac34d5ea73b0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a64c997bf0b0e778a682dac34d5ea73b0"></a>

退出了某群

**Parameters**

* `group` 退出的群组
* `reason` 退出原因

#### `public inline void onInvitated(long groupId,long inviter,String message)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a94245e458821f8ba12d1122db0cf6003" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a94245e458821f8ba12d1122db0cf6003"></a>

收到入群邀请

**Parameters**

* `groupId` 邀请进入的群组id
* `inviter` 邀请者id
* `message` 邀请原因

#### `public inline void onInvitationAccepted(`[`BMXGroup`](broken-reference) `group,long inviteeId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1ad9f9f328cb8fdfabb2d60028f9f652e4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1ad9f9f328cb8fdfabb2d60028f9f652e4"></a>

入群邀请被接受

**Parameters**

* `group` 邀请被同意的群组
* `inviteeId` 被邀请者id

#### `public inline void onInvitationDeclined(`[`BMXGroup`](broken-reference) `group,long inviteeId,String reason)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a216fea716c9362de69c0ad6a58b68bd4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a216fea716c9362de69c0ad6a58b68bd4"></a>

入群申请被拒绝

**Parameters**

* `group` 邀请被拒绝的群组
* `inviteeId` 被邀请者id
* `reason` 拒绝原因

#### `public inline void onApplied(`[`BMXGroup`](broken-reference) `group,long applicantId,String message)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a797dca6f341522fe4b8def93fed182b9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a797dca6f341522fe4b8def93fed182b9"></a>

收到入群申请

**Parameters**

* `group` 收到入群申请的群组
* `applicantId` 申请者id
* `message` 申请原因

#### `public inline void onApplicationAccepted(`[`BMXGroup`](broken-reference) `group,long approver)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1adb73eda53676c6800f05f40c9e72208f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1adb73eda53676c6800f05f40c9e72208f"></a>

入群申请被接受

**Parameters**

* `group` 入群申请被接受的群组
* `approver` 申请的批准者

#### `public inline void onApplicationDeclined(`[`BMXGroup`](broken-reference) `group,long approver,String reason)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1ad4493d985277b1d1d3850b632034f26e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1ad4493d985277b1d1d3850b632034f26e"></a>

入群申请被拒绝

**Parameters**

* `group` 入群申请被拒绝的群组
* `approver` 申请的批准者
* `reason` 拒绝的原因

#### `public inline void onMembersBanned(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members,long duration)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a43a2fc60ab9f8bf6ad55f031bf935b6e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a43a2fc60ab9f8bf6ad55f031bf935b6e"></a>

群成员被禁言

**Parameters**

* `group` 群成员被禁言的群组
* `members` 被禁言的群成员id列表
* `duration` 禁言时长

#### `public inline void onMembersUnbanned(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1aa2be7d13c723e6f3013889fd0064fb49" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1aa2be7d13c723e6f3013889fd0064fb49"></a>

群成员被解除禁言

**Parameters**

* `group` 群成员被解除禁言的群组
* `members` 被解除禁言的群成员id列表

#### `public inline void onMemberJoined(`[`BMXGroup`](broken-reference) `group,long memberId,long inviter)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1ac24ee5b92090c6470cd3c9c48e59a2cb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1ac24ee5b92090c6470cd3c9c48e59a2cb"></a>

加入新成员

**Parameters**

* `group` 有成员加入的群组
* `memberId` 加入成员的id
* `inviter` 邀请者id

#### `public inline void onMemberLeft(`[`BMXGroup`](broken-reference) `group,long memberId,String reason)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a1035f33fc0c764268644de0e41d4953d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a1035f33fc0c764268644de0e41d4953d"></a>

群成员退出

**Parameters**

* `group` 有成员退出的群组
* `memberId` 退出的群成员id
* `reason` 退出的原因

#### `public inline void onAdminsAdded(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1afb7e28ee708dd655b094f73ab3f1f940" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1afb7e28ee708dd655b094f73ab3f1f940"></a>

添加了新管理员

**Parameters**

* `group` 发生添加新管理员的群组
* `members` 被提升为管理员的成员列表

#### `public inline void onAdminsRemoved(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members,String reason)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a5a95c8ba5d95496328e42195a8cdb176" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a5a95c8ba5d95496328e42195a8cdb176"></a>

移除了管理员

**Parameters**

* `group` 发生移除管理员的群组
* `members` 被移除了管理员的成员列表
* `reason` 被移除的原因

#### `public inline void onOwnerAssigned(`[`BMXGroup`](broken-reference) `group)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a1c91781e261d594e56dcee4ddaa1a778" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a1c91781e261d594e56dcee4ddaa1a778"></a>

成为群主

**Parameters**

* `group` 被转让为群主的群组

#### `public inline void onGroupInfoUpdate(`[`BMXGroup`](broken-reference) `group,BMXGroup.UpdateInfoType type)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1af55c12f36ee5372061ab78861b1e0669" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1af55c12f36ee5372061ab78861b1e0669"></a>

群组信息变更

**Parameters**

* `group` 群信息发生变更的群组
* `type` 发生变更的群信息类型

#### `public inline void onMemberChangeNickName(`[`BMXGroup`](broken-reference) `group,long memberId,String nickName)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a6665c516224e762f57e982153d0c7d5a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a6665c516224e762f57e982153d0c7d5a"></a>

群成员更改群内昵称

**Parameters**

* `group` 发生群成员变更群昵称的群组
* `memberId` 变更群昵称的群成员id
* `nickName` 变更后的群昵称

#### `public inline void onAnnouncementUpdate(`[`BMXGroup`](broken-reference) `group,BMXGroup.Announcement announcement)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1ae05fbf564e0b5aac67abb2289ccd965f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1ae05fbf564e0b5aac67abb2289ccd965f"></a>

收到群公告

**Parameters**

* `group` 发生群公告更新的群组
* `announcement` 变更后的最新的群更高

#### `public inline void onSharedFileUploaded(`[`BMXGroup`](broken-reference) `group,BMXGroup.SharedFile sharedFile)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a9d99bb8ca9b5f0b94dd6ef0288606097" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a9d99bb8ca9b5f0b94dd6ef0288606097"></a>

收到共享文件

**Parameters**

* `group` 发生群共享文件上传的群组
* `sharedFile` 新上传的群共享文件

#### `public inline void onSharedFileDeleted(`[`BMXGroup`](broken-reference) `group,BMXGroup.SharedFile sharedFile)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1aa1d9246f91412b1432f907e3c66a9132" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1aa1d9246f91412b1432f907e3c66a9132"></a>

删除了共享文件

**Parameters**

* `group` 发生群共享文件删除的群组
* `sharedFile` 被删除的群共享文件

#### `public inline void onSharedFileUpdated(`[`BMXGroup`](broken-reference) `group,BMXGroup.SharedFile sharedFile)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a5caeffb2379f0879c48f451b121cec39" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a5caeffb2379f0879c48f451b121cec39"></a>

共享文件更新文件名

**Parameters**

* `group` 发生群共享文件更新的群组
* `sharedFile` 更新的群共享文件

#### `public inline void onBlockListAdded(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a040e2ca9efc18f22f7592732ea8ce86d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a040e2ca9efc18f22f7592732ea8ce86d"></a>

添加黑名单

**Parameters**

* `group` 添加黑名单的群组
* `members` 添加的黑名单成员列表

#### `public inline void onBlockListRemoved(`[`BMXGroup`](broken-reference) `group,`[`ListOfLongLong`](broken-reference) `members)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1ad7d266caaa21c90da58d8b4479604ffb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1ad7d266caaa21c90da58d8b4479604ffb"></a>

删除黑名单

**Parameters**

* `group` 删除黑名单的群组
* `members` 删除的黑名单成员列表

#### `public inline void onGroupListUpdate()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a29d5037956799cc3ebd03b3fa1ab0421" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a29d5037956799cc3ebd03b3fa1ab0421"></a>

客户端从服务器拉取到新群组时触发，用于用户群组列表更新，从SDK调用本地获取群组即可取得全部成员信息

#### `public inline BMXGroupServiceListener()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a288c576a37d0e622f13c30f9e3290109" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a288c576a37d0e622f13c30f9e3290109"></a>

#### `public inline void registerGroupService(`[`BMXGroupService`](broken-reference) `service)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1aef8f93bb51609a2a61e83f5acce64ac1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1aef8f93bb51609a2a61e83f5acce64ac1"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1ab7153bdb3307bc452a4b4caae1b01be2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1ab7153bdb3307bc452a4b4caae1b01be2"></a>

#### `protected inline BMXGroupServiceListener(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a69abc1031de9e43770c4997fc85e1d86" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a69abc1031de9e43770c4997fc85e1d86"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a116ef63bb736b2a9d3a1e2e71675beef" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a116ef63bb736b2a9d3a1e2e71675beef"></a>

#### `protected inline void swigDirectorDisconnect()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a810d63b5964258f34d80c033993e7d46" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_service_listener_1a810d63b5964258f34d80c033993e7d46"></a>

## class `BMXGroupSharedFileList` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list"></a>

### Summary

| Members                                                                 | Descriptions |
| ----------------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                              |              |
| `public inline BMXGroupSharedFileList()`                                |              |
| `public inline BMXGroupSharedFileList(long n)`                          |              |
| `public inline long size()`                                             |              |
| `public inline long capacity()`                                         |              |
| `public inline void reserve(long n)`                                    |              |
| `public inline boolean isEmpty()`                                       |              |
| `public inline void clear()`                                            |              |
| `public inline void add(BMXGroup.SharedFile x)`                         |              |
| `public inline BMXGroup.SharedFile get(int i)`                          |              |
| `public inline void set(int i,BMXGroup.SharedFile val)`                 |              |
| `protected transient boolean swigCMemOwn`                               |              |
| `protected inline BMXGroupSharedFileList(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                                      |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a1071130599d3845894cb7d9646e44244" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a1071130599d3845894cb7d9646e44244"></a>

#### `public inline BMXGroupSharedFileList()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a0d821365bd5b85f1f2204d9cdaf32044" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a0d821365bd5b85f1f2204d9cdaf32044"></a>

#### `public inline BMXGroupSharedFileList(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a6e71dc9e3bc971cd3b9745c5965c41d9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a6e71dc9e3bc971cd3b9745c5965c41d9"></a>

#### `public inline long size()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a42d1f6b4d745f7d3c1ba83101ccaeb49" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a42d1f6b4d745f7d3c1ba83101ccaeb49"></a>

#### `public inline long capacity()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a5cd5e3565c3a2d3db4356e25418488e3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a5cd5e3565c3a2d3db4356e25418488e3"></a>

#### `public inline void reserve(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a2ad2a174d767548b4ffbecf21318e035" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a2ad2a174d767548b4ffbecf21318e035"></a>

#### `public inline boolean isEmpty()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a32603be91025e87277c21e866a22a978" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a32603be91025e87277c21e866a22a978"></a>

#### `public inline void clear()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a0818eda1a2503c5fad95be14eec61ae9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a0818eda1a2503c5fad95be14eec61ae9"></a>

#### `public inline void add(BMXGroup.SharedFile x)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1ad16966e17c1cfc0a4ce3dac0d408008b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1ad16966e17c1cfc0a4ce3dac0d408008b"></a>

#### `public inline BMXGroup.SharedFile get(int i)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a47c9262d5c0bf2465d5583eb56292bb8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a47c9262d5c0bf2465d5583eb56292bb8"></a>

#### `public inline void set(int i,BMXGroup.SharedFile val)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a9116c99fe489d12fef2236e58814733e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1a9116c99fe489d12fef2236e58814733e"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1abad59f34db92f915b9064998eab25e8f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1abad59f34db92f915b9064998eab25e8f"></a>

#### `protected inline BMXGroupSharedFileList(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1adb5c90d257eb21bac197b0080d797bfc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1adb5c90d257eb21bac197b0080d797bfc"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1ad6ccfc49f18f91ef2ee7284cf6de3e68" id="classim_1_1floo_1_1floolib_1_1_b_m_x_group_shared_file_list_1ad6ccfc49f18f91ef2ee7284cf6de3e68"></a>

## class `BMXHttpClient` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_http_client" id="classim_1_1floo_1_1floolib_1_1_b_m_x_http_client"></a>

### Summary

| Members                                  | Descriptions |
| ---------------------------------------- | ------------ |
| `class` [`MyCallback`](broken-reference) |              |

### Members

#### `class` [`MyCallback`](broken-reference) <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_http_client_1_1_my_callback" id="classim_1_1floo_1_1floolib_1_1_b_m_x_http_client_1_1_my_callback"></a>

## class `MyCallback` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_http_client_1_1_my_callback" id="classim_1_1floo_1_1floolib_1_1_b_m_x_http_client_1_1_my_callback"></a>

```
class MyCallback
  : public Callback
```

### Summary

| Members                                                                                          | Descriptions |
| ------------------------------------------------------------------------------------------------ | ------------ |
| `public inline void deleteFile(FileOutputStream fos,String path)`                                |              |
| `public inline void changePercent(final Object fileLock,final StringBuffer percent,long newVal)` |              |
| `public inline void onFailure(Call call,IOException e)`                                          |              |
| `public inline void onResponse(Call call,Response response)`                                     |              |

### Members

#### `public inline void deleteFile(FileOutputStream fos,String path)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_http_client_1_1_my_callback_1a8b92712c920c1326156c1daf582e02f1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_http_client_1_1_my_callback_1a8b92712c920c1326156c1daf582e02f1"></a>

#### `public inline void changePercent(final Object fileLock,final StringBuffer percent,long newVal)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_http_client_1_1_my_callback_1a65114da284bcea4269b5203a55624ff0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_http_client_1_1_my_callback_1a65114da284bcea4269b5203a55624ff0"></a>

#### `public inline void onFailure(Call call,IOException e)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_http_client_1_1_my_callback_1a63abda44d5cd02b6cd4ccf5b1d2935b5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_http_client_1_1_my_callback_1a63abda44d5cd02b6cd4ccf5b1d2935b5"></a>

#### `public inline void onResponse(Call call,Response response)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_http_client_1_1_my_callback_1a71c135ca9740a4909cd3214ec18ef2eb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_http_client_1_1_my_callback_1a71c135ca9740a4909cd3214ec18ef2eb"></a>

## class `BMXImageAttachment` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment" id="classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment"></a>

```
class BMXImageAttachment
  : public im.floo.floolib.BMXFileAttachment
```

图片消息附件

### Summary

| Members                                                                                                               | Descriptions    |
| --------------------------------------------------------------------------------------------------------------------- | --------------- |
| `public inline synchronized void delete()`                                                                            |                 |
| `public inline BMXImageAttachment(String path,BMXMessageAttachment.Size size,String displayName)`                     | 构造函数，构建发送图片消息附件 |
| `public inline BMXImageAttachment(String path,BMXMessageAttachment.Size size)`                                        |                 |
| `public inline BMXImageAttachment(String ratelUrl,BMXMessageAttachment.Size size,String displayName,long fileLength)` | 构造函数，构建接收图片消息附件 |
| `public inline BMXMessageAttachment.Type type()`                                                                      | 返回图片附件类型        |
| `public inline` [`BMXMessageAttachment`](broken-reference) `clone()`                                                  | 克隆函数            |
| `public inline BMXMessageAttachment.Size size()`                                                                      | 图片大小            |
| `public inline String thumbnailUrl()`                                                                                 |                 |
| `public inline void setThumbnail(String path)`                                                                        | 设置发送图片消息缩略图     |
| `public inline String thumbnailPath()`                                                                                | 缩略图本地路径         |
| `public inline BMXMessageAttachment.DownloadStatus thumbnailDownloadStatus()`                                         | 缩略图下载状态         |
| `protected inline BMXImageAttachment(long cPtr,boolean cMemoryOwn)`                                                   |                 |
| `protected inline void finalize()`                                                                                    |                 |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a978fca8fb34da7f3b3329b3e463e7b0b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a978fca8fb34da7f3b3329b3e463e7b0b"></a>

#### `public inline BMXImageAttachment(String path,BMXMessageAttachment.Size size,String displayName)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a9068d20715296f7b5631ba6f7ffd9ca1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a9068d20715296f7b5631ba6f7ffd9ca1"></a>

构造函数，构建发送图片消息附件

**Parameters**

* `path` 本地路径
* `size` 图片的大小，宽度和高度
* `displayName` 展示名

#### `public inline BMXImageAttachment(String path,BMXMessageAttachment.Size size)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a9d85e14e30727d97392839ac807d9893" id="classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a9d85e14e30727d97392839ac807d9893"></a>

#### `public inline BMXImageAttachment(String ratelUrl,BMXMessageAttachment.Size size,String displayName,long fileLength)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a4df1f40ecdd5259becaa21f70117afcb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a4df1f40ecdd5259becaa21f70117afcb"></a>

构造函数，构建接收图片消息附件

**Parameters**

* `ratelUrl` ratel服务器地址
* `size` 图片的大小，宽度和高度
* `displayName` 展示名
* `fileLength` 文件大小

#### `public inline BMXMessageAttachment.Type type()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a29bdf72f89e00084c4c7d7eb5dd313a6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a29bdf72f89e00084c4c7d7eb5dd313a6"></a>

返回图片附件类型

**Returns**

Type

#### `public inline` [`BMXMessageAttachment`](broken-reference) `clone()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a28e55bfb2a0703d8976b955d2a344be0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a28e55bfb2a0703d8976b955d2a344be0"></a>

克隆函数

**Returns**

BMXMessageAttachmentPtr

#### `public inline BMXMessageAttachment.Size size()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1ab53c15e7cf3fb78284d56324b06b3091" id="classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1ab53c15e7cf3fb78284d56324b06b3091"></a>

图片大小

**Returns**

Size

#### `public inline String thumbnailUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1acba1364a18adb83a655ef287384d05a7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1acba1364a18adb83a655ef287384d05a7"></a>

#### `public inline void setThumbnail(String path)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a82bb350796ce6af67b9a21f4ff27df31" id="classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a82bb350796ce6af67b9a21f4ff27df31"></a>

设置发送图片消息缩略图

**Parameters**

* `path` 本地路径

#### `public inline String thumbnailPath()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1abab9271090104d63c91e00a0f302da11" id="classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1abab9271090104d63c91e00a0f302da11"></a>

缩略图本地路径

**Returns**

std::string

#### `public inline BMXMessageAttachment.DownloadStatus thumbnailDownloadStatus()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a6155606df9d53cc37649cca8978d556c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a6155606df9d53cc37649cca8978d556c"></a>

缩略图下载状态

**Returns**

DownloadStatus

#### `protected inline BMXImageAttachment(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a8da1025d455bb7e968e513fa9d26848f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1a8da1025d455bb7e968e513fa9d26848f"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1ab7e89b9e8787628eae6b08653cd718aa" id="classim_1_1floo_1_1floolib_1_1_b_m_x_image_attachment_1ab7e89b9e8787628eae6b08653cd718aa"></a>

## class `BMXLocationAttachment` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment" id="classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment"></a>

```
class BMXLocationAttachment
  : public im.floo.floolib.BMXMessageAttachment
```

位置消息附件

### Summary

| Members                                                                                | Descriptions |
| -------------------------------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                                             |              |
| `public inline BMXLocationAttachment(double latitude,double longitude,String address)` | 构造函数         |
| `public inline BMXMessageAttachment.Type type()`                                       | 返回位置附件类型     |
| `public inline` [`BMXMessageAttachment`](broken-reference) `clone()`                   | 克隆函数         |
| `public inline double latitude()`                                                      | 纬度           |
| `public inline double longitude()`                                                     | 经度           |
| `public inline String address()`                                                       | 地址           |
| `protected inline BMXLocationAttachment(long cPtr,boolean cMemoryOwn)`                 |              |
| `protected inline void finalize()`                                                     |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1a47c5b692991d0e818ef6949a458e7d55" id="classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1a47c5b692991d0e818ef6949a458e7d55"></a>

#### `public inline BMXLocationAttachment(double latitude,double longitude,String address)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1a95c312489b4db8d6acaa37414ed8d831" id="classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1a95c312489b4db8d6acaa37414ed8d831"></a>

构造函数

**Parameters**

* `latitude` 纬度
* `longitude` 经度
* `address` 地址名称

#### `public inline BMXMessageAttachment.Type type()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1ab21f48c50c213572842cfaea0b1475a9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1ab21f48c50c213572842cfaea0b1475a9"></a>

返回位置附件类型

**Returns**

Type

#### `public inline` [`BMXMessageAttachment`](broken-reference) `clone()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1af8bd71922bfecd2d438a38c9ee4c7494" id="classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1af8bd71922bfecd2d438a38c9ee4c7494"></a>

克隆函数

**Returns**

BMXMessageAttachmentPtr

#### `public inline double latitude()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1a01136d092fe88e2ea4fe6ceb8fc010c6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1a01136d092fe88e2ea4fe6ceb8fc010c6"></a>

纬度

**Returns**

double

#### `public inline double longitude()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1a760339b153a621cfdd05aea6c5e44a0c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1a760339b153a621cfdd05aea6c5e44a0c"></a>

经度

**Returns**

double

#### `public inline String address()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1a0ec1673096e72cb6394d51e2644f5a4d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1a0ec1673096e72cb6394d51e2644f5a4d"></a>

地址

**Returns**

std::string

#### `protected inline BMXLocationAttachment(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1a361c459c460a1bad1476ebcffaade399" id="classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1a361c459c460a1bad1476ebcffaade399"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1a98a6ee3f3cd615a1f3317f3839a1700f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_location_attachment_1a98a6ee3f3cd615a1f3317f3839a1700f"></a>

## class `BMXMessage` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message"></a>

```
class BMXMessage
  : public im.floo.floolib.BMXBaseObject
```

消息

### Summary

| Members                                                                       | Descriptions                                                                                 |
| ----------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `public inline synchronized void delete()`                                    |                                                                                              |
| `public inline long msgId()`                                                  | 消息唯一ID                                                                                       |
| `public inline long clientMsgId()`                                            | 消息客户端ID,仅在消息发送端存在                                                                            |
| `public inline long fromId()`                                                 | 消息发送方ID                                                                                      |
| `public inline long toId()`                                                   | 消息接收方ID                                                                                      |
| `public inline BMXMessage.MessageType type()`                                 | 消息类型                                                                                         |
| `public inline long conversationId()`                                         | 消息所属会话ID                                                                                     |
| `public inline BMXMessage.DeliveryStatus deliveryStatus()`                    | 消息投递状态                                                                                       |
| `public inline void setDeliveryStatus(BMXMessage.DeliveryStatus arg0)`        | 设置消息投递状态                                                                                     |
| `public inline long serverTimestamp()`                                        | 消息时间戳（服务端收到时的时间）                                                                             |
| `public inline void setServerTimestamp(long arg0)`                            | 设置时间戳（服务端收到时的时间）                                                                             |
| `public inline long clientTimestamp()`                                        | 本地时间戳（消息创建或者收到时的本地时间）                                                                        |
| `public inline void setClientTimestamp(long arg0)`                            | 设置消息本地时间戳                                                                                    |
| `public inline boolean isPlayed()`                                            | 语音或者视频消息是否播放过，仅对收到的音视频消息有效                                                                   |
| `public inline void setIsPlayed(boolean arg0)`                                |                                                                                              |
| `public inline boolean isPlayAcked()`                                         | 语音或者视频消息是否收到播放回执，仅对收到的音视频消息有效                                                                |
| `public inline void setIsPlayAcked(boolean arg0)`                             |                                                                                              |
| `public inline boolean isReceiveMsg()`                                        | 是否接收的消息                                                                                      |
| `public inline void setIsReceiveMsg(boolean arg0)`                            |                                                                                              |
| `public inline boolean isRead()`                                              | 消息是否已读标志                                                                                     |
| `public inline void setIsRead(boolean arg0)`                                  |                                                                                              |
| `public inline boolean isReadAcked()`                                         | 对于发送方表示是否收到了已读回执，对于接收方表示是否发送了已读回执                                                            |
| `public inline void setIsReadAcked(boolean arg0)`                             |                                                                                              |
| `public inline boolean isDeliveryAcked()`                                     | 对于发送方表示消息是否已投递到对方，对于接收方表示是否发送了消息已到达回执                                                        |
| `public inline void setIsDeliveryAcked(boolean arg0)`                         |                                                                                              |
| `public inline String content()`                                              | 消息文本内容                                                                                       |
| `public inline void setContent(String content)`                               | 消息文本内容                                                                                       |
| `public inline BMXMessage.ContentType contentType()`                          | 消息内容类型，如果带附件就表示附件类型，不带附件就是文本类型                                                               |
| `public inline` [`BMXMessageAttachment`](broken-reference) `attachment()`     | 消息附件，BMXMessage拥有附件的所有权，负责释放                                                                 |
| `public inline` [`BMXMessageConfig`](broken-reference) `config()`             | 消息的配置信息                                                                                      |
| `public inline void setConfig(`[`BMXMessageConfig`](broken-reference) `arg0)` | 设置消息配置信息                                                                                     |
| `public inline String extension()`                                            | 消息扩展信息                                                                                       |
| `public inline void setExtension(String arg0)`                                | 设置消息扩展信息                                                                                     |
| `public inline BMXMessage.DeliveryQos deliveryQos()`                          | 消息投递QOS                                                                                      |
| `public inline void setDeliveryQos(BMXMessage.DeliveryQos qos)`               | 设置消息投递QOS                                                                                    |
| `public inline String senderName()`                                           | 消息发送者的显示名称                                                                                   |
| `public inline void setSenderName(String senderName)`                         | 设置消息的发送者显示名称                                                                                 |
| `public inline int groupAckCount()`                                           | 群消息已读AckCount数目                                                                              |
| `public inline void setGroupAckCount(int count)`                              | 设置消息已读groupAckCount数目(SDK 内部调用接口，上层不应该调用)                                                    |
| `public inline int groupAckUnreadCount()`                                     | 群消息未读AckCount数目                                                                              |
| `public inline void setGroupAckUnreadCount(int count)`                        | 设置消息未读groupAckCount数目(SDK 内部调用接口，上层不应该调用)                                                    |
| `public inline boolean groupAckReadAll()`                                     | 群消息是否全部已读                                                                                    |
| `public inline int groupPlayAckCount()`                                       | 获取群消息已播放计数                                                                                   |
| `public inline void setGroupPlayAckCount(int count)`                          |                                                                                              |
| `public inline int groupPlayAckUnreadCount()`                                 | 获取群消息已播放回执未读计数                                                                               |
| `public inline void setGroupPlayAckUnreadCount(int count)`                    |                                                                                              |
| `public inline boolean groupPlayAckReadAll()`                                 | 设置所有群消息已播回执为已读                                                                               |
| `public inline void setPriority(int priority)`                                | 设置消息的扩散优先级，默认为0。0表示扩散，数字越小扩散的越多。 取值范围0-10。普通人在聊天室发送的消息级别默认为5，可以丢弃。管理员默认为0不会丢弃。其它值可以根据业务自行设置。 |
| `public inline int priority()`                                                | 消息的扩散优先级                                                                                     |
| `public inline void setPushMessageMode(boolean arg0)`                         | 设置是否推送消息                                                                                     |
| `public inline boolean isPushMessage()`                                       | 是否是推送消息                                                                                      |
| `protected inline BMXMessage(long cPtr,boolean cMemoryOwn)`                   |                                                                                              |
| `protected inline void finalize()`                                            |                                                                                              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a3048994cbe857b8fba00ca4a53bf5f3f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a3048994cbe857b8fba00ca4a53bf5f3f"></a>

#### `public inline long msgId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a8344ac9bde8655c4efd5d9efa96e1ce2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a8344ac9bde8655c4efd5d9efa96e1ce2"></a>

消息唯一ID

**Returns**

int64\_t

#### `public inline long clientMsgId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a0d3a91afabd3851c08e38a91414d286c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a0d3a91afabd3851c08e38a91414d286c"></a>

消息客户端ID,仅在消息发送端存在

**Returns**

int64\_t

#### `public inline long fromId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a799021253cc54fc4d23e26f2c2650b78" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a799021253cc54fc4d23e26f2c2650b78"></a>

消息发送方ID

**Returns**

int64\_t

#### `public inline long toId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ac42887d82f8302c2b2df25f65095e384" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ac42887d82f8302c2b2df25f65095e384"></a>

消息接收方ID

**Returns**

int64\_t

#### `public inline BMXMessage.MessageType type()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a26c8331db361200c766a64d78817bb80" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a26c8331db361200c766a64d78817bb80"></a>

消息类型

**Returns**

[MessageType](broken-reference)

#### `public inline long conversationId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a4aec73a9960982bc07612fbae7891080" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a4aec73a9960982bc07612fbae7891080"></a>

消息所属会话ID

**Returns**

int64\_t

#### `public inline BMXMessage.DeliveryStatus deliveryStatus()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1aa27186e4af8bceaeddb9fcce33c4eaec" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1aa27186e4af8bceaeddb9fcce33c4eaec"></a>

消息投递状态

**Returns**

[DeliveryStatus](broken-reference)

#### `public inline void setDeliveryStatus(BMXMessage.DeliveryStatus arg0)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ac2969088a008d59786622a7e3cecbe99" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ac2969088a008d59786622a7e3cecbe99"></a>

设置消息投递状态

#### `public inline long serverTimestamp()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1aff2ab94b61d2443e177d0cfa8a12d657" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1aff2ab94b61d2443e177d0cfa8a12d657"></a>

消息时间戳（服务端收到时的时间）

**Returns**

int64\_t

#### `public inline void setServerTimestamp(long arg0)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a2012abfa6a48dfd53c918da834001572" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a2012abfa6a48dfd53c918da834001572"></a>

设置时间戳（服务端收到时的时间）

#### `public inline long clientTimestamp()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a64f9148ddefce306a070da4e3a572600" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a64f9148ddefce306a070da4e3a572600"></a>

本地时间戳（消息创建或者收到时的本地时间）

**Returns**

int64\_t

#### `public inline void setClientTimestamp(long arg0)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a03642fa05fed94d03951f9e6e2b69a6e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a03642fa05fed94d03951f9e6e2b69a6e"></a>

设置消息本地时间戳

#### `public inline boolean isPlayed()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1aebd3f7e6fb8a7b7c130db27d2fa4c6a7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1aebd3f7e6fb8a7b7c130db27d2fa4c6a7"></a>

语音或者视频消息是否播放过，仅对收到的音视频消息有效

**Returns**

bool

#### `public inline void setIsPlayed(boolean arg0)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1aa87356d9206b28ae6dd49dd3ded4915e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1aa87356d9206b28ae6dd49dd3ded4915e"></a>

#### `public inline boolean isPlayAcked()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a462310a75e314e0ef147c3ac67b8c768" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a462310a75e314e0ef147c3ac67b8c768"></a>

语音或者视频消息是否收到播放回执，仅对收到的音视频消息有效

**Returns**

bool

#### `public inline void setIsPlayAcked(boolean arg0)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1aff79695aa05415df0cfbd7e71860317d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1aff79695aa05415df0cfbd7e71860317d"></a>

#### `public inline boolean isReceiveMsg()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a054e2f8c8bd174223815ff799ba7cd5f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a054e2f8c8bd174223815ff799ba7cd5f"></a>

是否接收的消息

**Returns**

bool

#### `public inline void setIsReceiveMsg(boolean arg0)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a0b837ee300a1be702648e4550e4e4e13" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a0b837ee300a1be702648e4550e4e4e13"></a>

#### `public inline boolean isRead()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a2e382ce373bdd3594e2dc723ebf1a4f4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a2e382ce373bdd3594e2dc723ebf1a4f4"></a>

消息是否已读标志

**Returns**

bool

#### `public inline void setIsRead(boolean arg0)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a52d976aaa75a0ca589d72b8a86aa89b7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a52d976aaa75a0ca589d72b8a86aa89b7"></a>

#### `public inline boolean isReadAcked()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ae46672f496472417b12bf858c5dbb6e1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ae46672f496472417b12bf858c5dbb6e1"></a>

对于发送方表示是否收到了已读回执，对于接收方表示是否发送了已读回执

**Returns**

bool

#### `public inline void setIsReadAcked(boolean arg0)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ab25891e09cf54c71fc5dcb5210c574b9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ab25891e09cf54c71fc5dcb5210c574b9"></a>

#### `public inline boolean isDeliveryAcked()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ac42c65dd6cd68100c8a30c6fe3aec4ff" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ac42c65dd6cd68100c8a30c6fe3aec4ff"></a>

对于发送方表示消息是否已投递到对方，对于接收方表示是否发送了消息已到达回执

**Returns**

bool

#### `public inline void setIsDeliveryAcked(boolean arg0)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a22660bb9ed2d02ca4dbc0a538f4c9a95" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a22660bb9ed2d02ca4dbc0a538f4c9a95"></a>

#### `public inline String content()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1adc9e728c3490e921215f5217e07b7e34" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1adc9e728c3490e921215f5217e07b7e34"></a>

消息文本内容

**Returns**

std::string

#### `public inline void setContent(String content)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a6e7ea4698a706cf4ce17c1806775e18c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a6e7ea4698a706cf4ce17c1806775e18c"></a>

消息文本内容

**Parameters**

* `content` 消息文本内容

#### `public inline BMXMessage.ContentType contentType()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ae1db79f272cb2ac6e168d2b6b0ad93f1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ae1db79f272cb2ac6e168d2b6b0ad93f1"></a>

消息内容类型，如果带附件就表示附件类型，不带附件就是文本类型

**Returns**

[ContentType](broken-reference)

#### `public inline` [`BMXMessageAttachment`](broken-reference) `attachment()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a2af1eb0977c8bc1db8682fe0f0c925cc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a2af1eb0977c8bc1db8682fe0f0c925cc"></a>

消息附件，BMXMessage拥有附件的所有权，负责释放

**Returns**

BMXMessageAttachmentPtr

#### `public inline` [`BMXMessageConfig`](broken-reference) `config()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1af155ca96a9cf693ac4cae6675a65b20b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1af155ca96a9cf693ac4cae6675a65b20b"></a>

消息的配置信息

**Returns**

JSON(std::string)

#### `public inline void setConfig(`[`BMXMessageConfig`](broken-reference) `arg0)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a29f3a1c19ec8589d18d2b3cd4403bbe8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a29f3a1c19ec8589d18d2b3cd4403bbe8"></a>

设置消息配置信息

#### `public inline String extension()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1aeaac4828b7073e55cc645808fb44df74" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1aeaac4828b7073e55cc645808fb44df74"></a>

消息扩展信息

**Returns**

JSON(std::string)

#### `public inline void setExtension(String arg0)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a8c60a50a1bd2559d04deb12d0c9c089e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a8c60a50a1bd2559d04deb12d0c9c089e"></a>

设置消息扩展信息

#### `public inline BMXMessage.DeliveryQos deliveryQos()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ae1ea9321ae2b86e32028869ca539e213" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ae1ea9321ae2b86e32028869ca539e213"></a>

消息投递QOS

**Returns**

[DeliveryQos](broken-reference)

#### `public inline void setDeliveryQos(BMXMessage.DeliveryQos qos)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a98cee3f34afb862b2f2967f81d0cde73" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a98cee3f34afb862b2f2967f81d0cde73"></a>

设置消息投递QOS

**Parameters**

* `qos` 消息投递QOS

#### `public inline String senderName()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a0f76f0c232976fa961be2ed08b99a560" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a0f76f0c232976fa961be2ed08b99a560"></a>

消息发送者的显示名称

**Returns**

std::string

#### `public inline void setSenderName(String senderName)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ac1e4a970d6d7bb378699a5bf7bccede9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ac1e4a970d6d7bb378699a5bf7bccede9"></a>

设置消息的发送者显示名称

**Parameters**

* `senderName` 消息文本内容

#### `public inline int groupAckCount()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a6eeba7280db4688a6981ecca219b23a1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a6eeba7280db4688a6981ecca219b23a1"></a>

群消息已读AckCount数目

**Returns**

int

#### `public inline void setGroupAckCount(int count)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a9dc8801f1b49c0b07b754dd4c0bbc1af" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a9dc8801f1b49c0b07b754dd4c0bbc1af"></a>

设置消息已读groupAckCount数目(SDK 内部调用接口，上层不应该调用)

**Parameters**

* `count` 设置群消息已读数目

#### `public inline int groupAckUnreadCount()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1af7ff968264468e70594ad8bd449f4ebc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1af7ff968264468e70594ad8bd449f4ebc"></a>

群消息未读AckCount数目

**Returns**

int

#### `public inline void setGroupAckUnreadCount(int count)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a56465c58e565ca85ae36cd804e12c578" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a56465c58e565ca85ae36cd804e12c578"></a>

设置消息未读groupAckCount数目(SDK 内部调用接口，上层不应该调用)

**Parameters**

* `count` 设置群消息未读数目

#### `public inline boolean groupAckReadAll()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ae98fa4b0e657abf44dea4bbaa5c7c4a2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ae98fa4b0e657abf44dea4bbaa5c7c4a2"></a>

群消息是否全部已读

**Returns**

bool

#### `public inline int groupPlayAckCount()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a12cc9ce14df3812f671dec4fe48e1886" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a12cc9ce14df3812f671dec4fe48e1886"></a>

获取群消息已播放计数

**Returns**

bool

#### `public inline void setGroupPlayAckCount(int count)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a0208ca8c6e8eb241d841d2aa99c516b9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a0208ca8c6e8eb241d841d2aa99c516b9"></a>

#### `public inline int groupPlayAckUnreadCount()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1aa82742b75ca0a7905eb6caba47dd0666" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1aa82742b75ca0a7905eb6caba47dd0666"></a>

获取群消息已播放回执未读计数

**Returns**

bool

#### `public inline void setGroupPlayAckUnreadCount(int count)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1af90d8cc8346d24f1972af74d642c219a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1af90d8cc8346d24f1972af74d642c219a"></a>

#### `public inline boolean groupPlayAckReadAll()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1aaf483c85fdc7a644f6f0fc7da7731918" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1aaf483c85fdc7a644f6f0fc7da7731918"></a>

设置所有群消息已播回执为已读

**Returns**

bool

#### `public inline void setPriority(int priority)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ae11befc089e32f68d79140ae036657c6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ae11befc089e32f68d79140ae036657c6"></a>

设置消息的扩散优先级，默认为0。0表示扩散，数字越小扩散的越多。 取值范围0-10。普通人在聊天室发送的消息级别默认为5，可以丢弃。管理员默认为0不会丢弃。其它值可以根据业务自行设置。

**Parameters**

* `priority` 设置群消息未读数目

#### `public inline int priority()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ad696621e99f9255597751e7db064724b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ad696621e99f9255597751e7db064724b"></a>

消息的扩散优先级

**Returns**

int

#### `public inline void setPushMessageMode(boolean arg0)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a1a6168c0efb4abb9c21cd0614c305966" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a1a6168c0efb4abb9c21cd0614c305966"></a>

设置是否推送消息

#### `public inline boolean isPushMessage()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1adea5d6c57159ad0d6dd89003646a26a5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1adea5d6c57159ad0d6dd89003646a26a5"></a>

是否是推送消息

**Returns**

boolean

#### `protected inline BMXMessage(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ab54875a779774c5259806f859d96a2e4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1ab54875a779774c5259806f859d96a2e4"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a23de4d7d2a72c9cd634e6b14498e49f8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_1a23de4d7d2a72c9cd634e6b14498e49f8"></a>

## class `BMXMessageAttachment` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment"></a>

```
class BMXMessageAttachment
  : public im.floo.floolib.BMXBaseObject
```

消息附件

### Summary

| Members                                                               | Descriptions |
| --------------------------------------------------------------------- | ------------ |
| `class` [`Size`](broken-reference)                                    | 图片/视频大小      |
| `public inline synchronized void delete()`                            |              |
| `public inline BMXMessageAttachment.Type type()`                      | 附件类型         |
| `public inline` [`BMXMessageAttachment`](broken-reference) `clone()`  | 复制附件         |
| `protected inline BMXMessageAttachment(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                                    |              |

### Members

#### `class` [`Size`](broken-reference) <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size"></a>

图片/视频大小

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1a42c8a282fd62d19381c680ba52ae7ca4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1a42c8a282fd62d19381c680ba52ae7ca4"></a>

#### `public inline BMXMessageAttachment.Type type()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1a5f00584adc16e8a24e9c8e782cc5527f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1a5f00584adc16e8a24e9c8e782cc5527f"></a>

附件类型

**Returns**

[Type](broken-reference)

#### `public inline` [`BMXMessageAttachment`](broken-reference) `clone()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1a9004e1fb0bf86302c8246d3a870c68e8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1a9004e1fb0bf86302c8246d3a870c68e8"></a>

复制附件

**Returns**

BMXMessageAttachmentPtr

#### `protected inline BMXMessageAttachment(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1a4f31d97515c3c14d1ba42d2dc06822fa" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1a4f31d97515c3c14d1ba42d2dc06822fa"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1ae172d5572b09ca3a1c2ce8875c590e1d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1ae172d5572b09ca3a1c2ce8875c590e1d"></a>

## class `Size` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size"></a>

图片/视频大小

### Summary

| Members                                               | Descriptions |
| ----------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`            |              |
| `public inline Size(double width,double height)`      |              |
| `public inline Size(double width)`                    |              |
| `public inline Size()`                                |              |
| `public inline void setMWidth(double value)`          |              |
| `public inline double getMWidth()`                    |              |
| `public inline void setMHeight(double value)`         |              |
| `public inline double getMHeight()`                   |              |
| `protected transient boolean swigCMemOwn`             |              |
| `protected inline Size(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                    |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1ae5c747ffa098d53a557b6071fb6cdb78" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1ae5c747ffa098d53a557b6071fb6cdb78"></a>

#### `public inline Size(double width,double height)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1af0de1322e881df05e319f4f5457b5694" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1af0de1322e881df05e319f4f5457b5694"></a>

#### `public inline Size(double width)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1adec85a57b1a09386c20a2d8a5246f679" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1adec85a57b1a09386c20a2d8a5246f679"></a>

#### `public inline Size()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1a806f55a7e94cf79d7e47a24bd2a252e1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1a806f55a7e94cf79d7e47a24bd2a252e1"></a>

#### `public inline void setMWidth(double value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1acdb4a53121f939c710cd64d8139330ab" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1acdb4a53121f939c710cd64d8139330ab"></a>

#### `public inline double getMWidth()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1ad2cad391ac114b723079974ec8fb0b95" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1ad2cad391ac114b723079974ec8fb0b95"></a>

#### `public inline void setMHeight(double value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1a2c5d2e7895392e84dabe5b2597bc1c5c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1a2c5d2e7895392e84dabe5b2597bc1c5c"></a>

#### `public inline double getMHeight()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1ab77c9b8a5dcb442c5e86baba76f443c6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1ab77c9b8a5dcb442c5e86baba76f443c6"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1a6470d480a75f8fcff194a649d2bde7f9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1a6470d480a75f8fcff194a649d2bde7f9"></a>

#### `protected inline Size(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1a718a6bb8a5ef41d106e4313ae518ce26" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1a718a6bb8a5ef41d106e4313ae518ce26"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1a3b70c94388f467931b0c6a02e863ad6a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_attachment_1_1_size_1a3b70c94388f467931b0c6a02e863ad6a"></a>

## class `BMXMessageList` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list"></a>

### Summary

| Members                                                                | Descriptions |
| ---------------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                             |              |
| `public inline BMXMessageList()`                                       |              |
| `public inline BMXMessageList(long n)`                                 |              |
| `public inline long size()`                                            |              |
| `public inline long capacity()`                                        |              |
| `public inline void reserve(long n)`                                   |              |
| `public inline boolean isEmpty()`                                      |              |
| `public inline void clear()`                                           |              |
| `public inline void add(`[`BMXMessage`](broken-reference) `x)`         |              |
| `public inline` [`BMXMessage`](broken-reference) `get(int i)`          |              |
| `public inline void set(int i,`[`BMXMessage`](broken-reference) `val)` |              |
| `protected transient boolean swigCMemOwn`                              |              |
| `protected inline BMXMessageList(long cPtr,boolean cMemoryOwn)`        |              |
| `protected inline void finalize()`                                     |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a30565d7b4638c373f9f0a5e781a7b513" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a30565d7b4638c373f9f0a5e781a7b513"></a>

#### `public inline BMXMessageList()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a9069daba0799488818ab5682729d0d6b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a9069daba0799488818ab5682729d0d6b"></a>

#### `public inline BMXMessageList(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1acb13c773b4db71edf26fb39b5edbe748" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1acb13c773b4db71edf26fb39b5edbe748"></a>

#### `public inline long size()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a3806345e4b606aa79092f54bbd64dbdc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a3806345e4b606aa79092f54bbd64dbdc"></a>

#### `public inline long capacity()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a0c6a04f16e3fcab03702298ccd4c4923" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a0c6a04f16e3fcab03702298ccd4c4923"></a>

#### `public inline void reserve(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a42b7934c65eb95fa648657925a98d567" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a42b7934c65eb95fa648657925a98d567"></a>

#### `public inline boolean isEmpty()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a96d0a5b1b802ad4a8716c14951e44ff0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a96d0a5b1b802ad4a8716c14951e44ff0"></a>

#### `public inline void clear()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1ab579ed55d4437d9b6509e0f536ad9ff7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1ab579ed55d4437d9b6509e0f536ad9ff7"></a>

#### `public inline void add(`[`BMXMessage`](broken-reference) `x)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a48243c31d3bddb2ae0103311de60c9e6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a48243c31d3bddb2ae0103311de60c9e6"></a>

#### `public inline` [`BMXMessage`](broken-reference) `get(int i)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a5d0b0d97d8a890ba5e2f54317180a7ec" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a5d0b0d97d8a890ba5e2f54317180a7ec"></a>

#### `public inline void set(int i,`[`BMXMessage`](broken-reference) `val)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a8335738bbaf5815fd5946afd6ec29980" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a8335738bbaf5815fd5946afd6ec29980"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a5938d4748921ffd2e54cb6606691f95c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a5938d4748921ffd2e54cb6606691f95c"></a>

#### `protected inline BMXMessageList(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a8819a6058d1f0b52b8b18d9cf526cb76" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a8819a6058d1f0b52b8b18d9cf526cb76"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a903675b276dd827470782714d8df7857" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_1a903675b276dd827470782714d8df7857"></a>

## class `BMXMessageListList` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list"></a>

### Summary

| Members                                                                    | Descriptions |
| -------------------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                                 |              |
| `public inline BMXMessageListList()`                                       |              |
| `public inline BMXMessageListList(long n)`                                 |              |
| `public inline long size()`                                                |              |
| `public inline long capacity()`                                            |              |
| `public inline void reserve(long n)`                                       |              |
| `public inline boolean isEmpty()`                                          |              |
| `public inline void clear()`                                               |              |
| `public inline void add(`[`BMXMessageList`](broken-reference) `x)`         |              |
| `public inline` [`BMXMessageList`](broken-reference) `get(int i)`          |              |
| `public inline void set(int i,`[`BMXMessageList`](broken-reference) `val)` |              |
| `protected transient boolean swigCMemOwn`                                  |              |
| `protected inline BMXMessageListList(long cPtr,boolean cMemoryOwn)`        |              |
| `protected inline void finalize()`                                         |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1a30628d2cc52ea5cbda54f8d3261cccb4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1a30628d2cc52ea5cbda54f8d3261cccb4"></a>

#### `public inline BMXMessageListList()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1aad6e90b9ce22e3969e0cf067a4853d5d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1aad6e90b9ce22e3969e0cf067a4853d5d"></a>

#### `public inline BMXMessageListList(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1aadb1be647c0d87b397f95b2c366685c9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1aadb1be647c0d87b397f95b2c366685c9"></a>

#### `public inline long size()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1af143669d1189dcee1322cfc57f282e33" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1af143669d1189dcee1322cfc57f282e33"></a>

#### `public inline long capacity()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1abdaff938ee4ae38fb0990335a1421697" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1abdaff938ee4ae38fb0990335a1421697"></a>

#### `public inline void reserve(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1ae19f9a37a28eb75183b8febdfe96fe03" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1ae19f9a37a28eb75183b8febdfe96fe03"></a>

#### `public inline boolean isEmpty()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1aa6f46c28cff959c0309889a3a3dbac94" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1aa6f46c28cff959c0309889a3a3dbac94"></a>

#### `public inline void clear()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1a9f69cbcd33c59774dad2c419f7d161df" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1a9f69cbcd33c59774dad2c419f7d161df"></a>

#### `public inline void add(`[`BMXMessageList`](broken-reference) `x)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1a3ee0ed589b4e6964aea89e48436ab48c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1a3ee0ed589b4e6964aea89e48436ab48c"></a>

#### `public inline` [`BMXMessageList`](broken-reference) `get(int i)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1a9bf235603e59915870ac6cdd999b4047" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1a9bf235603e59915870ac6cdd999b4047"></a>

#### `public inline void set(int i,`[`BMXMessageList`](broken-reference) `val)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1ad73353aff6f03d0d8b0ba421a1d6825d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1ad73353aff6f03d0d8b0ba421a1d6825d"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1a51de94fd10d54e49adb3aa411df0cdf8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1a51de94fd10d54e49adb3aa411df0cdf8"></a>

#### `protected inline BMXMessageListList(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1a143480d8b4768f6e5117e5a414a43630" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1a143480d8b4768f6e5117e5a414a43630"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1aa32dea40b2393680d93eff10d8011493" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_list_list_1aa32dea40b2393680d93eff10d8011493"></a>

## class `BMXMessagePage` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_page" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_page"></a>

```
class BMXMessagePage
  : public im.floo.floolib.BMXBaseObject
```

### Summary

| Members                                                                                     | Descriptions |
| ------------------------------------------------------------------------------------------- | ------------ |
| `public transient long swigCPtr`                                                            |              |
| `public inline synchronized void delete()`                                                  |              |
| `public inline BMXMessagePage()`                                                            |              |
| `public inline BMXMessagePage(`[`BMXMessageList`](broken-reference) `result,long offset)`   |              |
| `public inline BMXMessagePage(`[`BMXMessageList`](broken-reference) `result,String cursor)` |              |
| `public inline BMXMessagePage(`[`BMXMessagePage`](broken-reference) `from)`                 |              |
| `public inline long count()`                                                                |              |
| `public inline long offset()`                                                               |              |
| `public inline String cursor()`                                                             |              |
| `public inline` [`BMXMessageList`](broken-reference) `result()`                             |              |
| `protected inline BMXMessagePage(long cPtr,boolean cMemoryOwn)`                             |              |
| `protected inline void finalize()`                                                          |              |

### Members

#### `public transient long swigCPtr` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1a78338168489c95269de80fa37dee7c42" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1a78338168489c95269de80fa37dee7c42"></a>

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1a869f48f76c667cee15370c9a6298e3bc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1a869f48f76c667cee15370c9a6298e3bc"></a>

#### `public inline BMXMessagePage()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1ae63d2f87d7e9cca910d40dba05210046" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1ae63d2f87d7e9cca910d40dba05210046"></a>

#### `public inline BMXMessagePage(`[`BMXMessageList`](broken-reference) `result,long offset)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1aa8fceb23810fc1cd4bc459900821432a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1aa8fceb23810fc1cd4bc459900821432a"></a>

#### `public inline BMXMessagePage(`[`BMXMessageList`](broken-reference) `result,String cursor)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1ac409ea41fed8d5a01129dd1a547dca02" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1ac409ea41fed8d5a01129dd1a547dca02"></a>

#### `public inline BMXMessagePage(`[`BMXMessagePage`](broken-reference) `from)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1a5bbfab5659e72e6e4a97c36783bf96aa" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1a5bbfab5659e72e6e4a97c36783bf96aa"></a>

#### `public inline long count()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1a583df9199f82ec37d8a05d3d4660f47f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1a583df9199f82ec37d8a05d3d4660f47f"></a>

#### `public inline long offset()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1ab1ffc034044f2634bf0e85eee2bcf67a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1ab1ffc034044f2634bf0e85eee2bcf67a"></a>

#### `public inline String cursor()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1a73f552c46c5979b4888564087f0f0836" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1a73f552c46c5979b4888564087f0f0836"></a>

#### `public inline` [`BMXMessageList`](broken-reference) `result()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1a87de77abcae37d69a427b77a6c5ab8e4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1a87de77abcae37d69a427b77a6c5ab8e4"></a>

#### `protected inline BMXMessagePage(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1aca00c789d4c26a5fc20c4fd8e8e63d5a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1aca00c789d4c26a5fc20c4fd8e8e63d5a"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1a61b2f880a2897112a95bac6dd55b9afb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_message_page_1a61b2f880a2897112a95bac6dd55b9afb"></a>

## class `BMXNetworkListener` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener" id="classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener"></a>

网络监听者

### Summary

| Members                                                                                              | Descriptions |
| ---------------------------------------------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                                                           |              |
| `public inline void swigReleaseOwnership()`                                                          |              |
| `public inline void swigTakeOwnership()`                                                             |              |
| `public inline void onNetworkChanged(`[`BMXNetworkType`](broken-reference) `type,boolean reconnect)` |              |
| `public inline BMXNetworkListener()`                                                                 |              |
| `protected inline BMXNetworkListener(long cPtr,boolean cMemoryOwn)`                                  |              |
| `protected inline void finalize()`                                                                   |              |
| `protected inline void swigDirectorDisconnect()`                                                     |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener_1a6600618e27c5ca74bf2d3ce26c8dd634" id="classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener_1a6600618e27c5ca74bf2d3ce26c8dd634"></a>

#### `public inline void swigReleaseOwnership()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener_1ab21af55dec23ecc89fafba904dc7b0dd" id="classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener_1ab21af55dec23ecc89fafba904dc7b0dd"></a>

#### `public inline void swigTakeOwnership()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener_1a0c212299e5170c24e757b70c49e8bc6a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener_1a0c212299e5170c24e757b70c49e8bc6a"></a>

#### `public inline void onNetworkChanged(`[`BMXNetworkType`](broken-reference) `type,boolean reconnect)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener_1ae9b84409fd4616695fccb293e8ab2c34" id="classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener_1ae9b84409fd4616695fccb293e8ab2c34"></a>

#### `public inline BMXNetworkListener()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener_1a7ebeaca795e190fbdd824dbd5ce8b469" id="classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener_1a7ebeaca795e190fbdd824dbd5ce8b469"></a>

#### `protected inline BMXNetworkListener(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener_1a71b63979e1f05cde7228b8a441924d90" id="classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener_1a71b63979e1f05cde7228b8a441924d90"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener_1a7e9ffc0097e4d9c5764aa7bc8cdca374" id="classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener_1a7e9ffc0097e4d9c5764aa7bc8cdca374"></a>

#### `protected inline void swigDirectorDisconnect()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener_1aad66db4aced7f0561fa03ea0f20d419f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_network_listener_1aad66db4aced7f0561fa03ea0f20d419f"></a>

## class `BMXPushManager` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager"></a>

推送管理器

### Summary

| Members                                                                                                                                                                                                | Descriptions                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------- |
| `public inline BMXPushManager(`[`BMXPushService`](broken-reference) `service)`                                                                                                                         |                                                                                                |
| `public inline void start(final String alias,final String bmxToken,final BMXCallBack callBack)`                                                                                                        | 初始化推送sdk。在仅使用推送的情况下使用该接口初始化推送sdk。在同时使用IM功能的时候直接在BMXClient调用登陆功能即可。config对象初始化的时候需要传入平台类型和设备id。 |
| `public inline void start(final String alias,final BMXCallBack callBack)`                                                                                                                              |                                                                                                |
| `public inline void start(final BMXCallBack callBack)`                                                                                                                                                 |                                                                                                |
| `public inline void stop(final BMXCallBack callBack)`                                                                                                                                                  | 停止推送功能接口。                                                                                      |
| `public inline void resume(final BMXCallBack callBack)`                                                                                                                                                | 恢复推送功能接口。                                                                                      |
| `public inline void unbindAlias(final String alias,final BMXCallBack callBack)`                                                                                                                        | 解除用户别名绑定。                                                                                      |
| `public inline String getToken()`                                                                                                                                                                      | 获取登陆后使用的用户token。                                                                               |
| `public inline String getCert()`                                                                                                                                                                       | 获取登陆后服务器返回的推送证书。                                                                               |
| `public inline BMXPushService.PushSdkStatus status()`                                                                                                                                                  | 推送sdk当前的状态。                                                                                    |
| `public inline void bindDeviceToken(final String token,final BMXCallBack callBack)`                                                                                                                    | 推送绑定设备token。                                                                                   |
| `public inline void bindVoipToken(final String token,final BMXCallBack callBack)`                                                                                                                      | 绑定推送设备的voiptoken。                                                                              |
| `public inline void getPushProfile(final boolean forceRefresh,final BMXDataCallBack<` [`BMXPushUserProfile`](broken-reference) `> callBack)`                                                           | 获取推送用户详情，如果forceRefresh == true，则强制从服务端拉取                                                      |
| `public inline void setTags(final` [`TagList`](broken-reference) `tags,final String operationId,final BMXCallBack callBack)`                                                                           | 设置推送用户的标签。                                                                                     |
| `public inline void getTags(final` [`TagList`](broken-reference) `tags,final String operationId,final BMXCallBack callBack)`                                                                           | 获取推送用户的标签。                                                                                     |
| `public inline void deleteTags(final` [`TagList`](broken-reference) `tags,final String operationId,final BMXCallBack callBack)`                                                                        | 删除推送用户的标签。                                                                                     |
| `public inline void clearTags(final String operationId,final BMXCallBack callBack)`                                                                                                                    | 清空推送用户的标签。                                                                                     |
| `public inline void setBadge(final int count,final BMXCallBack callBack)`                                                                                                                              | 设置推送用户的未读角标。                                                                                   |
| `public inline void setPushMode(final boolean enable,final BMXCallBack callBack)`                                                                                                                      | 设置推送启用状态。默认为使用推送。                                                                              |
| `public inline void setPushMode(final BMXCallBack callBack)`                                                                                                                                           |                                                                                                |
| `public inline void setPushTime(final int startHour,final int endHour,final BMXCallBack callBack)`                                                                                                     | 设置允许推送时间。                                                                                      |
| `public inline void setSilenceTime(final int startHour,final int endHour,final BMXCallBack callBack)`                                                                                                  | 设置推送静默的起始结束时间。                                                                                 |
| `public inline void setRunBackgroundMode(final boolean enable,final BMXCallBack callBack)`                                                                                                             | 设置推送是否可以后台运行。默认是false。                                                                         |
| `public inline void setRunBackgroundMode(final BMXCallBack callBack)`                                                                                                                                  |                                                                                                |
| `public inline void setGeoFenceMode(final boolean enable,final boolean isAllow,final BMXCallBack callBack)`                                                                                            | 设置推送的地理围栏功能是否运行。                                                                               |
| `public inline void setGeoFenceMode(final boolean enable,final BMXCallBack callBack)`                                                                                                                  |                                                                                                |
| `public inline void setGeoFenceMode(final BMXCallBack callBack)`                                                                                                                                       |                                                                                                |
| `public inline void clearNotification(final long notificationId)`                                                                                                                                      | 清除指定id的通知。                                                                                     |
| `public inline void clearAllNotifications()`                                                                                                                                                           |                                                                                                |
| `public inline void sendMessage(final String content)`                                                                                                                                                 | 发送推送上行消息，消息状态变化会通过listener通知                                                                   |
| `public inline void loadLocalPushMessages(final long refMsgId,final long size,final` [`BMXMessageList`](broken-reference) `result,final BMXPushService.PushDirection arg3,final BMXCallBack callBack)` | 加载数据库本地存储的推送消息。如果不指定则从最新消息开始                                                                   |
| `public inline void loadLocalPushMessages(final long refMsgId,final long size,final` [`BMXMessageList`](broken-reference) `result,final BMXCallBack callBack)`                                         |                                                                                                |
| `public inline void addPushListener(`[`BMXPushServiceListener`](broken-reference) `listener)`                                                                                                          | 添加推送监听者                                                                                        |
| `public inline void removePushListener(`[`BMXPushServiceListener`](broken-reference) `listener)`                                                                                                       | 移除推送监听者                                                                                        |

### Members

#### `public inline BMXPushManager(`[`BMXPushService`](broken-reference) `service)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a5abde8dde5d3d7f9ce4834baacc89343" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a5abde8dde5d3d7f9ce4834baacc89343"></a>

#### `public inline void start(final String alias,final String bmxToken,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1aa58256fd595220d5f08628bf94d2cd98" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1aa58256fd595220d5f08628bf94d2cd98"></a>

初始化推送sdk。在仅使用推送的情况下使用该接口初始化推送sdk。在同时使用IM功能的时候直接在BMXClient调用登陆功能即可。config对象初始化的时候需要传入平台类型和设备id。

**Parameters**

* `alias` 推送初始化使用的当前用户别名
* `bmxToken` 推送初始化的时候App传入的使用的用户的token，无用户的状态下不传入即可。
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void start(final String alias,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1ad9fc5a285619d6a60964ad2b962500b5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1ad9fc5a285619d6a60964ad2b962500b5"></a>

#### `public inline void start(final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a23f20cd5f82648a403a839e29a75c72a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a23f20cd5f82648a403a839e29a75c72a"></a>

#### `public inline void stop(final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a586083b9cbfe5de76ec0ef8f990bfcd6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a586083b9cbfe5de76ec0ef8f990bfcd6"></a>

停止推送功能接口。

**Parameters**

* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void resume(final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1aad6bc23dace230332141507ea75f4aeb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1aad6bc23dace230332141507ea75f4aeb"></a>

恢复推送功能接口。

**Parameters**

* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void unbindAlias(final String alias,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a2aa819108ccefd57976c3529fa8140d6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a2aa819108ccefd57976c3529fa8140d6"></a>

解除用户别名绑定。

**Parameters**

* `alias` 需要解除绑定的用户别名。
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline String getToken()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a72ef7306e8bbc4883283649e45573c14" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a72ef7306e8bbc4883283649e45573c14"></a>

获取登陆后使用的用户token。

#### `public inline String getCert()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a94f7d0928dfecc1cd324e61a4cf8201a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a94f7d0928dfecc1cd324e61a4cf8201a"></a>

获取登陆后服务器返回的推送证书。

#### `public inline BMXPushService.PushSdkStatus status()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a7526ec0eee1e95ed9f2a3ea36f39ac2c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a7526ec0eee1e95ed9f2a3ea36f39ac2c"></a>

推送sdk当前的状态。

**Returns**

PushSdkStatus

#### `public inline void bindDeviceToken(final String token,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1aed56500a4c9a52e39e750e2b769c65c1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1aed56500a4c9a52e39e750e2b769c65c1"></a>

推送绑定设备token。

**Parameters**

* `token` 设备的推送token
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void bindVoipToken(final String token,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a1213d43c82d05d2b6c806cdd29cd0716" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a1213d43c82d05d2b6c806cdd29cd0716"></a>

绑定推送设备的voiptoken。

**Parameters**

* `token` 设备的voip推送token
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void getPushProfile(final boolean forceRefresh,final BMXDataCallBack<` [`BMXPushUserProfile`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1adfdeb9c643a946bbbe6009edc1478d0e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1adfdeb9c643a946bbbe6009edc1478d0e"></a>

获取推送用户详情，如果forceRefresh == true，则强制从服务端拉取

**Parameters**

* `forceRefresh` 是否强制从服务器拉取，本地获取失败的情况下会自动从服务器拉取
* `callBack` 推送用户profile信息，初始传入指向为空的shared\_ptr对象，函数返回后从此处获取用户profile信息

#### `public inline void setTags(final` [`TagList`](broken-reference) `tags,final String operationId,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a5527efcd35273b3570deb9aaf0e801ce" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a5527efcd35273b3570deb9aaf0e801ce"></a>

设置推送用户的标签。

**Parameters**

* `tags` 用户标签
* `operationId` 操作id。在回调通知中对应通知提醒。
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void getTags(final` [`TagList`](broken-reference) `tags,final String operationId,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a0314f15cb982f6610c04509da2f9ee2f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a0314f15cb982f6610c04509da2f9ee2f"></a>

获取推送用户的标签。

**Parameters**

* `tags` 用户标签
* `operationId` 操作id。在回调通知中对应通知提醒。
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void deleteTags(final` [`TagList`](broken-reference) `tags,final String operationId,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a1261c14b7078dc035a3ea04cbd61b6a0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a1261c14b7078dc035a3ea04cbd61b6a0"></a>

删除推送用户的标签。

**Parameters**

* `tags` 要删除用户标签
* `operationId` 操作id。在回调通知中对应通知提醒。
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void clearTags(final String operationId,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a72b9f371fbe920989a2212b570d2d6f1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a72b9f371fbe920989a2212b570d2d6f1"></a>

清空推送用户的标签。

**Parameters**

* `operationId` 操作id。在回调通知中对应通知提醒。
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setBadge(final int count,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a9188fdbb1f64dad24dbcff63ae33ccf2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a9188fdbb1f64dad24dbcff63ae33ccf2"></a>

设置推送用户的未读角标。

**Parameters**

* `count` 用户未读角标数
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setPushMode(final boolean enable,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a2d4f8d821f5900d761a798f2a1fdbc55" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a2d4f8d821f5900d761a798f2a1fdbc55"></a>

设置推送启用状态。默认为使用推送。

**Parameters**

* `enable` 推送的启用状态
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setPushMode(final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a9cdefe094f6b1f7d64a39aa4336d73eb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a9cdefe094f6b1f7d64a39aa4336d73eb"></a>

#### `public inline void setPushTime(final int startHour,final int endHour,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a694472224b33a6b7465e5a48c98573e6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a694472224b33a6b7465e5a48c98573e6"></a>

设置允许推送时间。

**Parameters**

* `startHour` 静默允许推送的起始时间小时
* `endHour` 静默允许推送的结束时间小时
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setSilenceTime(final int startHour,final int endHour,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a4fb3060fd957f0e7f2dfe8764703aa78" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a4fb3060fd957f0e7f2dfe8764703aa78"></a>

设置推送静默的起始结束时间。

**Parameters**

* `startHour` 静默推送的起始时间小时
* `endHour` 静默推送的结束时间小时
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setRunBackgroundMode(final boolean enable,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1ae4106656df64ff70fb20c7fe6970a22b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1ae4106656df64ff70fb20c7fe6970a22b"></a>

设置推送是否可以后台运行。默认是false。

**Parameters**

* `enable` 推送后台运行状态。
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setRunBackgroundMode(final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a9d3fd0dc2965e525b2372b6d200bf6bd" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a9d3fd0dc2965e525b2372b6d200bf6bd"></a>

#### `public inline void setGeoFenceMode(final boolean enable,final boolean isAllow,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a8ced52ac02b77a8dd1cad258250939d8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a8ced52ac02b77a8dd1cad258250939d8"></a>

设置推送的地理围栏功能是否运行。

**Parameters**

* `enable` 地理围栏功能是否运行。
* `isAllow` 用户是否主动弹出用户定位请求。
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setGeoFenceMode(final boolean enable,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1acd92a9157e93b8d4071553e9a860662f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1acd92a9157e93b8d4071553e9a860662f"></a>

#### `public inline void setGeoFenceMode(final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1aabac0aeb0f21fc74e741c1f0792d07cd" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1aabac0aeb0f21fc74e741c1f0792d07cd"></a>

#### `public inline void clearNotification(final long notificationId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a4d0801a956d4afb9ddcf3c0a1c193646" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a4d0801a956d4afb9ddcf3c0a1c193646"></a>

清除指定id的通知。

**Parameters**

* `notificationId` 通知id

#### `public inline void clearAllNotifications()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a3701a1da804a4f017cfc26f5d1c34f54" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a3701a1da804a4f017cfc26f5d1c34f54"></a>

#### `public inline void sendMessage(final String content)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a3d898ff9d35769aa05d08f1defebb5a3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a3d898ff9d35769aa05d08f1defebb5a3"></a>

发送推送上行消息，消息状态变化会通过listener通知

**Parameters**

* `content` 发送的上行推送消息内容

#### `public inline void loadLocalPushMessages(final long refMsgId,final long size,final` [`BMXMessageList`](broken-reference) `result,final BMXPushService.PushDirection arg3,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a0b90a16e5dd725560544c458edd8e034" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a0b90a16e5dd725560544c458edd8e034"></a>

加载数据库本地存储的推送消息。如果不指定则从最新消息开始

**Parameters**

* `refMsgId` 加载推送消息的起始id
* `size` 最大加载消息条数
* `result` 数据库返回的加载本地推送消息列表
* `arg3` 加载推送消息的方向，默认是加载更早的消息

#### `public inline void loadLocalPushMessages(final long refMsgId,final long size,final` [`BMXMessageList`](broken-reference) `result,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1af2201493a73294c2896b8aff9dd8f768" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1af2201493a73294c2896b8aff9dd8f768"></a>

#### `public inline void addPushListener(`[`BMXPushServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a5e7f06900fcf63638a1eefbe3490451e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a5e7f06900fcf63638a1eefbe3490451e"></a>

添加推送监听者

**Parameters**

* `listener` 推送监听者

#### `public inline void removePushListener(`[`BMXPushServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a5a09621c35c3bf55b0c020764778d137" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_manager_1a5a09621c35c3bf55b0c020764778d137"></a>

移除推送监听者

**Parameters**

* `listener` 推送监听者

## class `BMXPushService` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service"></a>

### Summary

| Members                                                                                                                                                                             | Descriptions                                                                                   |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `public inline synchronized void delete()`                                                                                                                                          |                                                                                                |
| `public inline` [`BMXErrorCode`](broken-reference) `start(String alias,String bmxToken)`                                                                                            | 初始化推送sdk。在仅使用推送的情况下使用该接口初始化推送sdk。在同时使用IM功能的时候直接在BMXClient调用登陆功能即可。config对象初始化的时候需要传入平台类型和设备id。 |
| `public inline` [`BMXErrorCode`](broken-reference) `start(String alias)`                                                                                                            |                                                                                                |
| `public inline` [`BMXErrorCode`](broken-reference) `start()`                                                                                                                        |                                                                                                |
| `public inline` [`BMXErrorCode`](broken-reference) `stop()`                                                                                                                         | 停止推送功能接口。                                                                                      |
| `public inline` [`BMXErrorCode`](broken-reference) `resume()`                                                                                                                       | 恢复推送功能接口。                                                                                      |
| `public inline` [`BMXErrorCode`](broken-reference) `unbindAlias(String alias)`                                                                                                      | 解除用户别名绑定。                                                                                      |
| `public inline String getToken()`                                                                                                                                                   | 获取登陆后使用的用户token。                                                                               |
| `public inline String getCert()`                                                                                                                                                    | 获取登陆后服务器返回的推送证书。                                                                               |
| `public inline BMXPushService.PushSdkStatus status()`                                                                                                                               | 推送sdk当前的状态。                                                                                    |
| `public inline` [`BMXErrorCode`](broken-reference) `bindDeviceToken(String token)`                                                                                                  | 推送绑定设备token。                                                                                   |
| `public inline` [`BMXErrorCode`](broken-reference) `bindVoipToken(String token)`                                                                                                    | 绑定推送设备的voiptoken。                                                                              |
| `public inline` [`BMXErrorCode`](broken-reference) `getPushProfile(`[`BMXPushUserProfile`](broken-reference) `pushProfile,boolean forceRefresh)`                                    | 获取推送用户详情，如果forceRefresh == true，则强制从服务端拉取                                                      |
| `public inline` [`BMXErrorCode`](broken-reference) `setTags(`[`TagList`](broken-reference) `tags,String operationId)`                                                               | 设置推送用户的标签。                                                                                     |
| `public inline` [`BMXErrorCode`](broken-reference) `getTags(`[`TagList`](broken-reference) `tags,String operationId)`                                                               | 获取推送用户的标签。                                                                                     |
| `public inline` [`BMXErrorCode`](broken-reference) `deleteTags(`[`TagList`](broken-reference) `tags,String operationId)`                                                            | 删除推送用户的标签。                                                                                     |
| `public inline` [`BMXErrorCode`](broken-reference) `clearTags(String operationId)`                                                                                                  | 清空推送用户的标签。                                                                                     |
| `public inline` [`BMXErrorCode`](broken-reference) `setBadge(int count)`                                                                                                            | 设置推送用户的未读角标。                                                                                   |
| `public inline` [`BMXErrorCode`](broken-reference) `setPushMode(boolean enable)`                                                                                                    | 设置推送启用状态。默认为使用推送。                                                                              |
| `public inline` [`BMXErrorCode`](broken-reference) `setPushMode()`                                                                                                                  |                                                                                                |
| `public inline` [`BMXErrorCode`](broken-reference) `setPushTime(int startHour,int endHour)`                                                                                         | 设置允许推送时间。                                                                                      |
| `public inline` [`BMXErrorCode`](broken-reference) `setSilenceTime(int startHour,int endHour)`                                                                                      | 设置推送静默的起始结束时间。                                                                                 |
| `public inline` [`BMXErrorCode`](broken-reference) `setRunBackgroundMode(boolean enable)`                                                                                           | 设置推送是否可以后台运行。默认是false。                                                                         |
| `public inline` [`BMXErrorCode`](broken-reference) `setRunBackgroundMode()`                                                                                                         |                                                                                                |
| `public inline` [`BMXErrorCode`](broken-reference) `setGeoFenceMode(boolean enable,boolean isAllow)`                                                                                | 设置推送的地理围栏功能是否运行。                                                                               |
| `public inline` [`BMXErrorCode`](broken-reference) `setGeoFenceMode(boolean enable)`                                                                                                |                                                                                                |
| `public inline` [`BMXErrorCode`](broken-reference) `setGeoFenceMode()`                                                                                                              |                                                                                                |
| `public inline void clearNotification(long notificationId)`                                                                                                                         | 清除指定id的通知。                                                                                     |
| `public inline void clearAllNotifications()`                                                                                                                                        |                                                                                                |
| `public inline void sendMessage(String content)`                                                                                                                                    | 发送推送上行消息，消息状态变化会通过listener通知                                                                   |
| `public inline` [`BMXErrorCode`](broken-reference) `loadLocalPushMessages(long refMsgId,long size,`[`BMXMessageList`](broken-reference) `result,BMXPushService.PushDirection arg3)` | 加载数据库本地存储的推送消息。如果不指定则从最新消息开始                                                                   |
| `public inline` [`BMXErrorCode`](broken-reference) `loadLocalPushMessages(long refMsgId,long size,`[`BMXMessageList`](broken-reference) `result)`                                   |                                                                                                |
| `public inline void addPushListener(`[`BMXPushServiceListener`](broken-reference) `listener)`                                                                                       | 添加推送监听者                                                                                        |
| `public inline void removePushListener(`[`BMXPushServiceListener`](broken-reference) `listener)`                                                                                    | 移除推送监听者                                                                                        |
| `protected transient boolean swigCMemOwn`                                                                                                                                           |                                                                                                |
| `protected inline BMXPushService(long cPtr,boolean cMemoryOwn)`                                                                                                                     |                                                                                                |
| `protected inline void finalize()`                                                                                                                                                  |                                                                                                |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a0a95d53d973a3eedd85dd3d0efb7b4c2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a0a95d53d973a3eedd85dd3d0efb7b4c2"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `start(String alias,String bmxToken)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a654354c695554f5537ca0ac500a3467b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a654354c695554f5537ca0ac500a3467b"></a>

初始化推送sdk。在仅使用推送的情况下使用该接口初始化推送sdk。在同时使用IM功能的时候直接在BMXClient调用登陆功能即可。config对象初始化的时候需要传入平台类型和设备id。

**Parameters**

* `alias` 推送初始化使用的当前用户别名
* `bmxToken` 推送初始化的时候App传入的使用的用户的token，无用户的状态下不传入即可。

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `start(String alias)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a6d63f6b994b71f1d62127f521a212712" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a6d63f6b994b71f1d62127f521a212712"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `start()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1abb136b58efe77d1b791f5d6f6837d5bc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1abb136b58efe77d1b791f5d6f6837d5bc"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `stop()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1add53c4d08ca6e8e51c23b2bb95807bbe" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1add53c4d08ca6e8e51c23b2bb95807bbe"></a>

停止推送功能接口。

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `resume()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a76c79d47975274c44e207cf27738cbcc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a76c79d47975274c44e207cf27738cbcc"></a>

恢复推送功能接口。

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `unbindAlias(String alias)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a750c2e3f373049edb0a0c00ffa3f3553" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a750c2e3f373049edb0a0c00ffa3f3553"></a>

解除用户别名绑定。

**Parameters**

* `alias` 需要解除绑定的用户别名。

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline String getToken()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a088aa93c1fae769084855c8b0077be5b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a088aa93c1fae769084855c8b0077be5b"></a>

获取登陆后使用的用户token。

#### `public inline String getCert()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a4d3ca4ee142260df6925798cadc21596" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a4d3ca4ee142260df6925798cadc21596"></a>

获取登陆后服务器返回的推送证书。

#### `public inline BMXPushService.PushSdkStatus status()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1afd24e93979bfdd1d034162839aff82ea" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1afd24e93979bfdd1d034162839aff82ea"></a>

推送sdk当前的状态。

**Returns**

[PushSdkStatus](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `bindDeviceToken(String token)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1ae83b02b7377ecd808eba71539855ce53" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1ae83b02b7377ecd808eba71539855ce53"></a>

推送绑定设备token。

**Parameters**

* `token` 设备的推送token

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `bindVoipToken(String token)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a65e92f31924bc7a7b3520021c9ac4554" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a65e92f31924bc7a7b3520021c9ac4554"></a>

绑定推送设备的voiptoken。

**Parameters**

* `token` 设备的voip推送token

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getPushProfile(`[`BMXPushUserProfile`](broken-reference) `pushProfile,boolean forceRefresh)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a2e6ab7ffaa0c2630a7dd1e98593efc7a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a2e6ab7ffaa0c2630a7dd1e98593efc7a"></a>

获取推送用户详情，如果forceRefresh == true，则强制从服务端拉取

**Parameters**

* `pushProfile` 推送用户profile信息，初始传入指向为空的shared\_ptr对象，函数返回后从此处获取用户profile信息。
* `forceRefresh` 是否强制从服务器拉取，本地获取失败的情况下会自动从服务器拉取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setTags(`[`TagList`](broken-reference) `tags,String operationId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1ad283f917f020a202c77284a629614bb7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1ad283f917f020a202c77284a629614bb7"></a>

设置推送用户的标签。

**Parameters**

* `tags` 用户标签
* `operationId` 操作id。在回调通知中对应通知提醒。

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getTags(`[`TagList`](broken-reference) `tags,String operationId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a108d008aca92cac85521cf5fa7daef6a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a108d008aca92cac85521cf5fa7daef6a"></a>

获取推送用户的标签。

**Parameters**

* `tags` 用户标签
* `operationId` 操作id。在回调通知中对应通知提醒。

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `deleteTags(`[`TagList`](broken-reference) `tags,String operationId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1ab154e74bf49445ef48704fd786556739" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1ab154e74bf49445ef48704fd786556739"></a>

删除推送用户的标签。

**Parameters**

* `tags` 要删除用户标签
* `operationId` 操作id。在回调通知中对应通知提醒。

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `clearTags(String operationId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a465b78cb3820d7694eb0bc07f52cedc2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a465b78cb3820d7694eb0bc07f52cedc2"></a>

清空推送用户的标签。

**Parameters**

* `operationId` 操作id。在回调通知中对应通知提醒。

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setBadge(int count)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a3e4ced7b0fc902ddec8ebb0228d2b83c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a3e4ced7b0fc902ddec8ebb0228d2b83c"></a>

设置推送用户的未读角标。

**Parameters**

* `count` 用户未读角标数

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setPushMode(boolean enable)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a160da0c0ff177022824cdd001c090564" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a160da0c0ff177022824cdd001c090564"></a>

设置推送启用状态。默认为使用推送。

**Parameters**

* `enable` 推送的启用状态

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setPushMode()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a04ba382e8dd001893fd074093d76ac0a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a04ba382e8dd001893fd074093d76ac0a"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `setPushTime(int startHour,int endHour)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a83131a3109de7d09872b3bf2dfd1ad03" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a83131a3109de7d09872b3bf2dfd1ad03"></a>

设置允许推送时间。

**Parameters**

* `startHour` 静默允许推送的起始时间小时
* `endHour` 静默允许推送的结束时间小时

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setSilenceTime(int startHour,int endHour)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1ae2a51a3c659b3e77f22fa1953851b2d4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1ae2a51a3c659b3e77f22fa1953851b2d4"></a>

设置推送静默的起始结束时间。

**Parameters**

* `startHour` 静默推送的起始时间小时
* `endHour` 静默推送的结束时间小时

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setRunBackgroundMode(boolean enable)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a75e5ba16e726ee74e15a9d0fc65bb713" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a75e5ba16e726ee74e15a9d0fc65bb713"></a>

设置推送是否可以后台运行。默认是false。

**Parameters**

* `enable` 推送后台运行状态。

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setRunBackgroundMode()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a66bd4e5d90ac537de6a778de0e949f71" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a66bd4e5d90ac537de6a778de0e949f71"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `setGeoFenceMode(boolean enable,boolean isAllow)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a17896e40820a0e6d16e18b2756e6c7fb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a17896e40820a0e6d16e18b2756e6c7fb"></a>

设置推送的地理围栏功能是否运行。

**Parameters**

* `enable` 地理围栏功能是否运行。
* `isAllow` 用户是否主动弹出用户定位请求。

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setGeoFenceMode(boolean enable)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1ac39a85087e11c0f99f6f1c42904b8cc5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1ac39a85087e11c0f99f6f1c42904b8cc5"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `setGeoFenceMode()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a477aae832056ec6bd80447be09eb23f5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a477aae832056ec6bd80447be09eb23f5"></a>

#### `public inline void clearNotification(long notificationId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a0d1e80c1e035073eca607fb761aabde2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a0d1e80c1e035073eca607fb761aabde2"></a>

清除指定id的通知。

**Parameters**

* `notificationId` 通知id

#### `public inline void clearAllNotifications()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1aca9e4da5ff1927477fb3190362490758" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1aca9e4da5ff1927477fb3190362490758"></a>

#### `public inline void sendMessage(String content)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1adac1fb598347574404d2750cc22f749b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1adac1fb598347574404d2750cc22f749b"></a>

发送推送上行消息，消息状态变化会通过listener通知

**Parameters**

* `content` 发送的上行推送消息内容

#### `public inline` [`BMXErrorCode`](broken-reference) `loadLocalPushMessages(long refMsgId,long size,`[`BMXMessageList`](broken-reference) `result,BMXPushService.PushDirection arg3)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1ab1735d1123a73b23f236749c26c1c987" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1ab1735d1123a73b23f236749c26c1c987"></a>

加载数据库本地存储的推送消息。如果不指定则从最新消息开始

**Parameters**

* `refMsgId` 加载推送消息的起始id
* `size` 最大加载消息条数
* `result` 数据库返回的加载本地推送消息列表
* `arg3` 加载推送消息的方向，默认是加载更早的消息

#### `public inline` [`BMXErrorCode`](broken-reference) `loadLocalPushMessages(long refMsgId,long size,`[`BMXMessageList`](broken-reference) `result)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a71d968bb36c173124beed9c8b197a75f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a71d968bb36c173124beed9c8b197a75f"></a>

#### `public inline void addPushListener(`[`BMXPushServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a9cdcfe432df120c666720f5ce6d1f3f7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a9cdcfe432df120c666720f5ce6d1f3f7"></a>

添加推送监听者

**Parameters**

* `listener` 推送监听者

#### `public inline void removePushListener(`[`BMXPushServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1ad78a4540c96834976961426286c84fa7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1ad78a4540c96834976961426286c84fa7"></a>

移除推送监听者

**Parameters**

* `listener` 推送监听者

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1aed7e26dc0c571ee980e96c825b5be437" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1aed7e26dc0c571ee980e96c825b5be437"></a>

#### `protected inline BMXPushService(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a5eb08e62b11318106bfe2c150add8598" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1a5eb08e62b11318106bfe2c150add8598"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1abcd3a56d0958aceacefdab1494b07aef" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_1abcd3a56d0958aceacefdab1494b07aef"></a>

## class `BMXPushServiceListener` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener"></a>

### Summary

| Members                                                                                                                 | Descriptions      |
| ----------------------------------------------------------------------------------------------------------------------- | ----------------- |
| `public inline synchronized void delete()`                                                                              |                   |
| `public inline void swigReleaseOwnership()`                                                                             |                   |
| `public inline void swigTakeOwnership()`                                                                                |                   |
| `public inline void onPushStart(String bmxToken)`                                                                       | Push初始化完成通知。      |
| `public inline void onPushStop()`                                                                                       | Push功能停止通知。       |
| `public inline void onCertRetrieved(String cert)`                                                                       | Push初始化完成后获取推送证书。 |
| `public inline void onSetTags(String operationId)`                                                                      | 设置用户推送成功回调。       |
| `public inline void onGetTags(String operationId)`                                                                      | 获取用户推送成功回调。       |
| `public inline void onDeleteTags(String operationId)`                                                                   | 删除用户推送成功回调。       |
| `public inline void onClearTags(String operationId)`                                                                    | 清空用户推送成功回调。       |
| `public inline void onReceivePush(`[`BMXMessageList`](broken-reference) `list)`                                         | 接收到新的Push通知。      |
| `public inline void onStatusChanged(`[`BMXMessage`](broken-reference) `msg,`[`BMXErrorCode`](broken-reference) `error)` | 发送Push上行消息状态变化通知。 |
| `public inline BMXPushServiceListener()`                                                                                |                   |
| `public inline void registerPushService(`[`BMXPushService`](broken-reference) `service)`                                |                   |
| `protected transient boolean swigCMemOwn`                                                                               |                   |
| `protected inline BMXPushServiceListener(long cPtr,boolean cMemoryOwn)`                                                 |                   |
| `protected inline void finalize()`                                                                                      |                   |
| `protected inline void swigDirectorDisconnect()`                                                                        |                   |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a7b226f773e71533f785c8decc5bc043d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a7b226f773e71533f785c8decc5bc043d"></a>

#### `public inline void swigReleaseOwnership()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a33886e13c472cc32e781d3502895c3cd" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a33886e13c472cc32e781d3502895c3cd"></a>

#### `public inline void swigTakeOwnership()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a602614028a1ee0f26fb08a8c1dbd644f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a602614028a1ee0f26fb08a8c1dbd644f"></a>

#### `public inline void onPushStart(String bmxToken)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1aac5ff51b1790a2e782c95e4e62b24b23" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1aac5ff51b1790a2e782c95e4e62b24b23"></a>

Push初始化完成通知。

**Parameters**

* `bmxToken` 当前push使用bmxToken

#### `public inline void onPushStop()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1ab4bb00f4ab554cad86925aad796a5b63" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1ab4bb00f4ab554cad86925aad796a5b63"></a>

Push功能停止通知。

#### `public inline void onCertRetrieved(String cert)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a3c1dad0237d18efd23a5bc8f18c09592" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a3c1dad0237d18efd23a5bc8f18c09592"></a>

Push初始化完成后获取推送证书。

**Parameters**

* `cert` 从服务器获取的推送证书

#### `public inline void onSetTags(String operationId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1aab240ba588be1c9608c5742a3be6e118" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1aab240ba588be1c9608c5742a3be6e118"></a>

设置用户推送成功回调。

**Parameters**

* `operationId` 操作id

#### `public inline void onGetTags(String operationId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a09ad0f568c6e54d0a730aa1772aa445a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a09ad0f568c6e54d0a730aa1772aa445a"></a>

获取用户推送成功回调。

**Parameters**

* `operationId` 操作id

#### `public inline void onDeleteTags(String operationId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a6f79ba1b1bb964f455bd0b93a05b26ff" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a6f79ba1b1bb964f455bd0b93a05b26ff"></a>

删除用户推送成功回调。

**Parameters**

* `operationId` 操作id

#### `public inline void onClearTags(String operationId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1acb79fb18b7a7026c7e8ffe7674c4b797" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1acb79fb18b7a7026c7e8ffe7674c4b797"></a>

清空用户推送成功回调。

**Parameters**

* `operationId` 操作id

#### `public inline void onReceivePush(`[`BMXMessageList`](broken-reference) `list)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a1de007055a488b21c2753cc2813f80f7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a1de007055a488b21c2753cc2813f80f7"></a>

接收到新的Push通知。

**Parameters**

* `list` Push通知列表

#### `public inline void onStatusChanged(`[`BMXMessage`](broken-reference) `msg,`[`BMXErrorCode`](broken-reference) `error)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a66e530c1b7cb7d367c34387b0c503442" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a66e530c1b7cb7d367c34387b0c503442"></a>

发送Push上行消息状态变化通知。

**Parameters**

* `msg` 发生状态变化的上行消息
* `error` 状态错误码

#### `public inline BMXPushServiceListener()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1ab93689a3f1a3c2da3a86561c33744840" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1ab93689a3f1a3c2da3a86561c33744840"></a>

#### `public inline void registerPushService(`[`BMXPushService`](broken-reference) `service)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a61b9da0e4a2f749aba6812a5f02413f0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a61b9da0e4a2f749aba6812a5f02413f0"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a8dd08a302bacb3cd6390ad26135d4d84" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a8dd08a302bacb3cd6390ad26135d4d84"></a>

#### `protected inline BMXPushServiceListener(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a3dcaa26912ae31dc1921b4d5b72f37dd" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a3dcaa26912ae31dc1921b4d5b72f37dd"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1ac8f5494fb01418ad55ee8e0053797c60" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1ac8f5494fb01418ad55ee8e0053797c60"></a>

#### `protected inline void swigDirectorDisconnect()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a9fd0a24de15be7900b3cfecc1d777368" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_service_listener_1a9fd0a24de15be7900b3cfecc1d777368"></a>

## class `BMXPushUserProfile` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile"></a>

```
class BMXPushUserProfile
  : public im.floo.floolib.BMXBaseObject
```

### Summary

| Members                                                                    | Descriptions |
| -------------------------------------------------------------------------- | ------------ |
| `class` [`MessagePushSetting`](broken-reference)                           |              |
| `public transient long swigCPtr`                                           |              |
| `public inline BMXPushUserProfile()`                                       |              |
| `public inline synchronized void delete()`                                 |              |
| `public inline long userId()`                                              |              |
| `public inline String pushAlias()`                                         |              |
| `public inline String pushToken()`                                         |              |
| `public inline BMXPushUserProfile.MessagePushSetting messagePushSetting()` |              |
| `protected inline BMXPushUserProfile(long cPtr,boolean cMemoryOwn)`        |              |
| `protected inline void finalize()`                                         |              |

### Members

#### `class` [`MessagePushSetting`](broken-reference) <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting"></a>

#### `public transient long swigCPtr` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1ad993a57670db743cc677750a19b75c49" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1ad993a57670db743cc677750a19b75c49"></a>

#### `public inline BMXPushUserProfile()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1ac8402283dc494440c9a3e76ff621697e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1ac8402283dc494440c9a3e76ff621697e"></a>

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1ab4fa11f6c9a0237f469bb618ccb641f3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1ab4fa11f6c9a0237f469bb618ccb641f3"></a>

#### `public inline long userId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1af0d9f71a1022294cfc1c4b91e89809df" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1af0d9f71a1022294cfc1c4b91e89809df"></a>

#### `public inline String pushAlias()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1a7d3a4326321590313d1a3406b7ec2f13" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1a7d3a4326321590313d1a3406b7ec2f13"></a>

#### `public inline String pushToken()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1ac72485dd3cc98d5db223e239c52c41b7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1ac72485dd3cc98d5db223e239c52c41b7"></a>

#### `public inline BMXPushUserProfile.MessagePushSetting messagePushSetting()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1a4b1988f8763f5ecb65972eb2b2c9f92b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1a4b1988f8763f5ecb65972eb2b2c9f92b"></a>

#### `protected inline BMXPushUserProfile(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1ac7733b0020c6aefc8d9cec1b0100ff7b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1ac7733b0020c6aefc8d9cec1b0100ff7b"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1a224024b685e0afc49e63f7f7685dae75" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1a224024b685e0afc49e63f7f7685dae75"></a>

## class `MessagePushSetting` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting"></a>

### Summary

| Members                                                             | Descriptions |
| ------------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                          |              |
| `public inline MessagePushSetting()`                                |              |
| `public inline void setMPushEnabled(boolean value)`                 |              |
| `public inline boolean getMPushEnabled()`                           |              |
| `public inline void setMSilenceStartTime(int value)`                |              |
| `public inline int getMSilenceStartTime()`                          |              |
| `public inline void setMSilenceEndTime(int value)`                  |              |
| `public inline int getMSilenceEndTime()`                            |              |
| `public inline void setMPushStartTime(int value)`                   |              |
| `public inline int getMPushStartTime()`                             |              |
| `public inline void setMPushEndTime(int value)`                     |              |
| `public inline int getMPushEndTime()`                               |              |
| `protected transient boolean swigCMemOwn`                           |              |
| `protected inline MessagePushSetting(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                                  |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1ac8cf5baefa2405614f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1ac8cf5baefa2405614f"></a>

#### `public inline MessagePushSetting()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1aa8da3f8bb4a6e885e4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1aa8da3f8bb4a6e885e4"></a>

#### `public inline void setMPushEnabled(boolean value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1a9e3b58be27a5ca0843" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1a9e3b58be27a5ca0843"></a>

#### `public inline boolean getMPushEnabled()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1a4eac57a20ba8a5f162" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1a4eac57a20ba8a5f162"></a>

#### `public inline void setMSilenceStartTime(int value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1ad2894e8717c81def03" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1ad2894e8717c81def03"></a>

#### `public inline int getMSilenceStartTime()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1aaf944a8bff1e8e41a1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1aaf944a8bff1e8e41a1"></a>

#### `public inline void setMSilenceEndTime(int value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1a49c28aec8189fea9e4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1a49c28aec8189fea9e4"></a>

#### `public inline int getMSilenceEndTime()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1abe4ce7e8400df38476" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1abe4ce7e8400df38476"></a>

#### `public inline void setMPushStartTime(int value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1aa2f55283f3a6636209" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1aa2f55283f3a6636209"></a>

#### `public inline int getMPushStartTime()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1abb0375e48bc77a0990" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1abb0375e48bc77a0990"></a>

#### `public inline void setMPushEndTime(int value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1ab16baa1eff65d5a918" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1ab16baa1eff65d5a918"></a>

#### `public inline int getMPushEndTime()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1abbc8a36fce80fd4307" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1abbc8a36fce80fd4307"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1ab159b8ba1d4434ca2a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1ab159b8ba1d4434ca2a"></a>

#### `protected inline MessagePushSetting(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1a71986f6c0402c7efca" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1a71986f6c0402c7efca"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1a2598152b2bd8d32340" id="classim_1_1floo_1_1floolib_1_1_b_m_x_push_user_profile_1_1_message_push_setting_1a2598152b2bd8d32340"></a>

## class `BMXRosterItemList` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list"></a>

### Summary

| Members                                                                   | Descriptions |
| ------------------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                                |              |
| `public inline BMXRosterItemList()`                                       |              |
| `public inline BMXRosterItemList(long n)`                                 |              |
| `public inline long size()`                                               |              |
| `public inline long capacity()`                                           |              |
| `public inline void reserve(long n)`                                      |              |
| `public inline boolean isEmpty()`                                         |              |
| `public inline void clear()`                                              |              |
| `public inline void add(`[`BMXRosterItem`](broken-reference) `x)`         |              |
| `public inline` [`BMXRosterItem`](broken-reference) `get(int i)`          |              |
| `public inline void set(int i,`[`BMXRosterItem`](broken-reference) `val)` |              |
| `protected transient boolean swigCMemOwn`                                 |              |
| `protected inline BMXRosterItemList(long cPtr,boolean cMemoryOwn)`        |              |
| `protected inline void finalize()`                                        |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1affdc1dfe6601a76a71e35643ad6a3050" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1affdc1dfe6601a76a71e35643ad6a3050"></a>

#### `public inline BMXRosterItemList()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1afc3da3b0b6cffb06b60a91ba0ea3257e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1afc3da3b0b6cffb06b60a91ba0ea3257e"></a>

#### `public inline BMXRosterItemList(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1acabdce1a2acee4a567e54a349d943a20" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1acabdce1a2acee4a567e54a349d943a20"></a>

#### `public inline long size()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1abfcd5c61fbec360981d5dbdbc48c1b2c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1abfcd5c61fbec360981d5dbdbc48c1b2c"></a>

#### `public inline long capacity()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1a77ba7c7882db6f25c8880d24243d1eed" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1a77ba7c7882db6f25c8880d24243d1eed"></a>

#### `public inline void reserve(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1ab2abecd5224e5654bd30b85016f808af" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1ab2abecd5224e5654bd30b85016f808af"></a>

#### `public inline boolean isEmpty()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1afb559c4aece9f6952e25e3c55464f475" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1afb559c4aece9f6952e25e3c55464f475"></a>

#### `public inline void clear()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1a7b23c682fa034687b807752582519e6c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1a7b23c682fa034687b807752582519e6c"></a>

#### `public inline void add(`[`BMXRosterItem`](broken-reference) `x)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1a73b78cd2051e67a4fe90528b2bcec74a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1a73b78cd2051e67a4fe90528b2bcec74a"></a>

#### `public inline` [`BMXRosterItem`](broken-reference) `get(int i)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1a60cfa36badc9a6eb0fa262d4efcb35b1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1a60cfa36badc9a6eb0fa262d4efcb35b1"></a>

#### `public inline void set(int i,`[`BMXRosterItem`](broken-reference) `val)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1a9ba097419ad283cd40b7e4e02d2078f3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1a9ba097419ad283cd40b7e4e02d2078f3"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1a2e0d457a7bec3b2d20ed1302c7164cbc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1a2e0d457a7bec3b2d20ed1302c7164cbc"></a>

#### `protected inline BMXRosterItemList(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1a9f0866f19ad6748fa0898e66ab332f3e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1a9f0866f19ad6748fa0898e66ab332f3e"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1a9bc9c761e62c8bb03f4915a444eee872" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_item_list_1a9bc9c761e62c8bb03f4915a444eee872"></a>

## class `BMXRosterManager` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager"></a>

好友管理器

### Summary

| Members                                                                                                                                                                                     | Descriptions                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------- |
| `public inline BMXRosterManager(`[`BMXRosterService`](broken-reference) `service)`                                                                                                          |                                         |
| `public inline void get(final boolean forceRefresh,final BMXDataCallBack<` [`ListOfLongLong`](broken-reference) `> callBack)`                                                               | 获取好友列表，如果forceRefresh == true，则强制从服务端拉取 |
| `public inline void search(final long rosterId,final boolean forceRefresh,final BMXDataCallBack<` [`BMXRosterItem`](broken-reference) `> callBack)`                                         | 搜索用户                                    |
| `public inline void search(final String name,final boolean forceRefresh,final BMXDataCallBack<` [`BMXRosterItem`](broken-reference) `> callBack)`                                           | 搜索用户                                    |
| `public inline void search(final` [`ListOfLongLong`](broken-reference)`rosterIdList,final boolean forceRefresh,final BMXDataCallBack<`[`BMXRosterItemList`](broken-reference) `> callBack)` | 批量搜索用户                                  |
| `public inline void setItemExtension(final` [`BMXRosterItem`](broken-reference) `item,final String extension,final BMXCallBack callBack)`                                                   | 更新好友本地扩展信息                              |
| `public inline void setItemAlias(final` [`BMXRosterItem`](broken-reference) `item,final String alias,final BMXCallBack callBack)`                                                           | 更新好友别名                                  |
| `public inline void setItemMuteNotification(final` [`BMXRosterItem`](broken-reference) `item,final boolean status,final BMXCallBack callBack)`                                              | 设置是否拒收用户消息                              |
| `public inline void apply(final long rosterId,final String message,final BMXCallBack callBack)`                                                                                             | 申请添加好友                                  |
| `public inline void remove(final long rosterId,final BMXCallBack callBack)`                                                                                                                 | 删除好友                                    |
| `public inline void getApplicationList(final String cursor,final int pageSize,final BMXDataCallBack<` [`ApplicationPage`](broken-reference) `> callBack)`                                   | 获取申请添加好友列表                              |
| `public inline void accept(final long rosterId,final BMXCallBack callBack)`                                                                                                                 | 接受加好友申请                                 |
| `public inline void decline(final long rosterId,final String reason,final BMXCallBack callBack)`                                                                                            | 拒绝加好友申请                                 |
| `public inline void block(final long rosterId,final BMXCallBack callBack)`                                                                                                                  | 加入黑名单                                   |
| `public inline void unblock(final long rosterId,final BMXCallBack callBack)`                                                                                                                | 从黑名单移除                                  |
| `public inline void getBlockList(final boolean forceRefresh,final BMXDataCallBack<` [`ListOfLongLong`](broken-reference) `> callBack)`                                                      | 获取黑名单，如果forceRefresh == true，则强制从服务端拉取  |
| `public inline void downloadAvatar(final` [`BMXRosterItem`](broken-reference)`item,final`[`FileProgressListener`](broken-reference) `listener,final BMXCallBack callBack)`                  | 下载头像                                    |
| `public inline void addRosterListener(`[`BMXRosterServiceListener`](broken-reference) `listener)`                                                                                           | 添加好友变化监听者                               |
| `public inline void removeRosterListener(`[`BMXRosterServiceListener`](broken-reference) `listener)`                                                                                        | 移除好友变化监听者                               |

### Members

#### `public inline BMXRosterManager(`[`BMXRosterService`](broken-reference) `service)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1a91d64bc423d92ed812cc9c3936f4a21d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1a91d64bc423d92ed812cc9c3936f4a21d"></a>

#### `public inline void get(final boolean forceRefresh,final BMXDataCallBack<` [`ListOfLongLong`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1a3d5c87353e8cf7695899359567fb85db" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1a3d5c87353e8cf7695899359567fb85db"></a>

获取好友列表，如果forceRefresh == true，则强制从服务端拉取

**Parameters**

* `forceRefresh` 是否从服务器读取数据，true为强制从服务器获取，false情况下本地读取列表为空的情况下会自动从服务器读取
* `callBack` [BMXErrorCode](broken-reference) 好友id列表

#### `public inline void search(final long rosterId,final boolean forceRefresh,final BMXDataCallBack<` [`BMXRosterItem`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1ae333c7b21614b470600d42ad613b89f9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1ae333c7b21614b470600d42ad613b89f9"></a>

搜索用户

**Parameters**

* `rosterId` 搜索的好友id
* `forceRefresh` 为true强制从服务器获取，为false情况下查询结果为空时自动从服务器获取。
* `callBack` [BMXErrorCode](broken-reference) 查询返回的用户的信息

#### `public inline void search(final String name,final boolean forceRefresh,final BMXDataCallBack<` [`BMXRosterItem`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1ad6a35329806ea815bfa27cc0d4d9a797" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1ad6a35329806ea815bfa27cc0d4d9a797"></a>

搜索用户

**Parameters**

* `name` 搜索的用户名
* `forceRefresh` 为true强制从服务器获取，为false情况下查询结果为空时自动从服务器获取。
* `callBack` [BMXErrorCode](broken-reference) 查询返回的用户的信息

#### `public inline void search(final` [`ListOfLongLong`](broken-reference)`rosterIdList,final boolean forceRefresh,final BMXDataCallBack<`[`BMXRosterItemList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1ae06ba55b12f71a3b70a6755abdaa513e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1ae06ba55b12f71a3b70a6755abdaa513e"></a>

批量搜索用户

**Parameters**

* `rosterIdList` 需要搜索的用户id列表
* `forceRefresh` 是否强制从服务器获取，为true则强制从服务器获取
* `callBack` [BMXErrorCode](broken-reference) 返回的好友信息列表

#### `public inline void setItemExtension(final` [`BMXRosterItem`](broken-reference) `item,final String extension,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1ae0569623bc916f57f99a1b10fbd2fc9d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1ae0569623bc916f57f99a1b10fbd2fc9d"></a>

更新好友本地扩展信息

**Parameters**

* `item` 用户信息
* `extension` 本地扩展信息
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setItemAlias(final` [`BMXRosterItem`](broken-reference) `item,final String alias,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1a246c40c23573cc3964f41e34c19e023f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1a246c40c23573cc3964f41e34c19e023f"></a>

更新好友别名

**Parameters**

* `item` 用户信息
* `alias` 好友别名
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setItemMuteNotification(final` [`BMXRosterItem`](broken-reference) `item,final boolean status,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1a0c4d39e20a157826c5e346454093d700" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1a0c4d39e20a157826c5e346454093d700"></a>

设置是否拒收用户消息

**Parameters**

* `item` 用户信息
* `status` 是否拒收用户消息，true拒收，false不拒收
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void apply(final long rosterId,final String message,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1afdda660daea4d2ac582ec750b341d539" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1afdda660daea4d2ac582ec750b341d539"></a>

申请添加好友

**Parameters**

* `rosterId` 申请添加的用户id
* `message` 好友申请信息
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void remove(final long rosterId,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1a81b9a440e71ca50f3a270cd2f3d389ab" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1a81b9a440e71ca50f3a270cd2f3d389ab"></a>

删除好友

**Parameters**

* `rosterId` 删除的好友id
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void getApplicationList(final String cursor,final int pageSize,final BMXDataCallBack<` [`ApplicationPage`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1aa525f2e2a002f940b6e6c8555f55c989" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1aa525f2e2a002f940b6e6c8555f55c989"></a>

获取申请添加好友列表

**Parameters**

* `cursor` 分页获取的起始cursor，第一次传入为空，后续传入上次操作返回的result中的cursor
* `pageSize` 分页大小
* `callBack` [BMXErrorCode](broken-reference) 返回的申请好友列表信息

#### `public inline void accept(final long rosterId,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1a7a996bb89b46a5ad236e48018afb394f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1a7a996bb89b46a5ad236e48018afb394f"></a>

接受加好友申请

**Parameters**

* `rosterId` 申请加为好友的用户id
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void decline(final long rosterId,final String reason,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1a0f923ce55b5795e64638d0e37938cc4c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1a0f923ce55b5795e64638d0e37938cc4c"></a>

拒绝加好友申请

**Parameters**

* `rosterId` 申请加为好友的用户id
* `reason` 拒绝的原因
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void block(final long rosterId,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1abebf32f1b38cc5249f8a8a6b5bfbb867" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1abebf32f1b38cc5249f8a8a6b5bfbb867"></a>

加入黑名单

**Parameters**

* `rosterId` 加入黑名单的用户id
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void unblock(final long rosterId,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1addb9d8f5014799ae79ecdbfcda3817d2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1addb9d8f5014799ae79ecdbfcda3817d2"></a>

从黑名单移除

**Parameters**

* `rosterId` 从黑名单移除的用户id
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void getBlockList(final boolean forceRefresh,final BMXDataCallBack<` [`ListOfLongLong`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1ae80fb718a40f46b3d33fda388924d170" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1ae80fb718a40f46b3d33fda388924d170"></a>

获取黑名单，如果forceRefresh == true，则强制从服务端拉取

**Parameters**

* `forceRefresh` 是否从服务器读取数据，true为强制从服务器获取，false情况下本地读取列表为空的情况下会自动从服务器读取
* `callBack` [BMXErrorCode](broken-reference) 好友id列表

#### `public inline void downloadAvatar(final` [`BMXRosterItem`](broken-reference)`item,final`[`FileProgressListener`](broken-reference) `listener,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1ab9f76853fe1acfe709654d81c7739d4e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1ab9f76853fe1acfe709654d81c7739d4e"></a>

下载头像

**Parameters**

* `item` 用户信息
* `listener` 下载回调函数
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void addRosterListener(`[`BMXRosterServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1a5b6e2a2ba80e347bf763e8741d65f68d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1a5b6e2a2ba80e347bf763e8741d65f68d"></a>

添加好友变化监听者

**Parameters**

* `listener` 好友变化监听者

#### `public inline void removeRosterListener(`[`BMXRosterServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1aacde16a51e3e531ff5392963e0444470" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_manager_1aacde16a51e3e531ff5392963e0444470"></a>

移除好友变化监听者

**Parameters**

* `listener` 好友变化监听者

## class `BMXRosterServiceApplicationList` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list"></a>

### Summary

| Members                                                                          | Descriptions |
| -------------------------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                                       |              |
| `public inline BMXRosterServiceApplicationList()`                                |              |
| `public inline BMXRosterServiceApplicationList(long n)`                          |              |
| `public inline long size()`                                                      |              |
| `public inline long capacity()`                                                  |              |
| `public inline void reserve(long n)`                                             |              |
| `public inline boolean isEmpty()`                                                |              |
| `public inline void clear()`                                                     |              |
| `public inline void add(BMXRosterService.Application x)`                         |              |
| `public inline BMXRosterService.Application get(int i)`                          |              |
| `public inline void set(int i,BMXRosterService.Application val)`                 |              |
| `protected transient boolean swigCMemOwn`                                        |              |
| `protected inline BMXRosterServiceApplicationList(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                                               |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1ab50270a6e8fdf0fa8fc17d4653ca7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1ab50270a6e8fdf0fa8fc17d4653ca7"></a>

#### `public inline BMXRosterServiceApplicationList()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1a2cd6bc7a2d469f2d9e709d9b1452d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1a2cd6bc7a2d469f2d9e709d9b1452d"></a>

#### `public inline BMXRosterServiceApplicationList(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1aee3c850a7010d2e26b9447dbb8d17" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1aee3c850a7010d2e26b9447dbb8d17"></a>

#### `public inline long size()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1a6f5b26197e039cf8ceb616b93dfdb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1a6f5b26197e039cf8ceb616b93dfdb"></a>

#### `public inline long capacity()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1a07cceaad249f464a7cf7c2bd5bc0e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1a07cceaad249f464a7cf7c2bd5bc0e"></a>

#### `public inline void reserve(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1a3d58c46949e234eeadcb97d6bfbc8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1a3d58c46949e234eeadcb97d6bfbc8"></a>

#### `public inline boolean isEmpty()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1aaa0a5317154bc78c3991fec8a888e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1aaa0a5317154bc78c3991fec8a888e"></a>

#### `public inline void clear()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1a669f78a1b022a2905041c89dbf1cd" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1a669f78a1b022a2905041c89dbf1cd"></a>

#### `public inline void add(BMXRosterService.Application x)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1ac3d9019194eb1eed220044087125f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1ac3d9019194eb1eed220044087125f"></a>

#### `public inline BMXRosterService.Application get(int i)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1a299ed6cd5191a43f8dad18e0dfff7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1a299ed6cd5191a43f8dad18e0dfff7"></a>

#### `public inline void set(int i,BMXRosterService.Application val)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1a37eb8aaba432f7a1541e3a8ebb550" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1a37eb8aaba432f7a1541e3a8ebb550"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1acea8e9504b58ab2a32a8f6d13b9b6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1acea8e9504b58ab2a32a8f6d13b9b6"></a>

#### `protected inline BMXRosterServiceApplicationList(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1ae5b5b50d8db6ee858fcda0f2ff3c3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1ae5b5b50d8db6ee858fcda0f2ff3c3"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1a38c259919a8cf9b70eeeae0272ef0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_application_list_1a38c259919a8cf9b70eeeae0272ef0"></a>

## class `BMXRosterServiceListener` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener"></a>

好友变化监听者

### Summary

| Members                                                                                      | Descriptions                                          |
| -------------------------------------------------------------------------------------------- | ----------------------------------------------------- |
| `public inline synchronized void delete()`                                                   |                                                       |
| `public inline void swigReleaseOwnership()`                                                  |                                                       |
| `public inline void swigTakeOwnership()`                                                     |                                                       |
| `public inline void onFriendAdded(long sponsorId,long recipientId)`                          | 添加好友                                                  |
| `public inline void onFriendRemoved(long sponsorId,long recipientId)`                        | 删除好友                                                  |
| `public inline void onApplied(long sponsorId,long recipientId,String message)`               | 收到加好友申请                                               |
| `public inline void onApplicationAccepted(long sponsorId,long recipientId)`                  | 加好友申请被通过了                                             |
| `public inline void onApplicationDeclined(long sponsorId,long recipientId,String reason)`    | 加好友申请被拒绝了                                             |
| `public inline void onBlockListAdded(long sponsorId,long recipientId)`                       | 添加黑名单                                                 |
| `public inline void onBlockListRemoved(long sponsorId,long recipientId)`                     | 删除黑名单                                                 |
| `public inline void onRosterInfoUpdate(`[`BMXRosterItem`](broken-reference) `item)`          | 用户信息更新                                                |
| `public inline void onRosterListUpdate()`                                                    | 客户端从服务器拉取到新联系人时触发，用于用户联系人列表更新，从SDK调用本地获取联系人即可取得全部成员信息 |
| `public inline BMXRosterServiceListener()`                                                   |                                                       |
| `public inline void registerRosterService(`[`BMXRosterService`](broken-reference) `service)` |                                                       |
| `protected transient boolean swigCMemOwn`                                                    |                                                       |
| `protected inline BMXRosterServiceListener(long cPtr,boolean cMemoryOwn)`                    |                                                       |
| `protected inline void finalize()`                                                           |                                                       |
| `protected inline void swigDirectorDisconnect()`                                             |                                                       |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a2ace5f49abbe479ce3cdadbfd728e68e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a2ace5f49abbe479ce3cdadbfd728e68e"></a>

#### `public inline void swigReleaseOwnership()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a971470027742d00b00a40f2314b4bada" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a971470027742d00b00a40f2314b4bada"></a>

#### `public inline void swigTakeOwnership()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a1198a723988b26c92b7b078ba9de07bc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a1198a723988b26c92b7b078ba9de07bc"></a>

#### `public inline void onFriendAdded(long sponsorId,long recipientId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a71686bcc8f047648eac5247a9b4ba29a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a71686bcc8f047648eac5247a9b4ba29a"></a>

添加好友

**Parameters**

* `sponsorId` 操作的发起者
* `recipientId` 操作的接受者

#### `public inline void onFriendRemoved(long sponsorId,long recipientId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a39ac214a1b1b3242ba671a34ded6ff00" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a39ac214a1b1b3242ba671a34ded6ff00"></a>

删除好友

**Parameters**

* `sponsorId` 操作的发起者
* `recipientId` 操作的接受者

#### `public inline void onApplied(long sponsorId,long recipientId,String message)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a37460e279719ca7da9346dea66d5e6b6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a37460e279719ca7da9346dea66d5e6b6"></a>

收到加好友申请

**Parameters**

* `sponsorId` 操作的发起者
* `recipientId` 操作的接受者
* `message` 好友申请消息

#### `public inline void onApplicationAccepted(long sponsorId,long recipientId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a58da903cc4ed4833c6818682af0ff312" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a58da903cc4ed4833c6818682af0ff312"></a>

加好友申请被通过了

**Parameters**

* `sponsorId` 操作的发起者
* `recipientId` 操作的接受者

#### `public inline void onApplicationDeclined(long sponsorId,long recipientId,String reason)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1ac4f0dfeb3f15268a1b28bbc5762b053c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1ac4f0dfeb3f15268a1b28bbc5762b053c"></a>

加好友申请被拒绝了

**Parameters**

* `sponsorId` 操作的发起者
* `recipientId` 操作的接受者
* `reason` 申请拒绝原因

#### `public inline void onBlockListAdded(long sponsorId,long recipientId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a99a5c934640f2501e91173b27db9cb7a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a99a5c934640f2501e91173b27db9cb7a"></a>

添加黑名单

**Parameters**

* `sponsorId` 操作的发起者
* `recipientId` 操作的接受者

#### `public inline void onBlockListRemoved(long sponsorId,long recipientId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a9ca94b3e271312e0fc929c1a2dffcf47" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a9ca94b3e271312e0fc929c1a2dffcf47"></a>

删除黑名单

**Parameters**

* `sponsorId` 操作的发起者
* `recipientId` 操作的接受者

#### `public inline void onRosterInfoUpdate(`[`BMXRosterItem`](broken-reference) `item)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a5a897b6e2645682532f4dc49801b6839" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a5a897b6e2645682532f4dc49801b6839"></a>

用户信息更新

**Parameters**

* `item` 更新的好友信息

#### `public inline void onRosterListUpdate()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a07c43140203e0cf2954308e43712a605" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a07c43140203e0cf2954308e43712a605"></a>

客户端从服务器拉取到新联系人时触发，用于用户联系人列表更新，从SDK调用本地获取联系人即可取得全部成员信息

#### `public inline BMXRosterServiceListener()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1adb84f2433ca67fdf7fab08ad732618e5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1adb84f2433ca67fdf7fab08ad732618e5"></a>

#### `public inline void registerRosterService(`[`BMXRosterService`](broken-reference) `service)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a94b7a648010c557c1b052e5915ab8798" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a94b7a648010c557c1b052e5915ab8798"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a9ffcc089e86b071926003052be99b5c2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a9ffcc089e86b071926003052be99b5c2"></a>

#### `protected inline BMXRosterServiceListener(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a394697d76b7871bf7c148c0e10487fd8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a394697d76b7871bf7c148c0e10487fd8"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a6801546d12bf410afe7fc59c3c875539" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a6801546d12bf410afe7fc59c3c875539"></a>

#### `protected inline void swigDirectorDisconnect()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a768b86aad0e8273ab97b3e26c72e2ac0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_roster_service_listener_1a768b86aad0e8273ab97b3e26c72e2ac0"></a>

## class `BMXSDKConfig` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config"></a>

SDK设置管理

### Summary

| Members                                                                                                                                                                                  | Descriptions |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| `class` [`HostConfig`](broken-reference)                                                                                                                                                 |              |
| `public inline synchronized void delete()`                                                                                                                                               |              |
| `public inline BMXSDKConfig(`[`BMXClientType`](broken-reference) `type,String vsn,String dataDir,String cacheDir,String pushCertName,boolean deliveryAck)`                               | 构造函数         |
| `public inline BMXSDKConfig(`[`BMXClientType`](broken-reference) `type,String vsn,String dataDir,String cacheDir,String pushCertName)`                                                   |              |
| `public inline BMXSDKConfig(`[`BMXClientType`](broken-reference) `type,String vsn,String dataDir,String cacheDir,String pushCertName,String appId,String appSecret,boolean deliveryAck)` |              |
| `public inline BMXSDKConfig(`[`BMXClientType`](broken-reference) `type,String vsn,String dataDir,String cacheDir,String pushCertName,String appId,String appSecret)`                     |              |
| `public inline String getDataDir()`                                                                                                                                                      |              |
| `public inline String getCacheDir()`                                                                                                                                                     |              |
| `public inline` [`BMXClientType`](broken-reference) `getClientType()`                                                                                                                    |              |
| `public inline String getVsn()`                                                                                                                                                          |              |
| `public inline String getSDKVersion()`                                                                                                                                                   |              |
| `public inline String getPushCertName()`                                                                                                                                                 |              |
| `public inline void setPushCertName(String arg0)`                                                                                                                                        |              |
| `public inline String getUserAgent()`                                                                                                                                                    |              |
| `public inline boolean carryUsernameInMessage()`                                                                                                                                         |              |
| `public inline void setCarryUsernameInMessage(boolean arg0)`                                                                                                                             |              |
| `public inline boolean enableDeliveryAck()`                                                                                                                                              |              |
| `public inline void setEnableDeliveryAck(boolean arg0)`                                                                                                                                  |              |
| `public inline` [`BMXLogLevel`](broken-reference) `getLogLevel()`                                                                                                                        |              |
| `public inline void setLogLevel(`[`BMXLogLevel`](broken-reference) `arg0)`                                                                                                               |              |
| `public inline boolean getConsoleOutput()`                                                                                                                                               |              |
| `public inline void setConsoleOutput(boolean arg0)`                                                                                                                                      |              |
| `public inline void setHostConfig(BMXSDKConfig.HostConfig config)`                                                                                                                       |              |
| `public inline BMXSDKConfig.HostConfig getHostConfig()`                                                                                                                                  |              |
| `public inline boolean getLoadAllServerConversations()`                                                                                                                                  |              |
| `public inline void setLoadAllServerConversations(boolean enable)`                                                                                                                       |              |
| `public inline void setLoadAllServerConversations()`                                                                                                                                     |              |
| `public inline String getDeviceUuid()`                                                                                                                                                   |              |
| `public inline void setDeviceUuid(String uuid)`                                                                                                                                          |              |
| `public inline String getDBCryptoKey()`                                                                                                                                                  |              |
| `public inline void setDBCryptoKey(String cryptoKey)`                                                                                                                                    |              |
| `public inline boolean getVerifyCertificate()`                                                                                                                                           |              |
| `public inline void setVerifyCertificate(boolean verify)`                                                                                                                                |              |
| `public inline void setVerifyCertificate()`                                                                                                                                              |              |
| `public inline boolean getEnableDNS()`                                                                                                                                                   |              |
| `public inline void setEnableDNS(boolean enable)`                                                                                                                                        |              |
| `public inline void setEnableDNS()`                                                                                                                                                      |              |
| `public inline String getUserDNSAddress()`                                                                                                                                               |              |
| `public inline void setUserDNSAddress(String dns)`                                                                                                                                       |              |
| `public inline String getAppID()`                                                                                                                                                        |              |
| `public inline void setAppID(String appID)`                                                                                                                                              |              |
| `public inline String getAppSecret()`                                                                                                                                                    |              |
| `public inline void setAppSecret(String appSecret)`                                                                                                                                      |              |
| `public inline` [`BMXPushProviderType`](broken-reference) `getPushProviderType()`                                                                                                        |              |
| `public inline void setPushProviderType(`[`BMXPushProviderType`](broken-reference) `type)`                                                                                               |              |
| `public inline` [`BMXPushEnvironmentType`](broken-reference) `getPushEnvironmentType()`                                                                                                  |              |
| `public inline void setEnvironmentType(`[`BMXPushEnvironmentType`](broken-reference) `type)`                                                                                             |              |
| `public inline long getDebugLogReceiverId()`                                                                                                                                             |              |
| `public inline void setDebugLogReceiverId(long uid)`                                                                                                                                     |              |
| `protected inline BMXSDKConfig(long cPtr,boolean cMemoryOwn)`                                                                                                                            |              |
| `protected inline void finalize()`                                                                                                                                                       |              |

### Members

#### `class` [`HostConfig`](broken-reference) <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config"></a>

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ab405fcae8fbe67fa5434b4ed1f381e2b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ab405fcae8fbe67fa5434b4ed1f381e2b"></a>

#### `public inline BMXSDKConfig(`[`BMXClientType`](broken-reference) `type,String vsn,String dataDir,String cacheDir,String pushCertName,boolean deliveryAck)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ade65e46e40f82bcadb78b7f7f4621e5b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ade65e46e40f82bcadb78b7f7f4621e5b"></a>

构造函数

**Parameters**

* `type` 客户端类型
* `vsn` 客户端OS版本
* `dataDir` 聊天数据存储路径
* `cacheDir` 缓存数据存储路径
* `pushCertName` Push证书名字
* `deliveryAck` 是否发送消息送达回执

#### `public inline BMXSDKConfig(`[`BMXClientType`](broken-reference) `type,String vsn,String dataDir,String cacheDir,String pushCertName)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a3ff284e06c355d693c7c2deb99e93797" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a3ff284e06c355d693c7c2deb99e93797"></a>

#### `public inline BMXSDKConfig(`[`BMXClientType`](broken-reference) `type,String vsn,String dataDir,String cacheDir,String pushCertName,String appId,String appSecret,boolean deliveryAck)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ac2225c76d1a30e0a796acf2c9451e817" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ac2225c76d1a30e0a796acf2c9451e817"></a>

#### `public inline BMXSDKConfig(`[`BMXClientType`](broken-reference) `type,String vsn,String dataDir,String cacheDir,String pushCertName,String appId,String appSecret)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a4d55bd9379c7eb6262d0245d483c658a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a4d55bd9379c7eb6262d0245d483c658a"></a>

#### `public inline String getDataDir()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a7bd47d2d8cd94ab753c23de0c6499774" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a7bd47d2d8cd94ab753c23de0c6499774"></a>

#### `public inline String getCacheDir()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1aa4cca1cd38ff149d59f5f1f9cc0a13ac" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1aa4cca1cd38ff149d59f5f1f9cc0a13ac"></a>

#### `public inline` [`BMXClientType`](broken-reference) `getClientType()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ac0730b34c7e71b87dd2b071eb6345c60" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ac0730b34c7e71b87dd2b071eb6345c60"></a>

#### `public inline String getVsn()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1aea57580a6fc4cb02be356ee2e95f1a7d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1aea57580a6fc4cb02be356ee2e95f1a7d"></a>

#### `public inline String getSDKVersion()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ab0b18ab20c269205b370b70ac7e7064d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ab0b18ab20c269205b370b70ac7e7064d"></a>

#### `public inline String getPushCertName()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ac29984dfd0d56e59872aa5bfaf4b631d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ac29984dfd0d56e59872aa5bfaf4b631d"></a>

#### `public inline void setPushCertName(String arg0)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a2932aa6e1c6f407196d866d44bed4ac3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a2932aa6e1c6f407196d866d44bed4ac3"></a>

#### `public inline String getUserAgent()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a08db1f634936a5071aaab04cddfc38eb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a08db1f634936a5071aaab04cddfc38eb"></a>

#### `public inline boolean carryUsernameInMessage()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a15cd7f08cd06321634c1a38d4676f1a3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a15cd7f08cd06321634c1a38d4676f1a3"></a>

#### `public inline void setCarryUsernameInMessage(boolean arg0)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a214a613c090d32ca52a715126e3ea84f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a214a613c090d32ca52a715126e3ea84f"></a>

#### `public inline boolean enableDeliveryAck()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a152b8b0ba03401538f330fa19da120d7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a152b8b0ba03401538f330fa19da120d7"></a>

#### `public inline void setEnableDeliveryAck(boolean arg0)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a9c0f9c7bb1dfd2c6d071a8453d22ab94" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a9c0f9c7bb1dfd2c6d071a8453d22ab94"></a>

#### `public inline` [`BMXLogLevel`](broken-reference) `getLogLevel()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a8dd84764179edb018878f88778fec7b8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a8dd84764179edb018878f88778fec7b8"></a>

#### `public inline void setLogLevel(`[`BMXLogLevel`](broken-reference) `arg0)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a79affa369f6c2caaed473d3efb6c585d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a79affa369f6c2caaed473d3efb6c585d"></a>

#### `public inline boolean getConsoleOutput()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a17f4595ae159830b703159524cc31cb1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a17f4595ae159830b703159524cc31cb1"></a>

#### `public inline void setConsoleOutput(boolean arg0)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ab5583dfc757a96f1bd1cd3be2f308071" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ab5583dfc757a96f1bd1cd3be2f308071"></a>

#### `public inline void setHostConfig(BMXSDKConfig.HostConfig config)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a12e03054009aa755ca3c477db49d61b5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a12e03054009aa755ca3c477db49d61b5"></a>

#### `public inline BMXSDKConfig.HostConfig getHostConfig()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a04bb061410b371d60d953aa78c602625" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a04bb061410b371d60d953aa78c602625"></a>

#### `public inline boolean getLoadAllServerConversations()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a7397452b8ffcc153b2379a8e36b213fc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a7397452b8ffcc153b2379a8e36b213fc"></a>

#### `public inline void setLoadAllServerConversations(boolean enable)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a85c75e803de359da1ce49311d7833c0c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a85c75e803de359da1ce49311d7833c0c"></a>

#### `public inline void setLoadAllServerConversations()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a45e795ab55efb6b1fa6fbd3c5b70560e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a45e795ab55efb6b1fa6fbd3c5b70560e"></a>

#### `public inline String getDeviceUuid()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a07bba65bdb4c7f7187efdef03ba827e1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a07bba65bdb4c7f7187efdef03ba827e1"></a>

#### `public inline void setDeviceUuid(String uuid)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a272bfbc1277da04f6496d0d21c883443" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a272bfbc1277da04f6496d0d21c883443"></a>

#### `public inline String getDBCryptoKey()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ab1519e82acceb76eb94bd00d10791c23" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ab1519e82acceb76eb94bd00d10791c23"></a>

#### `public inline void setDBCryptoKey(String cryptoKey)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a2b8e2a128b4dc3f09f9cb1c868e12f6b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a2b8e2a128b4dc3f09f9cb1c868e12f6b"></a>

#### `public inline boolean getVerifyCertificate()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1af0d929eb3feb3902da3b414527e9acaa" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1af0d929eb3feb3902da3b414527e9acaa"></a>

#### `public inline void setVerifyCertificate(boolean verify)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a9db9473e15a59ed2137e006425959564" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a9db9473e15a59ed2137e006425959564"></a>

#### `public inline void setVerifyCertificate()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a4aa2fb357acadf634b1591322ebf8449" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a4aa2fb357acadf634b1591322ebf8449"></a>

#### `public inline boolean getEnableDNS()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1aa1fc30d21350e44e0bd5f77df5a1589e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1aa1fc30d21350e44e0bd5f77df5a1589e"></a>

#### `public inline void setEnableDNS(boolean enable)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a5407f766c7f97f8ac15fa6779d0ea1ee" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a5407f766c7f97f8ac15fa6779d0ea1ee"></a>

#### `public inline void setEnableDNS()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1aeabac490bcffeab2de26b1d9cc57d597" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1aeabac490bcffeab2de26b1d9cc57d597"></a>

#### `public inline String getUserDNSAddress()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ac06d26d3c2d8ea01db127af2ec022562" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ac06d26d3c2d8ea01db127af2ec022562"></a>

#### `public inline void setUserDNSAddress(String dns)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a5c622e92adaea40dec2edb96f4a5e968" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a5c622e92adaea40dec2edb96f4a5e968"></a>

#### `public inline String getAppID()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a3f57383ab9dab469299c7ef1a097f180" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a3f57383ab9dab469299c7ef1a097f180"></a>

#### `public inline void setAppID(String appID)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a4280909b8e9d3e772b4e139d03e2bbed" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a4280909b8e9d3e772b4e139d03e2bbed"></a>

#### `public inline String getAppSecret()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ab2208178c97dc8d098b08c41fb154253" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ab2208178c97dc8d098b08c41fb154253"></a>

#### `public inline void setAppSecret(String appSecret)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ae9456467b70c5ac909a5a1d08cf8d076" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ae9456467b70c5ac909a5a1d08cf8d076"></a>

#### `public inline` [`BMXPushProviderType`](broken-reference) `getPushProviderType()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a11a12be9f43eb72b160465a1b792861f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a11a12be9f43eb72b160465a1b792861f"></a>

#### `public inline void setPushProviderType(`[`BMXPushProviderType`](broken-reference) `type)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1af6338616f20e9f9bcbf72d08a4c177e6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1af6338616f20e9f9bcbf72d08a4c177e6"></a>

#### `public inline` [`BMXPushEnvironmentType`](broken-reference) `getPushEnvironmentType()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a0b020c82927d8fe867a7276a06902566" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a0b020c82927d8fe867a7276a06902566"></a>

#### `public inline void setEnvironmentType(`[`BMXPushEnvironmentType`](broken-reference) `type)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ad7f94dcce9d23a6814b687141d1a5ffd" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ad7f94dcce9d23a6814b687141d1a5ffd"></a>

#### `public inline long getDebugLogReceiverId()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a78aa1d8281e28eec50fab19b2385ebbe" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a78aa1d8281e28eec50fab19b2385ebbe"></a>

#### `public inline void setDebugLogReceiverId(long uid)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a5c80aefc9860fa1f6cf7e448f9f60b0f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1a5c80aefc9860fa1f6cf7e448f9f60b0f"></a>

#### `protected inline BMXSDKConfig(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1acbc4a5dcbef1016535e6e78edbee1544" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1acbc4a5dcbef1016535e6e78edbee1544"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ab72904b3414fbb717356b1b7d2a74c8c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1ab72904b3414fbb717356b1b7d2a74c8c"></a>

## class `HostConfig` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config"></a>

### Summary

| Members                                                     | Descriptions |
| ----------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                  |              |
| `public inline HostConfig()`                                |              |
| `public inline HostConfig(String im,int port,String rest)`  | 服务设置         |
| `public inline void setImHost(String value)`                |              |
| `public inline String getImHost()`                          |              |
| `public inline void setImPort(int value)`                   |              |
| `public inline int getImPort()`                             |              |
| `public inline void setRestHost(String value)`              |              |
| `public inline String getRestHost()`                        |              |
| `protected transient boolean swigCMemOwn`                   |              |
| `protected inline HostConfig(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                          |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a70d6b298bc096056f5d821dfbe8dc407" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a70d6b298bc096056f5d821dfbe8dc407"></a>

#### `public inline HostConfig()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a789bd8b22ae25049d6add887611ca6eb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a789bd8b22ae25049d6add887611ca6eb"></a>

#### `public inline HostConfig(String im,int port,String rest)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a6b6988189b9abafaa2f3950687e45f7f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a6b6988189b9abafaa2f3950687e45f7f"></a>

服务设置

**Parameters**

* `im` IM服务器地址
* `port` IM服务器端口
* `rest` ratel服务器地址

#### `public inline void setImHost(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a2737d160c06e98023c57971197440f4e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a2737d160c06e98023c57971197440f4e"></a>

#### `public inline String getImHost()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a0e89bf0b56f7c80a2e219dcc6648036d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a0e89bf0b56f7c80a2e219dcc6648036d"></a>

#### `public inline void setImPort(int value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a74395828a65acf3a82328843f56a7e2f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a74395828a65acf3a82328843f56a7e2f"></a>

#### `public inline int getImPort()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a4285142c29b5505ccafabde6ee4fdf12" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a4285142c29b5505ccafabde6ee4fdf12"></a>

#### `public inline void setRestHost(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a9d4aafbddf7e48230773d442b94f5726" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a9d4aafbddf7e48230773d442b94f5726"></a>

#### `public inline String getRestHost()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a32b0c90d1c3833303421659e8f19d7dc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a32b0c90d1c3833303421659e8f19d7dc"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a62d917abe3aa276907529e7e0e650613" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a62d917abe3aa276907529e7e0e650613"></a>

#### `protected inline HostConfig(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a952eddce2773255eb50b340304e3de8b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a952eddce2773255eb50b340304e3de8b"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a18802092db33acc2fb7986ca2ee85ab7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_s_d_k_config_1_1_host_config_1a18802092db33acc2fb7986ca2ee85ab7"></a>

## class `BMXUserManager` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager"></a>

用户管理器

### Summary

| Members                                                                                                                                                                        | Descriptions   |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------- |
| `public inline BMXUserManager(`[`BMXUserService`](broken-reference) `service,`[`BMXClient`](broken-reference) `bmxClient)`                                                     |                |
| `public inline void signUpNewUser(final String username,final String password,final BMXDataCallBack<` [`BMXUserProfile`](broken-reference) `> callBack)`                       | 注册             |
| `public inline void signInByName(final String name,final String password,final BMXCallBack callBack)`                                                                          | 用户名登陆          |
| `public inline void signInById(final long id,final String password,final BMXCallBack callBack)`                                                                                | id 登陆          |
| `public inline void autoSignInByName(final String name,final String password,final BMXCallBack callBack)`                                                                      | 自动登陆 根据用户名     |
| `public inline void autoSignInById(final long uid,final String password,final BMXCallBack callBack)`                                                                           | 自动登陆 根据id      |
| `public inline void signOut(final BMXCallBack callBack)`                                                                                                                       | 退出登录           |
| `public inline void signOut(final long userId,final BMXCallBack callBack)`                                                                                                     | 退出登录           |
| `public inline` [`BMXConnectStatus`](broken-reference) `connectStatus()`                                                                                                       | 获取当前和服务器的连接状态  |
| `public inline` [`BMXSignInStatus`](broken-reference) `signInStatus()`                                                                                                         | 获取当前的登录状态      |
| `public inline void bindDevice(final String token,final BMXCallBack callBack)`                                                                                                 | 绑定设备推送token    |
| `public inline void getDeviceList(final BMXDataCallBack<` [`BMXDeviceList`](broken-reference) `> callBack)`                                                                    | 获取登录的设备列表      |
| `public inline void deleteDevice(final int device_sn,final BMXCallBack callBack)`                                                                                              | 删除设备           |
| `public inline void getProfile(final boolean forceRefresh,final BMXDataCallBack<` [`BMXUserProfile`](broken-reference) `> callBack)`                                           | 获取用户详情         |
| `public inline void setNickname(final String nickname,final BMXCallBack callBack)`                                                                                             | 设置昵称           |
| `public inline void uploadAvatar(final String avatarPath,final` [`FileProgressListener`](broken-reference) `listener,final BMXCallBack callBack)`                              | 上传头像           |
| `public inline void downloadAvatar(final` [`BMXUserProfile`](broken-reference)`profile,final`[`FileProgressListener`](broken-reference) `listener,final BMXCallBack callBack)` | 下载头像           |
| `public inline void setPublicInfo(final String publicInfo,final BMXCallBack callBack)`                                                                                         | 设置公开扩展信息       |
| `public inline void setPrivateInfo(final String privateInfo,final BMXCallBack callBack)`                                                                                       | 设置私有扩展信息       |
| `public inline void setAddFriendAuthMode(final BMXUserProfile.AddFriendAuthMode mode,final BMXCallBack callBack)`                                                              | 设置加好友验证方式      |
| `public inline void setAuthQuestion(final BMXUserProfile.AuthQuestion authQuestion,final BMXCallBack callBack)`                                                                | 设置加好友验证问题      |
| `public inline void setEnablePush(final boolean enable,final BMXCallBack callBack)`                                                                                            | 设置是否允许推送       |
| `public inline void setEnablePushDetaile(final boolean enable,final BMXCallBack callBack)`                                                                                     | 设置是否推送详情       |
| `public inline void setPushNickname(final String nickname,final BMXCallBack callBack)`                                                                                         | 设置推送昵称         |
| `public inline void setPushAlias(final String alias,final String bmxPushToken,final BMXCallBack callBack)`                                                                     | 设置推送别名         |
| `public inline void setNotificationSound(final boolean enable,final BMXCallBack callBack)`                                                                                     | 设置收到新消息是否声音提醒  |
| `public inline void setNotificationVibrate(final boolean enable,final BMXCallBack callBack)`                                                                                   | 设置收到新消息是否震动    |
| `public inline void setAutoDownloadAttachment(final boolean enable,final BMXCallBack callBack)`                                                                                | 设置是否自动缩略图和语音附件 |
| `public inline void setAutoAcceptGroupInvite(final boolean enable,final BMXCallBack callBack)`                                                                                 | 设置是否自动同意入群邀请   |
| `public inline void addUserListener(`[`BMXUserServiceListener`](broken-reference) `listener)`                                                                                  | 添加用户状态监听者      |
| `public inline void removeUserListener(`[`BMXUserServiceListener`](broken-reference) `listener)`                                                                               | 移除用户状态监听者      |
| `public inline void changeAppId(final String appId,final BMXCallBack callBack)`                                                                                                | 切换appId        |

### Members

#### `public inline BMXUserManager(`[`BMXUserService`](broken-reference) `service,`[`BMXClient`](broken-reference) `bmxClient)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a709be6259ccc5a299ea7ad0b67c33d82" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a709be6259ccc5a299ea7ad0b67c33d82"></a>

#### `public inline void signUpNewUser(final String username,final String password,final BMXDataCallBack<` [`BMXUserProfile`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a07d799d210bb314b509b42d52ac3e4b3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a07d799d210bb314b509b42d52ac3e4b3"></a>

注册

**Parameters**

* `password` 密码
* `username` 用户名
* `callBack` [BMXUserProfile](broken-reference)

#### `public inline void signInByName(final String name,final String password,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a31fb17814cefcd800085dc40e17aabc2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a31fb17814cefcd800085dc40e17aabc2"></a>

用户名登陆

**Parameters**

* `name`
* `password`
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void signInById(final long id,final String password,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1aed4decd37f69bb7432d038acb61c603f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1aed4decd37f69bb7432d038acb61c603f"></a>

id 登陆

**Parameters**

* `id`
* `password`
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void autoSignInByName(final String name,final String password,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1af6f603cd3dd03aa3c3387e723bc4777c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1af6f603cd3dd03aa3c3387e723bc4777c"></a>

自动登陆 根据用户名

**Parameters**

* `name`
* `password`
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void autoSignInById(final long uid,final String password,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a2afcb98d2b444565b4b0e17e86a392bb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a2afcb98d2b444565b4b0e17e86a392bb"></a>

自动登陆 根据id

**Parameters**

* `uid`
* `password`
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void signOut(final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a4658d67a1fcc89cbc4c06009bac209bd" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a4658d67a1fcc89cbc4c06009bac209bd"></a>

退出登录

**Parameters**

* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void signOut(final long userId,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a632f4b82f4834bcca92d68168e9c6871" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a632f4b82f4834bcca92d68168e9c6871"></a>

退出登录

**Parameters**

* `callBack` [BMXErrorCode](broken-reference)

#### `public inline` [`BMXConnectStatus`](broken-reference) `connectStatus()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1aa19aa6cb8b4b3dabc77f97d280d3a091" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1aa19aa6cb8b4b3dabc77f97d280d3a091"></a>

获取当前和服务器的连接状态

#### `public inline` [`BMXSignInStatus`](broken-reference) `signInStatus()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a6174c537d28df43d2db3beea3021dce0" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a6174c537d28df43d2db3beea3021dce0"></a>

获取当前的登录状态

#### `public inline void bindDevice(final String token,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a54822ed429818780022487bff3bc9a4e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a54822ed429818780022487bff3bc9a4e"></a>

绑定设备推送token

**Parameters**

* `token` device token
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void getDeviceList(final BMXDataCallBack<` [`BMXDeviceList`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a5eeb9fa24a33fce47f4743d47c742922" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a5eeb9fa24a33fce47f4743d47c742922"></a>

获取登录的设备列表

**Parameters**

* `callBack` [BMXErrorCode](broken-reference) 登录的设备列表

#### `public inline void deleteDevice(final int device_sn,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a1a51fb839f54e963e3a385cd1d19c5bf" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a1a51fb839f54e963e3a385cd1d19c5bf"></a>

删除设备

**Parameters**

* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void getProfile(final boolean forceRefresh,final BMXDataCallBack<` [`BMXUserProfile`](broken-reference) `> callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1ae42e16e738aa9366c667b2ad533d72c5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1ae42e16e738aa9366c667b2ad533d72c5"></a>

获取用户详情

**Parameters**

* `forceRefresh` 强制从服务器拉取最新结果
* `callBack` [BMXErrorCode](broken-reference),用户详情

#### `public inline void setNickname(final String nickname,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a1c63b52d974f10ef672228b0fa667182" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a1c63b52d974f10ef672228b0fa667182"></a>

设置昵称

**Parameters**

* `nickname` 昵称
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void uploadAvatar(final String avatarPath,final` [`FileProgressListener`](broken-reference) `listener,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a171e68997b2871baffe454dbcaef06cb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a171e68997b2871baffe454dbcaef06cb"></a>

上传头像

**Parameters**

* `avatarPath` 头像本地文件路径
* `listener` 上传进度监听器
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void downloadAvatar(final` [`BMXUserProfile`](broken-reference)`profile,final`[`FileProgressListener`](broken-reference) `listener,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1af5f771675332f3e13b15c59f585876d5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1af5f771675332f3e13b15c59f585876d5"></a>

下载头像

**Parameters**

* `profile` 用户详情
* `listener` 下载进度监听器
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setPublicInfo(final String publicInfo,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a9eed26e22bd77606d67b32371a46a11f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a9eed26e22bd77606d67b32371a46a11f"></a>

设置公开扩展信息

**Parameters**

* `publicInfo` 用户公开信息
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setPrivateInfo(final String privateInfo,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a71ef7760d5bb08098472aa91a33265fa" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a71ef7760d5bb08098472aa91a33265fa"></a>

设置私有扩展信息

**Parameters**

* `privateInfo` 用户私有信息（只对自己可见）
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setAddFriendAuthMode(final BMXUserProfile.AddFriendAuthMode mode,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a50974cbff43ffeb59d6cd84e004890ee" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a50974cbff43ffeb59d6cd84e004890ee"></a>

设置加好友验证方式

**Parameters**

* `mode` 添加好友时的验证方式
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setAuthQuestion(final BMXUserProfile.AuthQuestion authQuestion,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a6445fd3f347c4f05b40ce95e92a89cf5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a6445fd3f347c4f05b40ce95e92a89cf5"></a>

设置加好友验证问题

**Parameters**

* `authQuestion` 验证问题
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setEnablePush(final boolean enable,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a94f9c30bab6f8a9aa6c8d11514b97d0a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a94f9c30bab6f8a9aa6c8d11514b97d0a"></a>

设置是否允许推送

**Parameters**

* `enable` 是否允许推送，true推送，false不推送
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setEnablePushDetaile(final boolean enable,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a9403edcb901aebba331272b23014352a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a9403edcb901aebba331272b23014352a"></a>

设置是否推送详情

**Parameters**

* `enable` 是否推送详情，true推送，false不推送
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setPushNickname(final String nickname,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a98a3f8cb7bdfbe5073aa4d0d209ac6aa" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a98a3f8cb7bdfbe5073aa4d0d209ac6aa"></a>

设置推送昵称

**Parameters**

* `nickname` 推送昵称
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setPushAlias(final String alias,final String bmxPushToken,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a896c3aca24124649169124f8039b7040" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a896c3aca24124649169124f8039b7040"></a>

设置推送别名

**Parameters**

* `alias` 别名
* `bmxPushToken` 推送token
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setNotificationSound(final boolean enable,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1af661b00065e3c0ffd147f4a258eb9e37" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1af661b00065e3c0ffd147f4a258eb9e37"></a>

设置收到新消息是否声音提醒

**Parameters**

* `enable` 收到新消息是否声音提醒，true提醒，false不提醒
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setNotificationVibrate(final boolean enable,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a004a289c4eed58134c927e1e9f0834e7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a004a289c4eed58134c927e1e9f0834e7"></a>

设置收到新消息是否震动

**Parameters**

* `enable` 收到新消息是否震动，true震动，false不震动
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setAutoDownloadAttachment(final boolean enable,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a2e1dab1e45bd5c1f8af3317d24e089a1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a2e1dab1e45bd5c1f8af3317d24e089a1"></a>

设置是否自动缩略图和语音附件

**Parameters**

* `enable` 是否自动缩略图和语音附件，true自动下载，false不会自动下载
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void setAutoAcceptGroupInvite(final boolean enable,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a7db600e243ee79291e845ce967339128" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a7db600e243ee79291e845ce967339128"></a>

设置是否自动同意入群邀请

**Parameters**

* `enable` 是否自动同意入群邀请，true同意，false不同意
* `callBack` [BMXErrorCode](broken-reference)

#### `public inline void addUserListener(`[`BMXUserServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a8e3d22a6fd26075089cfa463543ea4c1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a8e3d22a6fd26075089cfa463543ea4c1"></a>

添加用户状态监听者

**Parameters**

* `listener` 用户状态监听者

#### `public inline void removeUserListener(`[`BMXUserServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1ae0c681a51af6302f5a2d57101ba71584" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1ae0c681a51af6302f5a2d57101ba71584"></a>

移除用户状态监听者

**Parameters**

* `listener` 用户状态监听者

#### `public inline void changeAppId(final String appId,final BMXCallBack callBack)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a177d31a6a9360006f7dfe33576549b38" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_manager_1a177d31a6a9360006f7dfe33576549b38"></a>

切换appId

**Parameters**

* `appId` appId

## class `BMXUserService` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service"></a>

用户Service

### Summary

| Members                                                                                                                                                                                     | Descriptions                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------- |
| `public inline synchronized void delete()`                                                                                                                                                  |                                         |
| `public inline` [`BMXErrorCode`](broken-reference) `bindDevice(String token)`                                                                                                               | 绑定设备推送token                             |
| `public inline` [`BMXErrorCode`](broken-reference) `getDeviceList(`[`BMXDeviceList`](broken-reference) `deviceList)`                                                                        | 获取设备列表                                  |
| `public inline` [`BMXErrorCode`](broken-reference) `getProfile(`[`BMXUserProfile`](broken-reference) `profile,boolean forceRefresh)`                                                        | 获取用户详情，如果forceRefresh == true，则强制从服务端拉取 |
| `public inline` [`BMXErrorCode`](broken-reference) `deleteDevice(int device_sn)`                                                                                                            | 删除设备                                    |
| `public inline` [`BMXErrorCode`](broken-reference) `setNickname(String nickname)`                                                                                                           | 设置昵称                                    |
| `public inline` [`BMXErrorCode`](broken-reference) `uploadAvatar(String avatarPath,`[`FileProgressListener`](broken-reference) `callback)`                                                  | 上传头像                                    |
| `public inline` [`BMXErrorCode`](broken-reference) `downloadAvatar(`[`BMXUserProfile`](broken-reference) `profile,boolean thumbnail,`[`FileProgressListener`](broken-reference) `callback)` | 下载头像，默认下载缩略图                            |
| `public inline` [`BMXErrorCode`](broken-reference) `setPublicInfo(String publicInfo)`                                                                                                       | 设置公开扩展信息                                |
| `public inline` [`BMXErrorCode`](broken-reference) `setPrivateInfo(String privateInfo)`                                                                                                     | 设置私有扩展信息                                |
| `public inline` [`BMXErrorCode`](broken-reference) `setAddFriendAuthMode(BMXUserProfile.AddFriendAuthMode mode)`                                                                            | 设置加好友验证方式                               |
| `public inline` [`BMXErrorCode`](broken-reference) `setAuthQuestion(BMXUserProfile.AuthQuestion authQuestion)`                                                                              | 设置加好友验证问题                               |
| `public inline` [`BMXErrorCode`](broken-reference) `setEnablePush(boolean enable)`                                                                                                          | 设置是否允许推送                                |
| `public inline` [`BMXErrorCode`](broken-reference) `setEnablePushDetaile(boolean enable)`                                                                                                   | 设置是否推送详情                                |
| `public inline` [`BMXErrorCode`](broken-reference) `setPushNickname(String nickname)`                                                                                                       | 设置推送昵称                                  |
| `public inline` [`BMXErrorCode`](broken-reference) `setPushAlias(String alias,String bmxPushToken)`                                                                                         | 设置推送别名                                  |
| `public inline` [`BMXErrorCode`](broken-reference) `setNotificationSound(boolean enable)`                                                                                                   | 设置收到新消息是否声音提醒                           |
| `public inline` [`BMXErrorCode`](broken-reference) `setNotificationVibrate(boolean enable)`                                                                                                 | 设置收到新消息是否震动                             |
| `public inline` [`BMXErrorCode`](broken-reference) `setAutoDownloadAttachment(boolean enable)`                                                                                              | 设置是否自动缩略图和语音附件                          |
| `public inline` [`BMXErrorCode`](broken-reference) `setAutoAcceptGroupInvite(boolean enable)`                                                                                               | 设置是否自动同意入群邀请                            |
| `public inline void addUserListener(`[`BMXUserServiceListener`](broken-reference) `listener)`                                                                                               | 添加用户状态监听者                               |
| `public inline void removeUserListener(`[`BMXUserServiceListener`](broken-reference) `listener)`                                                                                            | 移除用户状态监听者                               |
| `protected transient boolean swigCMemOwn`                                                                                                                                                   |                                         |
| `protected inline BMXUserService(long cPtr,boolean cMemoryOwn)`                                                                                                                             |                                         |
| `protected inline void finalize()`                                                                                                                                                          |                                         |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a931252ee065703d7561107433ed79f30" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a931252ee065703d7561107433ed79f30"></a>

#### `public inline` [`BMXErrorCode`](broken-reference) `bindDevice(String token)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1ace02ea6fd7a9669b3fa285455c927654" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1ace02ea6fd7a9669b3fa285455c927654"></a>

绑定设备推送token

**Parameters**

* `token` 设备token

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getDeviceList(`[`BMXDeviceList`](broken-reference) `deviceList)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1adb8f3ec72b6df3d764e4de29c545c2ba" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1adb8f3ec72b6df3d764e4de29c545c2ba"></a>

获取设备列表

**Parameters**

* `deviceList` 设备列表，传入空列表函数返回后从此处获取返回的设备列表

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `getProfile(`[`BMXUserProfile`](broken-reference) `profile,boolean forceRefresh)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a326eb22b22fbaaff57db25d2244e5b15" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a326eb22b22fbaaff57db25d2244e5b15"></a>

获取用户详情，如果forceRefresh == true，则强制从服务端拉取

**Parameters**

* `profile` 用户profile信息，初始传入指向为空的shared\_ptr对象，函数返回后从此处获取用户profile信息。
* `forceRefresh` 是否强制从服务器拉取，本地获取失败的情况下会自动从服务器拉取

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `deleteDevice(int device_sn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1ab3da60e3e86349208baf626278d735db" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1ab3da60e3e86349208baf626278d735db"></a>

删除设备

**Parameters**

* `device_sn` 设备序列号

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setNickname(String nickname)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a6bd3e3f98b19af8be9a6d34844c4c397" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a6bd3e3f98b19af8be9a6d34844c4c397"></a>

设置昵称

**Parameters**

* `nickname` 用户昵称

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `uploadAvatar(String avatarPath,`[`FileProgressListener`](broken-reference) `callback)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a2ee0e79052c29443c7460a7a6bd79b16" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a2ee0e79052c29443c7460a7a6bd79b16"></a>

上传头像

**Parameters**

* `avatarPath` 上传头像的本地地址
* `callback` 上传回调函数

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `downloadAvatar(`[`BMXUserProfile`](broken-reference) `profile,boolean thumbnail,`[`FileProgressListener`](broken-reference) `callback)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a939e92566ca4ff6ba589839e8cdd1af9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a939e92566ca4ff6ba589839e8cdd1af9"></a>

下载头像，默认下载缩略图

**Parameters**

* `profile` 用户profile
* `thumbnail` 是否下载缩略图，true下载缩略图，false下载原图
* `callback` 下载回调函数

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setPublicInfo(String publicInfo)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a32e57e54bd1639fecae02f5d28ca8f3e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a32e57e54bd1639fecae02f5d28ca8f3e"></a>

设置公开扩展信息

**Parameters**

* `publicInfo` 公开扩展信息

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setPrivateInfo(String privateInfo)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a0f6931025048c9565e3863d5b191005e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a0f6931025048c9565e3863d5b191005e"></a>

设置私有扩展信息

**Parameters**

* `privateInfo` 私有扩展信息

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setAddFriendAuthMode(BMXUserProfile.AddFriendAuthMode mode)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a330529da50ed7f7ef4ce38c58aee3ba7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a330529da50ed7f7ef4ce38c58aee3ba7"></a>

设置加好友验证方式

**Parameters**

* `mode` 加好友验证方式

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setAuthQuestion(BMXUserProfile.AuthQuestion authQuestion)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a39af52ac8baaee42d2a106da5438ae31" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a39af52ac8baaee42d2a106da5438ae31"></a>

设置加好友验证问题

**Parameters**

* `authQuestion` 加好友验证问题

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setEnablePush(boolean enable)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1ab92d45a6b5a56b6d8e9abf2cf45acc38" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1ab92d45a6b5a56b6d8e9abf2cf45acc38"></a>

设置是否允许推送

**Parameters**

* `enable` 是否允许推送，true推送，false不推送

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setEnablePushDetaile(boolean enable)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1acc4e1a16c8e6549473bfe5cb1bb40c19" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1acc4e1a16c8e6549473bfe5cb1bb40c19"></a>

设置是否推送详情

**Parameters**

* `enable` 是否推送详情，true推送，false不推送

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setPushNickname(String nickname)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a004d1959bdc57db3ccf55f8bf7df3850" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a004d1959bdc57db3ccf55f8bf7df3850"></a>

设置推送昵称

**Parameters**

* `nickname` 推送昵称

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setPushAlias(String alias,String bmxPushToken)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1af9ee09821305bb5128847ab395862cb5" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1af9ee09821305bb5128847ab395862cb5"></a>

设置推送别名

**Parameters**

* `alias` 别名
* `bmxPushToken` 推送token

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setNotificationSound(boolean enable)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1ad1a578ba37fe0bbc46a7fa04f15a5fbb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1ad1a578ba37fe0bbc46a7fa04f15a5fbb"></a>

设置收到新消息是否声音提醒

**Parameters**

* `enable` 收到新消息是否声音提醒，true提醒，false不提醒

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setNotificationVibrate(boolean enable)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a98717a7e5746e5b83ddab7b9b8e1f833" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a98717a7e5746e5b83ddab7b9b8e1f833"></a>

设置收到新消息是否震动

**Parameters**

* `enable` 收到新消息是否震动，true震动，false不震动

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setAutoDownloadAttachment(boolean enable)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a11698d30f02d61968a2aee9eaf46a1d6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a11698d30f02d61968a2aee9eaf46a1d6"></a>

设置是否自动缩略图和语音附件

**Parameters**

* `enable` 是否自动缩略图和语音附件，true自动下载，false不会自动下载

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline` [`BMXErrorCode`](broken-reference) `setAutoAcceptGroupInvite(boolean enable)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a931cb74c45e66414feedf7249c84ba4b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a931cb74c45e66414feedf7249c84ba4b"></a>

设置是否自动同意入群邀请

**Parameters**

* `enable` 是否自动同意入群邀请，true同意，false不同意

**Returns**

[BMXErrorCode](broken-reference)

#### `public inline void addUserListener(`[`BMXUserServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1ad37e92f01ee2200d568915d3e81e4f04" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1ad37e92f01ee2200d568915d3e81e4f04"></a>

添加用户状态监听者

**Parameters**

* `listener` 用户状态监听者

#### `public inline void removeUserListener(`[`BMXUserServiceListener`](broken-reference) `listener)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a001c27eb80914234061b2b6b339d5638" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a001c27eb80914234061b2b6b339d5638"></a>

移除用户状态监听者

**Parameters**

* `listener` 用户状态监听者

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1adc122f6160e0a0b850c41d0fcecf6cb2" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1adc122f6160e0a0b850c41d0fcecf6cb2"></a>

#### `protected inline BMXUserService(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1add284c873c9431375751feb2306ece04" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1add284c873c9431375751feb2306ece04"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a256204d711396765b4c76940b46614fb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_1a256204d711396765b4c76940b46614fb"></a>

## class `BMXUserServiceListener` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener"></a>

用户状态监听者

### Summary

| Members                                                                                      | Descriptions             |
| -------------------------------------------------------------------------------------------- | ------------------------ |
| `public inline synchronized void delete()`                                                   |                          |
| `public inline void swigReleaseOwnership()`                                                  |                          |
| `public inline void swigTakeOwnership()`                                                     |                          |
| `public inline void onConnectStatusChanged(`[`BMXConnectStatus`](broken-reference) `status)` | 链接状态发生变化                 |
| `public inline void onUserSignIn(`[`BMXUserProfile`](broken-reference) `profile)`            | 用户登陆                     |
| `public inline void onUserSignOut(`[`BMXErrorCode`](broken-reference) `error,long userId)`   | 用户登出                     |
| `public inline void onInfoUpdated(`[`BMXUserProfile`](broken-reference) `profile)`           | 同步用户信息更新（其他设备操作发生用户信息变更） |
| `public inline void onOtherDeviceSingIn(int deviceSN)`                                       | 用户在其他设备上登陆               |
| `public inline void onOtherDeviceSingOut(int deviceSN)`                                      | 用户在其他设备上登出               |
| `public inline BMXUserServiceListener()`                                                     |                          |
| `public inline void registerUserService(`[`BMXUserService`](broken-reference) `service)`     |                          |
| `protected transient boolean swigCMemOwn`                                                    |                          |
| `protected inline BMXUserServiceListener(long cPtr,boolean cMemoryOwn)`                      |                          |
| `protected inline void finalize()`                                                           |                          |
| `protected inline void swigDirectorDisconnect()`                                             |                          |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a3016de529913e4d8e17ae26b6e419665" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a3016de529913e4d8e17ae26b6e419665"></a>

#### `public inline void swigReleaseOwnership()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a04d4b8c62bb6461bf79e1fb77ed14e68" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a04d4b8c62bb6461bf79e1fb77ed14e68"></a>

#### `public inline void swigTakeOwnership()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a7f28db05563caff786766d8df741087c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a7f28db05563caff786766d8df741087c"></a>

#### `public inline void onConnectStatusChanged(`[`BMXConnectStatus`](broken-reference) `status)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a829963367ece1e404f4d84b5ab15442e" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a829963367ece1e404f4d84b5ab15442e"></a>

链接状态发生变化

**Parameters**

* `status` 连接状态

#### `public inline void onUserSignIn(`[`BMXUserProfile`](broken-reference) `profile)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a8ccc54104c7bb2b33174fb0e5a556666" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a8ccc54104c7bb2b33174fb0e5a556666"></a>

用户登陆

**Parameters**

* `profile` 用户profile

#### `public inline void onUserSignOut(`[`BMXErrorCode`](broken-reference) `error,long userId)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a72ec5b4051a30a19fcc185e37f5547c8" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a72ec5b4051a30a19fcc185e37f5547c8"></a>

用户登出

**Parameters**

* `error` 状态错误码

#### `public inline void onInfoUpdated(`[`BMXUserProfile`](broken-reference) `profile)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a6d18b37c16988b0603bbbdc68ec7da39" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a6d18b37c16988b0603bbbdc68ec7da39"></a>

同步用户信息更新（其他设备操作发生用户信息变更）

**Parameters**

* `profile` 用户profile

#### `public inline void onOtherDeviceSingIn(int deviceSN)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1afe26623532ecb57ef7ef2d6374ad1fc9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1afe26623532ecb57ef7ef2d6374ad1fc9"></a>

用户在其他设备上登陆

**Parameters**

* `deviceSN` 设备序列号

#### `public inline void onOtherDeviceSingOut(int deviceSN)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1afc4957f2a9958340bd6e231dd8b41698" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1afc4957f2a9958340bd6e231dd8b41698"></a>

用户在其他设备上登出

**Parameters**

* `deviceSN` 设备序列号

#### `public inline BMXUserServiceListener()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a0e14acd0047f6f52e22973fe8ca25761" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a0e14acd0047f6f52e22973fe8ca25761"></a>

#### `public inline void registerUserService(`[`BMXUserService`](broken-reference) `service)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a1b967c6b5ec0b5fecc15cb7124633dc6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a1b967c6b5ec0b5fecc15cb7124633dc6"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a7ab9eaac2d67685f67c79199b3a5c686" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a7ab9eaac2d67685f67c79199b3a5c686"></a>

#### `protected inline BMXUserServiceListener(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1aa0dae059f17e8f4240e0c522dd33a1b3" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1aa0dae059f17e8f4240e0c522dd33a1b3"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a9f6658160d4f2e60c19f0e4b98d0c8b7" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a9f6658160d4f2e60c19f0e4b98d0c8b7"></a>

#### `protected inline void swigDirectorDisconnect()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a8fe5225769f5e3d9261c1767723c778a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_user_service_listener_1a8fe5225769f5e3d9261c1767723c778a"></a>

## class `BMXVideoAttachment` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment"></a>

```
class BMXVideoAttachment
  : public im.floo.floolib.BMXFileAttachment
```

视频消息附件

### Summary

| Members                                                                                                                                                | Descriptions    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------- |
| `public inline synchronized void delete()`                                                                                                             |                 |
| `public inline BMXVideoAttachment(String path,int duration,BMXMessageAttachment.Size size,String displayName)`                                         | 构造函数，构建发送视频消息附件 |
| `public inline BMXVideoAttachment(String path,int duration,BMXMessageAttachment.Size size)`                                                            |                 |
| `public inline BMXVideoAttachment(String path,String thumbnailPath,int duration,BMXMessageAttachment.Size size,String displayName)`                    | 构造函数，构建发送视频消息附件 |
| `public inline BMXVideoAttachment(String path,String thumbnailPath,int duration,BMXMessageAttachment.Size size)`                                       |                 |
| `public inline BMXVideoAttachment(String ratelUrl,int duration,BMXMessageAttachment.Size size,String displayName,long fileLength)`                     | 构造函数，构建接收视频消息附件 |
| `public inline BMXVideoAttachment(String ratelUrl,String thumbnailUrl,int duration,BMXMessageAttachment.Size size,String displayName,long fileLength)` | 构造函数，构建接收视频消息附件 |
| `public inline BMXMessageAttachment.Type type()`                                                                                                       | 返回文件类型          |
| `public inline` [`BMXMessageAttachment`](broken-reference) `clone()`                                                                                   | 克隆函数            |
| `public inline BMXMessageAttachment.Size size()`                                                                                                       | 视频大小，宽度和高度      |
| `public inline int duration()`                                                                                                                         | 视频片段时长          |
| `public inline void setThumbnail(String path)`                                                                                                         | 设置发送视频片段消息缩略图   |
| `public inline String thumbnailPath()`                                                                                                                 | 缩略图本地路径         |
| `public inline String thumbnailUrl()`                                                                                                                  | 缩略图服务器路径        |
| `public inline void setThumbnailRatelUrl(String thumbnailRatelUrl)`                                                                                    |                 |
| `public inline String thumbnailRatelUrl()`                                                                                                             |                 |
| `public inline BMXMessageAttachment.DownloadStatus thumbnailDownloadStatus()`                                                                          | 缩略图下载状态         |
| `protected inline BMXVideoAttachment(long cPtr,boolean cMemoryOwn)`                                                                                    |                 |
| `protected inline void finalize()`                                                                                                                     |                 |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1a494260699385490af142a7776ccc1e49" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1a494260699385490af142a7776ccc1e49"></a>

#### `public inline BMXVideoAttachment(String path,int duration,BMXMessageAttachment.Size size,String displayName)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1a20cf51f5640be8e16ed9e2622865cce1" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1a20cf51f5640be8e16ed9e2622865cce1"></a>

构造函数，构建发送视频消息附件

**Parameters**

* `path` 文件的本地路径
* `duration` 视频片段时长
* `size` 视频大小，宽度和高度
* `displayName` 文件展示名

#### `public inline BMXVideoAttachment(String path,int duration,BMXMessageAttachment.Size size)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1a969f575f23da5359ccda9cef68aa03f9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1a969f575f23da5359ccda9cef68aa03f9"></a>

#### `public inline BMXVideoAttachment(String path,String thumbnailPath,int duration,BMXMessageAttachment.Size size,String displayName)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1a7a1101e54c55d6683a29bba233fcee63" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1a7a1101e54c55d6683a29bba233fcee63"></a>

构造函数，构建发送视频消息附件

**Parameters**

* `path` 文件的本地路径
* `thumbnailPath` 缩略图文件的本地路径
* `duration` 视频片段时长
* `size` 视频大小，宽度和高度
* `displayName` 文件展示名

#### `public inline BMXVideoAttachment(String path,String thumbnailPath,int duration,BMXMessageAttachment.Size size)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1af87b9d4bda6da1d0264a4a0c07cf2a2b" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1af87b9d4bda6da1d0264a4a0c07cf2a2b"></a>

#### `public inline BMXVideoAttachment(String ratelUrl,int duration,BMXMessageAttachment.Size size,String displayName,long fileLength)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1ac46e353e67a48ec1ad3176bb2c61ab9d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1ac46e353e67a48ec1ad3176bb2c61ab9d"></a>

构造函数，构建接收视频消息附件

**Parameters**

* `ratelUrl` ratel服务器地址
* `duration` 视频片段时长
* `size` 视频大小，宽度和高度
* `displayName` 文件展示名
* `fileLength` 文件大小

#### `public inline BMXVideoAttachment(String ratelUrl,String thumbnailUrl,int duration,BMXMessageAttachment.Size size,String displayName,long fileLength)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1a5dc46493057dc6677ad9c218ff99a2cf" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1a5dc46493057dc6677ad9c218ff99a2cf"></a>

构造函数，构建接收视频消息附件

**Parameters**

* `ratelUrl` ratel服务器地址
* `thumbnailUrl` 缩略图文件服务器地址
* `duration` 视频片段时长
* `size` 视频大小，宽度和高度
* `displayName` 文件展示名
* `fileLength` 文件大小

#### `public inline BMXMessageAttachment.Type type()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1abc8ea789bb1e5e1d5722fd23dba08efb" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1abc8ea789bb1e5e1d5722fd23dba08efb"></a>

返回文件类型

**Returns**

Type

#### `public inline` [`BMXMessageAttachment`](broken-reference) `clone()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1a7a432322e3618ed78cfea7696d189f27" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1a7a432322e3618ed78cfea7696d189f27"></a>

克隆函数

**Returns**

BMXMessageAttachmentPtr

#### `public inline BMXMessageAttachment.Size size()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1af3f40dff3dbd0526a65c23aabada7d3d" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1af3f40dff3dbd0526a65c23aabada7d3d"></a>

视频大小，宽度和高度

**Returns**

Size

#### `public inline int duration()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1ac1e249725e554ab6ccdf0ec898cc3abd" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1ac1e249725e554ab6ccdf0ec898cc3abd"></a>

视频片段时长

**Returns**

int32\_t

#### `public inline void setThumbnail(String path)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1af44539a2f15aa51766955861a75d4e35" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1af44539a2f15aa51766955861a75d4e35"></a>

设置发送视频片段消息缩略图

**Parameters**

* `path` 视频片段消息缩略图

#### `public inline String thumbnailPath()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1aa39209e8dc63f76a99e6d9d722e2b190" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1aa39209e8dc63f76a99e6d9d722e2b190"></a>

缩略图本地路径

**Returns**

std::string

#### `public inline String thumbnailUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1ad92a829ee3ac275d517babb165219258" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1ad92a829ee3ac275d517babb165219258"></a>

缩略图服务器路径

**Returns**

std::string

#### `public inline void setThumbnailRatelUrl(String thumbnailRatelUrl)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1a9b4a352c0f7009d3892dd0d8675917bc" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1a9b4a352c0f7009d3892dd0d8675917bc"></a>

#### `public inline String thumbnailRatelUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1aedeb916bc6abe20b1f61faab11602d98" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1aedeb916bc6abe20b1f61faab11602d98"></a>

#### `public inline BMXMessageAttachment.DownloadStatus thumbnailDownloadStatus()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1af8d702c6c7b93086c7f87767f54450ff" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1af8d702c6c7b93086c7f87767f54450ff"></a>

缩略图下载状态

**Returns**

DownloadStatus

#### `protected inline BMXVideoAttachment(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1aade1d12f548d0b0e26b1e1372d358cc4" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1aade1d12f548d0b0e26b1e1372d358cc4"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1a96cd9e6fcb5e6e5ee9f79eb55e8ec7d9" id="classim_1_1floo_1_1floolib_1_1_b_m_x_video_attachment_1a96cd9e6fcb5e6e5ee9f79eb55e8ec7d9"></a>

## class `BMXVoiceAttachment` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment" id="classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment"></a>

```
class BMXVoiceAttachment
  : public im.floo.floolib.BMXFileAttachment
```

音频消息附件

### Summary

| Members                                                                                             | Descriptions    |
| --------------------------------------------------------------------------------------------------- | --------------- |
| `public inline synchronized void delete()`                                                          |                 |
| `public inline BMXVoiceAttachment(String path,int duration,String displayName)`                     | 构造函数，构建发送音频消息附件 |
| `public inline BMXVoiceAttachment(String path,int duration)`                                        |                 |
| `public inline BMXVoiceAttachment(String ratelUrl,int duration,String displayName,long fileLength)` | 构造函数，构建接收音频消息附件 |
| `public inline BMXMessageAttachment.Type type()`                                                    | 返回文件类型          |
| `public inline` [`BMXMessageAttachment`](broken-reference) `clone()`                                | 克隆函数            |
| `public inline int duration()`                                                                      | 语音时长            |
| `protected inline BMXVoiceAttachment(long cPtr,boolean cMemoryOwn)`                                 |                 |
| `protected inline void finalize()`                                                                  |                 |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1af561ef7d3d0f38283de017e784b735b6" id="classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1af561ef7d3d0f38283de017e784b735b6"></a>

#### `public inline BMXVoiceAttachment(String path,int duration,String displayName)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1a48052d8bca3a059f6610afb091482d04" id="classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1a48052d8bca3a059f6610afb091482d04"></a>

构造函数，构建发送音频消息附件

**Parameters**

* `path` 文件的本地路径
* `duration` 音频时长
* `displayName` 文件展示名

#### `public inline BMXVoiceAttachment(String path,int duration)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1aee5fbb26b34bc7b4b6e1610131a8ed8a" id="classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1aee5fbb26b34bc7b4b6e1610131a8ed8a"></a>

#### `public inline BMXVoiceAttachment(String ratelUrl,int duration,String displayName,long fileLength)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1a9f8852c265444ceef956ce7b15348593" id="classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1a9f8852c265444ceef956ce7b15348593"></a>

构造函数，构建接收音频消息附件

**Parameters**

* `ratelUrl` ratel服务器地址
* `duration` 音频时长
* `displayName` 文件展示名
* `fileLength` 文件大小

#### `public inline BMXMessageAttachment.Type type()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1ae6a344cfe228a81bd0f8ef8b97b5b31c" id="classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1ae6a344cfe228a81bd0f8ef8b97b5b31c"></a>

返回文件类型

**Returns**

Type

#### `public inline` [`BMXMessageAttachment`](broken-reference) `clone()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1aeece1b44253bc121288d0f25401ce668" id="classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1aeece1b44253bc121288d0f25401ce668"></a>

克隆函数

**Returns**

BMXMessageAttachmentPtr

#### `public inline int duration()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1a99328f22003c90257d4263b29a5a0833" id="classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1a99328f22003c90257d4263b29a5a0833"></a>

语音时长

**Returns**

int32\_t

#### `protected inline BMXVoiceAttachment(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1a2175aa4371f8f62e3e42940d4de38f7f" id="classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1a2175aa4371f8f62e3e42940d4de38f7f"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1a94491c5bd9faac1968a770ad3fdefd77" id="classim_1_1floo_1_1floolib_1_1_b_m_x_voice_attachment_1a94491c5bd9faac1968a770ad3fdefd77"></a>

## class `floo` <a href="#classim_1_1floo_1_1floolib_1_1floo" id="classim_1_1floo_1_1floolib_1_1floo"></a>

```
class floo
  : public im.floo.floolib.flooConstants
```

### Summary

### Members

## class `flooJNI` <a href="#classim_1_1floo_1_1floolib_1_1floo_j_n_i" id="classim_1_1floo_1_1floolib_1_1floo_j_n_i"></a>

### Summary

### Members

## class `GroupApplicationPage` <a href="#classim_1_1floo_1_1floolib_1_1_group_application_page" id="classim_1_1floo_1_1floolib_1_1_group_application_page"></a>

```
class GroupApplicationPage
  : public im.floo.floolib.BMXBaseObject
```

### Summary

| Members                                                                                                    | Descriptions |
| ---------------------------------------------------------------------------------------------------------- | ------------ |
| `public transient long swigCPtr`                                                                           |              |
| `public inline synchronized void delete()`                                                                 |              |
| `public inline GroupApplicationPage()`                                                                     |              |
| `public inline GroupApplicationPage(`[`BMXGroupApplicationList`](broken-reference) `result,long offset)`   |              |
| `public inline GroupApplicationPage(`[`BMXGroupApplicationList`](broken-reference) `result,String cursor)` |              |
| `public inline GroupApplicationPage(`[`GroupApplicationPage`](broken-reference) `from)`                    |              |
| `public inline long count()`                                                                               |              |
| `public inline long offset()`                                                                              |              |
| `public inline String cursor()`                                                                            |              |
| `public inline` [`BMXGroupApplicationList`](broken-reference) `result()`                                   |              |
| `protected inline GroupApplicationPage(long cPtr,boolean cMemoryOwn)`                                      |              |
| `protected inline void finalize()`                                                                         |              |

### Members

#### `public transient long swigCPtr` <a href="#classim_1_1floo_1_1floolib_1_1_group_application_page_1a1f2fceaaa0a442ccc12a0c10a464d5fe" id="classim_1_1floo_1_1floolib_1_1_group_application_page_1a1f2fceaaa0a442ccc12a0c10a464d5fe"></a>

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_group_application_page_1afcfa476ad75aa848ff4f4269cdde3e50" id="classim_1_1floo_1_1floolib_1_1_group_application_page_1afcfa476ad75aa848ff4f4269cdde3e50"></a>

#### `public inline GroupApplicationPage()` <a href="#classim_1_1floo_1_1floolib_1_1_group_application_page_1aaa43566214ca91c731aab60c0a1f72e8" id="classim_1_1floo_1_1floolib_1_1_group_application_page_1aaa43566214ca91c731aab60c0a1f72e8"></a>

#### `public inline GroupApplicationPage(`[`BMXGroupApplicationList`](broken-reference) `result,long offset)` <a href="#classim_1_1floo_1_1floolib_1_1_group_application_page_1a6dd9928d26078040c51dc9a744e21aa4" id="classim_1_1floo_1_1floolib_1_1_group_application_page_1a6dd9928d26078040c51dc9a744e21aa4"></a>

#### `public inline GroupApplicationPage(`[`BMXGroupApplicationList`](broken-reference) `result,String cursor)` <a href="#classim_1_1floo_1_1floolib_1_1_group_application_page_1a9b9cd0432435367d7a43ccf3a10dcfae" id="classim_1_1floo_1_1floolib_1_1_group_application_page_1a9b9cd0432435367d7a43ccf3a10dcfae"></a>

#### `public inline GroupApplicationPage(`[`GroupApplicationPage`](broken-reference) `from)` <a href="#classim_1_1floo_1_1floolib_1_1_group_application_page_1a133452ee2e27f39b83011180790b2c9c" id="classim_1_1floo_1_1floolib_1_1_group_application_page_1a133452ee2e27f39b83011180790b2c9c"></a>

#### `public inline long count()` <a href="#classim_1_1floo_1_1floolib_1_1_group_application_page_1aad9b8958eb1eb248c67257ba3d51970a" id="classim_1_1floo_1_1floolib_1_1_group_application_page_1aad9b8958eb1eb248c67257ba3d51970a"></a>

#### `public inline long offset()` <a href="#classim_1_1floo_1_1floolib_1_1_group_application_page_1a3c6568db6e62cb7d4d9d83e0bca7f3dc" id="classim_1_1floo_1_1floolib_1_1_group_application_page_1a3c6568db6e62cb7d4d9d83e0bca7f3dc"></a>

#### `public inline String cursor()` <a href="#classim_1_1floo_1_1floolib_1_1_group_application_page_1a53cc7311dbb6dc74f9a72cc1a9dad30f" id="classim_1_1floo_1_1floolib_1_1_group_application_page_1a53cc7311dbb6dc74f9a72cc1a9dad30f"></a>

#### `public inline` [`BMXGroupApplicationList`](broken-reference) `result()` <a href="#classim_1_1floo_1_1floolib_1_1_group_application_page_1a79c3a2b42bba99a509ccd888da18c2bf" id="classim_1_1floo_1_1floolib_1_1_group_application_page_1a79c3a2b42bba99a509ccd888da18c2bf"></a>

#### `protected inline GroupApplicationPage(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_group_application_page_1a168d935ee543061e5c5c6b28fbe18804" id="classim_1_1floo_1_1floolib_1_1_group_application_page_1a168d935ee543061e5c5c6b28fbe18804"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_group_application_page_1afe66938fe2044fa01afc2c36b82c7077" id="classim_1_1floo_1_1floolib_1_1_group_application_page_1afe66938fe2044fa01afc2c36b82c7077"></a>

## class `GroupInvitaionPage` <a href="#classim_1_1floo_1_1floolib_1_1_group_invitaion_page" id="classim_1_1floo_1_1floolib_1_1_group_invitaion_page"></a>

```
class GroupInvitaionPage
  : public im.floo.floolib.BMXBaseObject
```

### Summary

| Members                                                                                                 | Descriptions |
| ------------------------------------------------------------------------------------------------------- | ------------ |
| `public transient long swigCPtr`                                                                        |              |
| `public inline synchronized void delete()`                                                              |              |
| `public inline GroupInvitaionPage()`                                                                    |              |
| `public inline GroupInvitaionPage(`[`BMXGroupInvitationList`](broken-reference) `result,long offset)`   |              |
| `public inline GroupInvitaionPage(`[`BMXGroupInvitationList`](broken-reference) `result,String cursor)` |              |
| `public inline GroupInvitaionPage(`[`GroupInvitaionPage`](broken-reference) `from)`                     |              |
| `public inline long count()`                                                                            |              |
| `public inline long offset()`                                                                           |              |
| `public inline String cursor()`                                                                         |              |
| `public inline` [`BMXGroupInvitationList`](broken-reference) `result()`                                 |              |
| `protected inline GroupInvitaionPage(long cPtr,boolean cMemoryOwn)`                                     |              |
| `protected inline void finalize()`                                                                      |              |

### Members

#### `public transient long swigCPtr` <a href="#classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1ae5b05c38431c95f79f58c92cdc705c41" id="classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1ae5b05c38431c95f79f58c92cdc705c41"></a>

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1a5b342489a0eb4832c90185f960025946" id="classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1a5b342489a0eb4832c90185f960025946"></a>

#### `public inline GroupInvitaionPage()` <a href="#classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1afad853bf893576c2ac8805a144c680d7" id="classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1afad853bf893576c2ac8805a144c680d7"></a>

#### `public inline GroupInvitaionPage(`[`BMXGroupInvitationList`](broken-reference) `result,long offset)` <a href="#classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1a91db202469ceec35a70441d5b2c657ac" id="classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1a91db202469ceec35a70441d5b2c657ac"></a>

#### `public inline GroupInvitaionPage(`[`BMXGroupInvitationList`](broken-reference) `result,String cursor)` <a href="#classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1a96952ffd5368419b6efccc8e314660ce" id="classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1a96952ffd5368419b6efccc8e314660ce"></a>

#### `public inline GroupInvitaionPage(`[`GroupInvitaionPage`](broken-reference) `from)` <a href="#classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1a774600295264605f0cbe0cdc1ce8e548" id="classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1a774600295264605f0cbe0cdc1ce8e548"></a>

#### `public inline long count()` <a href="#classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1a411085f2e9756995ed952f0f28ba59cc" id="classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1a411085f2e9756995ed952f0f28ba59cc"></a>

#### `public inline long offset()` <a href="#classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1a06b002d1fe5c36103285b39b4955066d" id="classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1a06b002d1fe5c36103285b39b4955066d"></a>

#### `public inline String cursor()` <a href="#classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1a6365cce961dd6bca9b2e00bf7264ef12" id="classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1a6365cce961dd6bca9b2e00bf7264ef12"></a>

#### `public inline` [`BMXGroupInvitationList`](broken-reference) `result()` <a href="#classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1afa28082e91efc1d23bda2b880e0f4db3" id="classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1afa28082e91efc1d23bda2b880e0f4db3"></a>

#### `protected inline GroupInvitaionPage(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1aacb5ed629c9b7a13bf46e156ac050c47" id="classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1aacb5ed629c9b7a13bf46e156ac050c47"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1a22e3d3d648347e0ef13c9b8c9d4d08af" id="classim_1_1floo_1_1floolib_1_1_group_invitaion_page_1a22e3d3d648347e0ef13c9b8c9d4d08af"></a>

## class `ListOfLongLong` <a href="#classim_1_1floo_1_1floolib_1_1_list_of_long_long" id="classim_1_1floo_1_1floolib_1_1_list_of_long_long"></a>

### Summary

| Members                                                         | Descriptions |
| --------------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`                      |              |
| `public inline ListOfLongLong()`                                |              |
| `public inline ListOfLongLong(long n)`                          |              |
| `public inline long size()`                                     |              |
| `public inline long capacity()`                                 |              |
| `public inline void reserve(long n)`                            |              |
| `public inline boolean isEmpty()`                               |              |
| `public inline void clear()`                                    |              |
| `public inline void add(long x)`                                |              |
| `public inline long get(int i)`                                 |              |
| `public inline void set(int i,long val)`                        |              |
| `protected transient boolean swigCMemOwn`                       |              |
| `protected inline ListOfLongLong(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                              |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a8148e91291e865ba060ef1320d970068" id="classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a8148e91291e865ba060ef1320d970068"></a>

#### `public inline ListOfLongLong()` <a href="#classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a9cf325de66cd71f9df7013cda606a0b1" id="classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a9cf325de66cd71f9df7013cda606a0b1"></a>

#### `public inline ListOfLongLong(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a501b70144a7872c643a1822560cf23c5" id="classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a501b70144a7872c643a1822560cf23c5"></a>

#### `public inline long size()` <a href="#classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a53fdb0535d9a07abdbbbafadb1f28a8c" id="classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a53fdb0535d9a07abdbbbafadb1f28a8c"></a>

#### `public inline long capacity()` <a href="#classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a5d375566eede9718e48d529f7214186d" id="classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a5d375566eede9718e48d529f7214186d"></a>

#### `public inline void reserve(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a745b7483673c3170f4359e4fea911464" id="classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a745b7483673c3170f4359e4fea911464"></a>

#### `public inline boolean isEmpty()` <a href="#classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a9c806334520888aa573bb3635795352e" id="classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a9c806334520888aa573bb3635795352e"></a>

#### `public inline void clear()` <a href="#classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a8fb717ade89c3fad95d584f2a07221b1" id="classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a8fb717ade89c3fad95d584f2a07221b1"></a>

#### `public inline void add(long x)` <a href="#classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a1c80f472aa3e13ce9013c95c836b1597" id="classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a1c80f472aa3e13ce9013c95c836b1597"></a>

#### `public inline long get(int i)` <a href="#classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a8aaf411e3424e35c752ffddf14e6b643" id="classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a8aaf411e3424e35c752ffddf14e6b643"></a>

#### `public inline void set(int i,long val)` <a href="#classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a56c99b34bb2599b18d4c8aa426f9d69e" id="classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a56c99b34bb2599b18d4c8aa426f9d69e"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_list_of_long_long_1ae37b7351baa402709bab404a6bb110ba" id="classim_1_1floo_1_1floolib_1_1_list_of_long_long_1ae37b7351baa402709bab404a6bb110ba"></a>

#### `protected inline ListOfLongLong(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a28078ed432e017f3fe05487277554239" id="classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a28078ed432e017f3fe05487277554239"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a3e8a0e8cb6b51f10d73d77fb6173caa0" id="classim_1_1floo_1_1floolib_1_1_list_of_long_long_1a3e8a0e8cb6b51f10d73d77fb6173caa0"></a>

## class `TagList` <a href="#classim_1_1floo_1_1floolib_1_1_tag_list" id="classim_1_1floo_1_1floolib_1_1_tag_list"></a>

### Summary

| Members                                                  | Descriptions |
| -------------------------------------------------------- | ------------ |
| `public inline synchronized void delete()`               |              |
| `public inline TagList()`                                |              |
| `public inline TagList(long n)`                          |              |
| `public inline long size()`                              |              |
| `public inline long capacity()`                          |              |
| `public inline void reserve(long n)`                     |              |
| `public inline boolean isEmpty()`                        |              |
| `public inline void clear()`                             |              |
| `public inline void add(String x)`                       |              |
| `public inline String get(int i)`                        |              |
| `public inline void set(int i,String val)`               |              |
| `protected transient boolean swigCMemOwn`                |              |
| `protected inline TagList(long cPtr,boolean cMemoryOwn)` |              |
| `protected inline void finalize()`                       |              |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_tag_list_1ab4e2007252f3398f64975e8c1df49051" id="classim_1_1floo_1_1floolib_1_1_tag_list_1ab4e2007252f3398f64975e8c1df49051"></a>

#### `public inline TagList()` <a href="#classim_1_1floo_1_1floolib_1_1_tag_list_1ac1143eb3a21813db0f352075b3025ddc" id="classim_1_1floo_1_1floolib_1_1_tag_list_1ac1143eb3a21813db0f352075b3025ddc"></a>

#### `public inline TagList(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_tag_list_1aef89e45b38283de5d914e3321f60c05c" id="classim_1_1floo_1_1floolib_1_1_tag_list_1aef89e45b38283de5d914e3321f60c05c"></a>

#### `public inline long size()` <a href="#classim_1_1floo_1_1floolib_1_1_tag_list_1aba69231a6e3fadf9c20cdfd12e38a022" id="classim_1_1floo_1_1floolib_1_1_tag_list_1aba69231a6e3fadf9c20cdfd12e38a022"></a>

#### `public inline long capacity()` <a href="#classim_1_1floo_1_1floolib_1_1_tag_list_1a0c808b66f10a5dc91ff042ed62a4f09d" id="classim_1_1floo_1_1floolib_1_1_tag_list_1a0c808b66f10a5dc91ff042ed62a4f09d"></a>

#### `public inline void reserve(long n)` <a href="#classim_1_1floo_1_1floolib_1_1_tag_list_1a41baeb698dc17bb356bfae6f4d47b0ed" id="classim_1_1floo_1_1floolib_1_1_tag_list_1a41baeb698dc17bb356bfae6f4d47b0ed"></a>

#### `public inline boolean isEmpty()` <a href="#classim_1_1floo_1_1floolib_1_1_tag_list_1a0adb1c12172dad7ed8601482e06b0bdf" id="classim_1_1floo_1_1floolib_1_1_tag_list_1a0adb1c12172dad7ed8601482e06b0bdf"></a>

#### `public inline void clear()` <a href="#classim_1_1floo_1_1floolib_1_1_tag_list_1a40a73d7ece3834deaf2e0957b913ca0b" id="classim_1_1floo_1_1floolib_1_1_tag_list_1a40a73d7ece3834deaf2e0957b913ca0b"></a>

#### `public inline void add(String x)` <a href="#classim_1_1floo_1_1floolib_1_1_tag_list_1a02bb2492ffdb86d33dbde408b92f5062" id="classim_1_1floo_1_1floolib_1_1_tag_list_1a02bb2492ffdb86d33dbde408b92f5062"></a>

#### `public inline String get(int i)` <a href="#classim_1_1floo_1_1floolib_1_1_tag_list_1a91cc241778f26a016eed38635dfd11ba" id="classim_1_1floo_1_1floolib_1_1_tag_list_1a91cc241778f26a016eed38635dfd11ba"></a>

#### `public inline void set(int i,String val)` <a href="#classim_1_1floo_1_1floolib_1_1_tag_list_1a441577441016f66bcd37882cd9549e69" id="classim_1_1floo_1_1floolib_1_1_tag_list_1a441577441016f66bcd37882cd9549e69"></a>

#### `protected transient boolean swigCMemOwn` <a href="#classim_1_1floo_1_1floolib_1_1_tag_list_1a7f223a7298438fab57901af6834779da" id="classim_1_1floo_1_1floolib_1_1_tag_list_1a7f223a7298438fab57901af6834779da"></a>

#### `protected inline TagList(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_tag_list_1a96c72e11ba4ff100d0a764cb99b82d55" id="classim_1_1floo_1_1floolib_1_1_tag_list_1a96c72e11ba4ff100d0a764cb99b82d55"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_tag_list_1a793df6c008f42e39ee6b32af38ed13f9" id="classim_1_1floo_1_1floolib_1_1_tag_list_1a793df6c008f42e39ee6b32af38ed13f9"></a>

## class `UserProfileImpl` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl"></a>

```
class UserProfileImpl
  : public im.floo.floolib.BMXUserProfile
```

### Summary

| Members                                                                                  | Descriptions      |
| ---------------------------------------------------------------------------------------- | ----------------- |
| `public inline synchronized void delete()`                                               |                   |
| `public inline UserProfileImpl(long uid)`                                                |                   |
| `public inline long userId()`                                                            | 用户ID（唯一）          |
| `public inline BMXUserProfile.UserCategory category()`                                   | 用户策略              |
| `public inline String username()`                                                        | 用户名（唯一）           |
| `public inline String nickname()`                                                        | 用户昵称              |
| `public inline String avatarRatelUrl()`                                                  | 用户头像ratel服务器地址    |
| `public inline String avatarUrl()`                                                       | 用户头像              |
| `public inline String avatarPath()`                                                      | 用户头像本地存储路径        |
| `public inline String avatarThumbnailPath()`                                             | 用户头像缩略图本地存储路径     |
| `public inline String mobilePhone()`                                                     | 用户手机              |
| `public inline String email()`                                                           | 用户邮箱              |
| `public inline String publicInfo()`                                                      | 用户公开扩展信息，好友可见     |
| `public inline String privateInfo()`                                                     | 用户私有扩展信息，好友不可见    |
| `public inline BMXUserProfile.AddFriendAuthMode addFriendAuthMode()`                     | 加好友校验方式           |
| `public inline BMXUserProfile.AuthQuestion authQuestion()`                               | 添加好友时的验证问题        |
| `public inline BMXUserProfile.MessageSetting messageSetting()`                           | 用户消息设定            |
| `public inline boolean isAutoAcceptGroupInvite()`                                        | 收到群组邀请进群时是否自动同意进群 |
| `public inline void calculateUrl(String storeToken,String accessKeySecret,String appId)` |                   |
| `public inline void set_userId(long value)`                                              |                   |
| `public inline long get_userId()`                                                        |                   |
| `public inline void set_category(BMXUserProfile.UserCategory value)`                     |                   |
| `public inline BMXUserProfile.UserCategory get_category()`                               |                   |
| `public inline void set_username(String value)`                                          |                   |
| `public inline String get_username()`                                                    |                   |
| `public inline void set_nickname(String value)`                                          |                   |
| `public inline String get_nickname()`                                                    |                   |
| `public inline void set_avatarRatelUrl(String value)`                                    |                   |
| `public inline String get_avatarRatelUrl()`                                              |                   |
| `public inline void set_avatarUrl(String value)`                                         |                   |
| `public inline String get_avatarUrl()`                                                   |                   |
| `public inline void set_avatarPath(String value)`                                        |                   |
| `public inline String get_avatarPath()`                                                  |                   |
| `public inline void set_avatarThumbnailPath(String value)`                               |                   |
| `public inline String get_avatarThumbnailPath()`                                         |                   |
| `public inline void set_mobilePhone(String value)`                                       |                   |
| `public inline String get_mobilePhone()`                                                 |                   |
| `public inline void set_email(String value)`                                             |                   |
| `public inline String get_email()`                                                       |                   |
| `public inline void set_publicInfo(String value)`                                        |                   |
| `public inline String get_publicInfo()`                                                  |                   |
| `public inline void set_privateInfo(String value)`                                       |                   |
| `public inline String get_privateInfo()`                                                 |                   |
| `public inline void set_addFriendAuthMode(BMXUserProfile.AddFriendAuthMode value)`       |                   |
| `public inline BMXUserProfile.AddFriendAuthMode get_addFriendAuthMode()`                 |                   |
| `public inline void set_authQuestion(BMXUserProfile.AuthQuestion value)`                 |                   |
| `public inline BMXUserProfile.AuthQuestion get_authQuestion()`                           |                   |
| `public inline void set_messageSetting(BMXUserProfile.MessageSetting value)`             |                   |
| `public inline BMXUserProfile.MessageSetting get_messageSetting()`                       |                   |
| `public inline void set_isAutoAcceptGroupInvite(boolean value)`                          |                   |
| `public inline boolean get_isAutoAcceptGroupInvite()`                                    |                   |
| `public inline void set_token(String value)`                                             |                   |
| `public inline String get_token()`                                                       |                   |
| `public inline void set_tokenExpireTime(long value)`                                     |                   |
| `public inline long get_tokenExpireTime()`                                               |                   |
| `public inline void set_rosterVersion(long value)`                                       |                   |
| `public inline long get_rosterVersion()`                                                 |                   |
| `public inline void set_encryptPubKey(String value)`                                     |                   |
| `public inline String get_encryptPubKey()`                                               |                   |
| `public inline void set_encryptType(int value)`                                          |                   |
| `public inline int get_encryptType()`                                                    |                   |
| `public inline void set_deviceGUID(String value)`                                        |                   |
| `public inline String get_deviceGUID()`                                                  |                   |
| `public inline void set_deviceToken(String value)`                                       |                   |
| `public inline String get_deviceToken()`                                                 |                   |
| `public inline void set_cacheBaseDir(String value)`                                      |                   |
| `public inline String get_cacheBaseDir()`                                                |                   |
| `public inline void set_appId(String value)`                                             |                   |
| `public inline String get_appId()`                                                       |                   |
| `public inline void set_storeToken(String value)`                                        |                   |
| `public inline String get_storeToken()`                                                  |                   |
| `public inline void set_accessKeySecret(String value)`                                   |                   |
| `public inline String get_accessKeySecret()`                                             |                   |
| `public inline void set_appSecret(String value)`                                         |                   |
| `public inline String get_appSecret()`                                                   |                   |
| `public inline void set_pushAlias(String value)`                                         |                   |
| `public inline String get_pushAlias()`                                                   |                   |
| `public inline void set_pushToken(String value)`                                         |                   |
| `public inline String get_pushToken()`                                                   |                   |
| `public inline void set_pushCertName(String value)`                                      |                   |
| `public inline String get_pushCertName()`                                                |                   |
| `public inline void set_pushCertContent(String value)`                                   |                   |
| `public inline String get_pushCertContent()`                                             |                   |
| `public inline void set_deviceSN(int value)`                                             |                   |
| `public inline int get_deviceSN()`                                                       |                   |
| `protected inline UserProfileImpl(long cPtr,boolean cMemoryOwn)`                         |                   |
| `protected inline void finalize()`                                                       |                   |

### Members

#### `public inline synchronized void delete()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1af9083d9f251faae89c56fc9097c1c8f6" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1af9083d9f251faae89c56fc9097c1c8f6"></a>

#### `public inline UserProfileImpl(long uid)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a8b7fcd799ceb86f2e2d8aaf17768275e" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a8b7fcd799ceb86f2e2d8aaf17768275e"></a>

#### `public inline long userId()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ad81873e4efa2b2bf829c0dac365b63c8" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ad81873e4efa2b2bf829c0dac365b63c8"></a>

用户ID（唯一）

**Returns**

int64\_t

#### `public inline BMXUserProfile.UserCategory category()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ad31665ab2743e223f7a0747f5b5f1d4a" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ad31665ab2743e223f7a0747f5b5f1d4a"></a>

用户策略

**Returns**

UserCategory

#### `public inline String username()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a00e3c1970b945d0a3f7cbb2298279c35" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a00e3c1970b945d0a3f7cbb2298279c35"></a>

用户名（唯一）

**Returns**

std::string

#### `public inline String nickname()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ab06b2fd03ecc776aaf54c3fb65c834d8" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ab06b2fd03ecc776aaf54c3fb65c834d8"></a>

用户昵称

**Returns**

std::string

#### `public inline String avatarRatelUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a24a0fff466a8104739631c8add18c9ac" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a24a0fff466a8104739631c8add18c9ac"></a>

用户头像ratel服务器地址

**Returns**

std::string

#### `public inline String avatarUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ab5e99e98d8491d503d40d3b669e0f98d" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ab5e99e98d8491d503d40d3b669e0f98d"></a>

用户头像

**Returns**

std::string

#### `public inline String avatarPath()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a8132b4dd08cffb65b2d99bdd3642ea2d" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a8132b4dd08cffb65b2d99bdd3642ea2d"></a>

用户头像本地存储路径

**Returns**

std::string

#### `public inline String avatarThumbnailPath()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1af98c988306e803d77be8d69d52d4fd92" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1af98c988306e803d77be8d69d52d4fd92"></a>

用户头像缩略图本地存储路径

**Returns**

std::string

#### `public inline String mobilePhone()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1abf752b5bb0c80c1d5b20f873368878ea" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1abf752b5bb0c80c1d5b20f873368878ea"></a>

用户手机

**Returns**

std::string

#### `public inline String email()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a9674b00442d226125f4a1dc7384e14d8" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a9674b00442d226125f4a1dc7384e14d8"></a>

用户邮箱

**Returns**

std::string

#### `public inline String publicInfo()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ab9bc0138c4b61cb26a9700e6f762d00c" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ab9bc0138c4b61cb26a9700e6f762d00c"></a>

用户公开扩展信息，好友可见

**Returns**

JSON(std::string)

#### `public inline String privateInfo()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1acb19cc750fbfd5eadfd45a27121c9152" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1acb19cc750fbfd5eadfd45a27121c9152"></a>

用户私有扩展信息，好友不可见

**Returns**

JSON(std::string)

#### `public inline BMXUserProfile.AddFriendAuthMode addFriendAuthMode()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a0e6dc5a579724970817264424849a376" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a0e6dc5a579724970817264424849a376"></a>

加好友校验方式

**Returns**

AddFriendAuthMode

#### `public inline BMXUserProfile.AuthQuestion authQuestion()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a5cf5b712761037e5a45a6df7dfd750ce" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a5cf5b712761037e5a45a6df7dfd750ce"></a>

添加好友时的验证问题

**Returns**

AuthQuestion

#### `public inline BMXUserProfile.MessageSetting messageSetting()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1aa1863810dc78fd948c0ac041a1b1d143" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1aa1863810dc78fd948c0ac041a1b1d143"></a>

用户消息设定

**Returns**

MessageSetting

#### `public inline boolean isAutoAcceptGroupInvite()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a5117e963ea92a0f7326350d4d2fbc552" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a5117e963ea92a0f7326350d4d2fbc552"></a>

收到群组邀请进群时是否自动同意进群

**Returns**

bool

#### `public inline void calculateUrl(String storeToken,String accessKeySecret,String appId)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a94f3187f204f1b36e0e1e6bfddcd8d09" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a94f3187f204f1b36e0e1e6bfddcd8d09"></a>

#### `public inline void set_userId(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a68200b2f3e3110c2a602b3600241ebfa" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a68200b2f3e3110c2a602b3600241ebfa"></a>

#### `public inline long get_userId()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1aaa87588d10dee02134160a4ab04171e7" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1aaa87588d10dee02134160a4ab04171e7"></a>

#### `public inline void set_category(BMXUserProfile.UserCategory value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ab78641e63a421ec4741e6c2408c307a0" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ab78641e63a421ec4741e6c2408c307a0"></a>

#### `public inline BMXUserProfile.UserCategory get_category()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a986fac946729fdaaa0096a193679adb2" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a986fac946729fdaaa0096a193679adb2"></a>

#### `public inline void set_username(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a5cd3200304ed8b95fcab63557ece909c" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a5cd3200304ed8b95fcab63557ece909c"></a>

#### `public inline String get_username()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1afa5c9f63ec1d8fa79c4ab07a1176af4a" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1afa5c9f63ec1d8fa79c4ab07a1176af4a"></a>

#### `public inline void set_nickname(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a88d4822891b79cefd4750a768f961a38" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a88d4822891b79cefd4750a768f961a38"></a>

#### `public inline String get_nickname()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1aea1370344cfb49a82d9db597ed7b72e0" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1aea1370344cfb49a82d9db597ed7b72e0"></a>

#### `public inline void set_avatarRatelUrl(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ac5871f73c1b91aac006a43167848c555" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ac5871f73c1b91aac006a43167848c555"></a>

#### `public inline String get_avatarRatelUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ac630b30795b558e8324cd573f515ab05" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ac630b30795b558e8324cd573f515ab05"></a>

#### `public inline void set_avatarUrl(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a8eeb153c3eff2e30a20b95862c5e4c21" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a8eeb153c3eff2e30a20b95862c5e4c21"></a>

#### `public inline String get_avatarUrl()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a9eaf1a29f66f7873ca34a1d7c5cf837f" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a9eaf1a29f66f7873ca34a1d7c5cf837f"></a>

#### `public inline void set_avatarPath(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a2a16ec08271757a05d0184dbdc513a09" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a2a16ec08271757a05d0184dbdc513a09"></a>

#### `public inline String get_avatarPath()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a4ea236c13580aa59622f2a29f931cf13" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a4ea236c13580aa59622f2a29f931cf13"></a>

#### `public inline void set_avatarThumbnailPath(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a820afd91c3a9b0548bc52ff8f67efc7a" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a820afd91c3a9b0548bc52ff8f67efc7a"></a>

#### `public inline String get_avatarThumbnailPath()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ae63941ee8368895845895c14294f62e6" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ae63941ee8368895845895c14294f62e6"></a>

#### `public inline void set_mobilePhone(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a047049c014d4d06faee51b05fe7e873c" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a047049c014d4d06faee51b05fe7e873c"></a>

#### `public inline String get_mobilePhone()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ad3d1e24b5a937e91e69a14d49e7c5687" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ad3d1e24b5a937e91e69a14d49e7c5687"></a>

#### `public inline void set_email(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ac74ad4bcac59eb30fcdf825bcc38a992" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ac74ad4bcac59eb30fcdf825bcc38a992"></a>

#### `public inline String get_email()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1abcb1190c9c406f8598c8011689c1c4d5" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1abcb1190c9c406f8598c8011689c1c4d5"></a>

#### `public inline void set_publicInfo(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ae01423bfcb87d881678705823b0ef92a" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ae01423bfcb87d881678705823b0ef92a"></a>

#### `public inline String get_publicInfo()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ab78265f99facb57b245cb6e7a06cbb0a" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ab78265f99facb57b245cb6e7a06cbb0a"></a>

#### `public inline void set_privateInfo(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a73add73aa2a9c7c73aef1def80de2838" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a73add73aa2a9c7c73aef1def80de2838"></a>

#### `public inline String get_privateInfo()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ace88f9d18699ec3d8db28d6bc6756d2c" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ace88f9d18699ec3d8db28d6bc6756d2c"></a>

#### `public inline void set_addFriendAuthMode(BMXUserProfile.AddFriendAuthMode value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a1e77d17f2d346bf45203f29957a8e34c" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a1e77d17f2d346bf45203f29957a8e34c"></a>

#### `public inline BMXUserProfile.AddFriendAuthMode get_addFriendAuthMode()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ab28c15d0f5252129fca55fa034e6bc6c" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ab28c15d0f5252129fca55fa034e6bc6c"></a>

#### `public inline void set_authQuestion(BMXUserProfile.AuthQuestion value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a076ec1e14fdd8175d71191c93720c209" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a076ec1e14fdd8175d71191c93720c209"></a>

#### `public inline BMXUserProfile.AuthQuestion get_authQuestion()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a9eb535edc2b9b0bd1a7222431da7f87a" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a9eb535edc2b9b0bd1a7222431da7f87a"></a>

#### `public inline void set_messageSetting(BMXUserProfile.MessageSetting value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a79bfded3902d6347e5b77b28cd1139c3" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a79bfded3902d6347e5b77b28cd1139c3"></a>

#### `public inline BMXUserProfile.MessageSetting get_messageSetting()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1aaea937ebbc9eb0ca149a92873f2c0d55" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1aaea937ebbc9eb0ca149a92873f2c0d55"></a>

#### `public inline void set_isAutoAcceptGroupInvite(boolean value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a78a3fb78dae920ddf1861a3c0b8cb272" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a78a3fb78dae920ddf1861a3c0b8cb272"></a>

#### `public inline boolean get_isAutoAcceptGroupInvite()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a74a70ccc512ea3c7ff8c1fb61eb79f93" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a74a70ccc512ea3c7ff8c1fb61eb79f93"></a>

#### `public inline void set_token(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a09be1d23e8ddbea862a7a4e446721986" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a09be1d23e8ddbea862a7a4e446721986"></a>

#### `public inline String get_token()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a7955cb781db350e4a301ba99bbfda49e" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a7955cb781db350e4a301ba99bbfda49e"></a>

#### `public inline void set_tokenExpireTime(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a09fec06c1e234185d0e6af3071478a45" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a09fec06c1e234185d0e6af3071478a45"></a>

#### `public inline long get_tokenExpireTime()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a478cb2a5083f0fab40060223dbf03621" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a478cb2a5083f0fab40060223dbf03621"></a>

#### `public inline void set_rosterVersion(long value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a7a7b5e6d657d7d152d9d8bc4e1c9e471" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a7a7b5e6d657d7d152d9d8bc4e1c9e471"></a>

#### `public inline long get_rosterVersion()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ae126d8dada00bd80441f00e9cc7d2551" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ae126d8dada00bd80441f00e9cc7d2551"></a>

#### `public inline void set_encryptPubKey(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ab32a46d4f32930162619de20f80ed870" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ab32a46d4f32930162619de20f80ed870"></a>

#### `public inline String get_encryptPubKey()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a363d8c54656d375d516007f8fc3b8c4c" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a363d8c54656d375d516007f8fc3b8c4c"></a>

#### `public inline void set_encryptType(int value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1adf96ef4df4dc650a3a5c31db6e8e8158" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1adf96ef4df4dc650a3a5c31db6e8e8158"></a>

#### `public inline int get_encryptType()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1abf06fba89446504f26002d12a6d20b77" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1abf06fba89446504f26002d12a6d20b77"></a>

#### `public inline void set_deviceGUID(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a1f2153230553cd6403bfd0a30b535bea" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a1f2153230553cd6403bfd0a30b535bea"></a>

#### `public inline String get_deviceGUID()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a6c32b5b17a094e3e9d90d15ee496a939" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a6c32b5b17a094e3e9d90d15ee496a939"></a>

#### `public inline void set_deviceToken(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1abce2a759a51430c2d3bcc77d0d582f83" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1abce2a759a51430c2d3bcc77d0d582f83"></a>

#### `public inline String get_deviceToken()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a29ebdc82f484d3402adbfbaa3cddaafb" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a29ebdc82f484d3402adbfbaa3cddaafb"></a>

#### `public inline void set_cacheBaseDir(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ac10783da3bc304d01d5d0fc469269426" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1ac10783da3bc304d01d5d0fc469269426"></a>

#### `public inline String get_cacheBaseDir()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a04e0a4bc766079392612fe30db27c8c0" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a04e0a4bc766079392612fe30db27c8c0"></a>

#### `public inline void set_appId(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1adce179cd68cfa2194228315040d96169" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1adce179cd68cfa2194228315040d96169"></a>

#### `public inline String get_appId()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a203014952525a5f694d57f32855a74bf" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a203014952525a5f694d57f32855a74bf"></a>

#### `public inline void set_storeToken(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a24775dae9f4cadc07b9cee33edf78539" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a24775dae9f4cadc07b9cee33edf78539"></a>

#### `public inline String get_storeToken()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a6f6b206d7fb35ac3d6d4c0f00974ebb4" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a6f6b206d7fb35ac3d6d4c0f00974ebb4"></a>

#### `public inline void set_accessKeySecret(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a9b8b6caae600ee4290992b8ee4dbf26b" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a9b8b6caae600ee4290992b8ee4dbf26b"></a>

#### `public inline String get_accessKeySecret()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a51735b67de31597cb2f5ebbe498dd98b" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a51735b67de31597cb2f5ebbe498dd98b"></a>

#### `public inline void set_appSecret(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1afbd80b803a080b46a8a969e3395cb8c1" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1afbd80b803a080b46a8a969e3395cb8c1"></a>

#### `public inline String get_appSecret()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a4af29a7fdbee406af31e88020f64f4b9" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a4af29a7fdbee406af31e88020f64f4b9"></a>

#### `public inline void set_pushAlias(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a4892bc15a12a827395dee6eae69a9b3c" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a4892bc15a12a827395dee6eae69a9b3c"></a>

#### `public inline String get_pushAlias()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a5106ddbf60b344b3a869d2134ea193f5" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a5106ddbf60b344b3a869d2134ea193f5"></a>

#### `public inline void set_pushToken(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a5f159ad84a4ac286d94d3a148952b073" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a5f159ad84a4ac286d94d3a148952b073"></a>

#### `public inline String get_pushToken()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1adae5df5c78f5d75140877f5732f96119" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1adae5df5c78f5d75140877f5732f96119"></a>

#### `public inline void set_pushCertName(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a70d46921b82892ff9140b409b0a29c20" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a70d46921b82892ff9140b409b0a29c20"></a>

#### `public inline String get_pushCertName()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1aab9667e662866430a5a5f301a7219d58" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1aab9667e662866430a5a5f301a7219d58"></a>

#### `public inline void set_pushCertContent(String value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a4370d039f397b679760fddf1121e3c4a" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a4370d039f397b679760fddf1121e3c4a"></a>

#### `public inline String get_pushCertContent()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a01c32f0c2c09ad2bd0855f76d14b901c" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a01c32f0c2c09ad2bd0855f76d14b901c"></a>

#### `public inline void set_deviceSN(int value)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a79c4d2ddf9bd6a28558683aaeea4ef21" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a79c4d2ddf9bd6a28558683aaeea4ef21"></a>

#### `public inline int get_deviceSN()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a68fe1e3868b9bb0320f6da1318c57b6b" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a68fe1e3868b9bb0320f6da1318c57b6b"></a>

#### `protected inline UserProfileImpl(long cPtr,boolean cMemoryOwn)` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a195910046288f4c4cf6d7df6050cbd30" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a195910046288f4c4cf6d7df6050cbd30"></a>

#### `protected inline void finalize()` <a href="#classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a21b00b62f5456e2ddeac7c8b4143105c" id="classim_1_1floo_1_1floolib_1_1_user_profile_impl_1a21b00b62f5456e2ddeac7c8b4143105c"></a>
