# userManage

### userManage

* [userManage](broken-reference)
  * [.getToken()](broken-reference) ⇒ `string`
  * [.getUid()](broken-reference) ⇒ `number`
  * [.getAppid()](broken-reference) ⇒ `string`
  * [.getConversationList()](broken-reference) ⇒ `Array.<module:types~ConversationItem>`
  * [.asyncUpdateAvatar(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncUpdateNickName(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncGetProfile()](broken-reference) ⇒ `Promise.<module:types~UserProfile>`
  * [.asyncUpdateProfile(params)](broken-reference) ⇒ `Promise.<boolean>`
  * [.asyncGetSettings()](broken-reference) ⇒ `Promise.<module:types~UserSettings>`
  * [.asyncUpdateSettings(settings)](broken-reference) ⇒ `Promise.<boolean>`

#### userManage.getToken() ⇒ `string`

获取登录用户的token

**Kind**: static method of [`userManage`](broken-reference)\
**Returns**: `string` - 用户的token\


#### userManage.getUid() ⇒ `number`

获取登录用户的uid

**Kind**: static method of [`userManage`](broken-reference)\
**Returns**: `number` - 用户ID\


#### userManage.getAppid() ⇒ `string`

获取appid

**Kind**: static method of [`userManage`](broken-reference)\
**Returns**: `string` - APP ID\


#### userManage.getConversationList() ⇒ `Array.<module:types~ConversationItem>`

获取最近会话列表

**Kind**: static method of [`userManage`](broken-reference)\


#### userManage.asyncUpdateAvatar(params) ⇒ `Promise.<boolean>`

更新头像

**Kind**: static method of [`userManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param         | Type     | Description |
| ------------- | -------- | ----------- |
| params        | `object` | 参数          |
| params.avatar | `string` | 头像 url      |

#### userManage.asyncUpdateNickName(params) ⇒ `Promise.<boolean>`

更新昵称

**Kind**: static method of [`userManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param             | Type     | Description |
| ----------------- | -------- | ----------- |
| params            | `object` | 参数          |
| params.nick\_name | `string` | 昵称          |

#### userManage.asyncGetProfile() ⇒ `Promise.<module:types~UserProfile>`

获取用户profile

**Kind**: static method of [`userManage`](broken-reference)\
**Returns**: `Promise.<module:types~UserProfile>` - 用户信息\


#### userManage.asyncUpdateProfile(params) ⇒ `Promise.<boolean>`

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

#### userManage.asyncGetSettings() ⇒ `Promise.<module:types~UserSettings>`

获取用户设置信息

**Kind**: static method of [`userManage`](broken-reference)\
**Returns**: `Promise.<module:types~UserSettings>` - 用户信息\


#### userManage.asyncUpdateSettings(settings) ⇒ `Promise.<boolean>`

修改用户设置

**Kind**: static method of [`userManage`](broken-reference)\
**Returns**: `Promise.<boolean>` - 是否成功

| Param    | Type                        | Description |
| -------- | --------------------------- | ----------- |
| settings | `module:types~UserSettings` | 更新的设置       |
