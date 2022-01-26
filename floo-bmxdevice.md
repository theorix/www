# floo::BMXDevice

设备信息

`#include <bmx_device.h>`

Inherits from BMXBaseObject

## Public Functions

|                     | Name                                                                                    |
| ------------------- | --------------------------------------------------------------------------------------- |
| virtual             | <p><strong>~BMXDevice</strong>()<br>析构函数</p>                                            |
| virtual int         | <p><strong>deviceSN</strong>() =0<br>设备序列号</p>                                          |
| virtual int64\_t    | <p><strong>userId</strong>() =0<br>用户id</p>                                             |
| virtual int         | <p><strong>platform</strong>() =0<br>软件平台</p>                                           |
| virtual std::string | <p><strong>userAgent</strong>() =0<br>用户代理信息</p>                                        |
| virtual void        | <p><strong>setUserAgent</strong>(const std::string &#x26; userAgent) =0<br>设置用户代理信息</p> |
| virtual bool        | <p><strong>isCurrentDevice</strong>() =0<br>是否是当前设备</p>                                 |

## Protected Functions

|   | Name            |
| - | --------------- |
|   | **BMXDevice**() |

## Public Functions Documentation

### function \~BMXDevice

```cpp
inline virtual ~BMXDevice()
```

析构函数

### function deviceSN

```cpp
virtual int deviceSN() =0
```

设备序列号

**Return**: int

### function userId

```cpp
virtual int64_t userId() =0
```

用户id

**Return**: int64\_t

### function platform

```cpp
virtual int platform() =0
```

软件平台

**Return**: int

### function userAgent

```cpp
virtual std::string userAgent() =0
```

用户代理信息

**Return**: std::string

### function setUserAgent

```cpp
virtual void setUserAgent(
    const std::string & userAgent
) =0
```

设置用户代理信息

**Parameters**:

* **userAgent** 用户代理信息

### function isCurrentDevice

```cpp
virtual bool isCurrentDevice() =0
```

是否是当前设备

**Return**: bool

## Protected Functions Documentation

### function BMXDevice

```cpp
inline BMXDevice()
```

***

Updated on 2022-01-26 at 17:20:40 +0800
