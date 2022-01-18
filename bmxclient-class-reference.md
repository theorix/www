# BMXClient Class Reference

| Inherits from | NSObject    |
| ------------- | ----------- |
| Declared in   | BMXClient.h |

#### `+ sharedClient`

`+ (instancetype)sharedClient`

#### &#x20; `userService`

`@property (nonatomic, strong, readonly) id<BMXUserManager> userService`

#### &#x20; `rosterService`

`@property (nonatomic, strong, readonly) id<BMXRosterManager> rosterService`

#### &#x20; `chatService`

`@property (nonatomic, strong, readonly) id<BMXChatManager> chatService`

#### &#x20; `groupService`

`@property (nonatomic, strong, readonly) id<BMXGroupManager> groupService`

#### &#x20; `pushService`

`@property (nonatomic, strong, readonly) id<BMXPushManager> pushService`

#### &#x20; `sdkConfig`

`@property (nonatomic, strong) BMXSDKConfig *sdkConfig`

#### `– registerWithSDKConfig:`

`- (void)registerWithSDKConfig:(BMXSDKConfig *)`_`config`_

#### `+ getCacheDir`

`+ (NSString *)getCacheDir`

#### `– signUpNewUser:password:completion:`

注册新用户，username和password是必填参数

`- (void)signUpNewUser:(NSString *)`_`userName`_` ``password:(NSString *)`_`password`_` ``completion:(void ( ^ ) ( BMXUserProfile *profile , BMXError *error ))`_`aCompletionBlock`_

**Parameters**

| `userName`         | 用户名                                                   |
| ------------------ | ----------------------------------------------------- |
| `password`         | 密码                                                    |
| `aCompletionBlock` | 注册成功后从该函数处获取新注册用户的Profile信息，初始传入指向为空的shared\_ptr对象即可。 |

**Discussion**

注册新用户，username和password是必填参数

#### `– signInByName:password:completion:`

通过用户名登录

`- (void)signInByName:(NSString *)`_`userName`_` ``password:(NSString *)`_`password`_` ``completion:(void ( ^ ) ( BMXError *error ))`_`aCompletionBlock`_

#### `– signInById:password:completion:`

通过用户ID登录

`- (void)signInById:(long long)`_`userId`_` ``password:(NSString *)`_`password`_` ``completion:(void ( ^ ) ( BMXError *error ))`_`aCompletionBlock`_

#### `– signInById:withToken:completion:`

通过用户ID和token登录

`- (void)signInById:(long long)`_`userId`_` ``withToken:(NSString *)`_`token`_` ``completion:(void ( ^ ) ( BMXError *error ))`_`aCompletionBlock`_

**Discussion**

通过用户ID和token登录

#### `– fastSignInByName:password:completion:`

通过用户名自动登录（要求之前成功登录过，登录速度较快）

`- (void)fastSignInByName:(NSString *)`_`name`_` ``password:(NSString *)`_`password`_` ``completion:(void ( ^ ) ( BMXError *error ))`_`aCompletionBlock`_

**Discussion**

通过用户名自动登录（要求之前成功登录过，登录速度较快）

#### `– fastSignInById:password:completion:`

通过用户ID自动登录（要求之前成功登录过，登录速度较快）

`- (void)fastSignInById:(long long)`_`uid`_` ``password:(NSString *)`_`password`_` ``completion:(void ( ^ ) ( BMXError *error ))`_`aCompletionBlock`_

**Discussion**

通过用户ID自动登录（要求之前成功登录过，登录速度较快）

#### `– signOutID:ignoreUnbindDevice:completion:`

退出登录

`- (void)signOutID:(NSInteger)`_`userID`_` ``ignoreUnbindDevice:(BOOL)`_`ignoreUnbindDevice`_` ``completion:(void ( ^ ) ( BMXError *error ))`_`aCompletionBlock`_

#### `– signOutignoreUnbindDevice:completion:`

`- (void)signOutignoreUnbindDevice:(BOOL)`_`ignoreUnbindDevice`_` ``completion:(void ( ^ ) ( BMXError *error ))`_`aCompletionBlock`_

#### `– signInStatus`

获取当前的登录状态

`- (BMXSignInStatus)signInStatus`

#### `– connectStatus`

获取当前和服务器的连接状态

`- (BMXConnectStatus)connectStatus`

#### `– networkDidChangedType:reconnect:`

处理网络状态发送变化

`- (void)networkDidChangedType:(BMXNetworkType)`_`type`_` ``reconnect:(BOOL)`_`reconnect`_

**Parameters**

| `type`      | 变化后的网络类型 |
| ----------- | -------- |
| `reconnect` | 网络是否需要重连 |

#### `– disConnect`

断开网络连接

`- (void)disConnect`

#### `– changeAppID:completion:`

更改SDK的appId，本操作会同时更新BMXConfig中的appId。

`- (void)changeAppID:(NSString *)`_`appID`_` ``completion:(void ( ^ ) ( BMXError *error ))`_`aCompletionBlock`_

**Parameters**

| `appID` | 新变更的appId |
| ------- | --------- |

**Discussion**

更改SDK的appId，本操作会同时更新BMXConfig中的appId。

#### `– initializeServerConfig:`

获取app的服务器网络配置，在初始化SDK之后登陆之前调用，可以提前获取服务器配置加快登陆速度。

`- (void)initializeServerConfig:(BOOL)`_`isLocal`_

**Parameters**

| `isLocal` | 为true则使用本地缓存的dns配置，为false则从服务器获取最新的配置。 |
| --------- | -------------------------------------- |

**Discussion**

获取app的服务器网络配置，在初始化SDK之后登陆之前调用，可以提前获取服务器配置加快登陆速度。
