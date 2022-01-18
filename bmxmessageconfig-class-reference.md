# BMXMessageConfig Class Reference

| Inherits from | NSObject           |
| ------------- | ------------------ |
| Declared in   | BMXMessageConfig.h |

#### &#x20; `mentionAll`

`@property (nonatomic, assign) BOOL mentionAll`

#### &#x20; `mentionList`

`@property (nonatomic, strong) NSArray<NSString*> *mentionList`

#### &#x20; `mentionMessage`

`@property (nonatomic, copy) NSString *mentionMessage`

#### &#x20; `pushMessage`

`@property (nonatomic, copy) NSString *pushMessage`

#### &#x20; `senderName`

`@property (nonatomic, copy) NSString *senderName`

#### &#x20; `groupMemberList`

`@property (nonatomic, strong) NSArray<NSString*> *groupMemberList`

#### `– initConfigWithMentionAll:`

`- (instancetype)initConfigWithMentionAll:(BOOL)`_`isMentionAll`_

#### `– addGroupMember:`

`- (void)addGroupMember:(NSString *)`_`rosterId`_

#### `– removeGroupMember:`

`- (void)removeGroupMember:(NSString *)`_`rosterId`_

#### `– clealerGroupMemberList`

`- (void)clealerGroupMemberList`
