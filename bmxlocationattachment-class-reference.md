# BMXLocationAttachment Class Reference

#### &#x20; `latitude`

`@property (nonatomic) double latitude`

#### &#x20; `longitude`

`@property (nonatomic) double longitude`

#### &#x20; `address`

地址

`@property (nonatomic, copy) NSString *address`

**Declared In**

`BMXLocationAttachment.h`

#### `– initWithLatitude:longitude:address:`

初始化BMXLocationAttachment

`- (instancetype)initWithLatitude:(double)`_`aLatitude`_` ``longitude:(double)`_`aLongitude`_` ``address:(NSString *)`_`aAddress`_

**Parameters**

| `aLatitude`  | 纬度 |
| ------------ | -- |
| `aLongitude` | 经度 |
| `aAddress`   | 地址 |

**Return Value**

BMXLocationAttachment

**Discussion**

初始化BMXLocationAttachment

**Declared In**

`BMXLocationAttachment.h`
