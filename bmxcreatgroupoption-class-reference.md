# BMXCreatGroupOption Class Reference

| Inherits from | NSObject              |
| ------------- | --------------------- |
| Declared in   | BMXCreatGroupOption.h |

#### &#x20; `name`

群名称

`@property (nonatomic, copy) NSString *name`

**Declared In**

`BMXCreatGroupOption.h`

#### &#x20; `groupDescription`

群描述

`@property (nonatomic, copy) NSString *groupDescription`

**Declared In**

`BMXCreatGroupOption.h`

#### &#x20; `isChatroom`

是否聊天室

`@property (nonatomic, assign) BOOL isChatroom`

**Declared In**

`BMXCreatGroupOption.h`

#### &#x20; `message`

建群时成员收到的邀请信息

`@property (nonatomic, copy) NSString *message`

**Declared In**

`BMXCreatGroupOption.h`

#### &#x20; `avatarPath`

群头像本地路径

`@property (nonatomic, copy) NSString *avatarPath`

**Declared In**

`BMXCreatGroupOption.h`

#### &#x20; `announcement`

群公告

`@property (nonatomic, copy) NSString *announcement`

**Declared In**

`BMXCreatGroupOption.h`

#### &#x20; `members`

建群时添加的成员

`@property (nonatomic, strong) NSArray *members`

**Declared In**

`BMXCreatGroupOption.h`

#### &#x20; `extion`

群扩展信息

`@property (nonatomic, copy) NSString *extion`

**Declared In**

`BMXCreatGroupOption.h`

#### `– initWithGroupName:groupDescription:isPublic:`

创建群实体

`- (instancetype)initWithGroupName:(NSString *)`_`name`_` ``groupDescription:(NSString *)`_`groupDescription`_` ``isPublic:(BOOL)`_`isPublic`_

**Parameters**

| `name`             | 必填  |
| ------------------ | --- |
| `groupDescription` | 非必填 |

**Return Value**

BMXCreatGroupOption

**Declared In**

`BMXCreatGroupOption.h`
