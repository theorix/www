# floo::BMXError

## Public Functions

|                                | Name                                                       |
| ------------------------------ | ---------------------------------------------------------- |
|                                | **BMXError**(BMXErrorCode errorCode)                       |
| virtual                        | **\~BMXError**()                                           |
| [BMXError](broken-reference) & | **operator=**(BMXErrorCode errorCode)                      |
| bool                           | **operator==**(BMXErrorCode errorCode)                     |
| bool                           | **operator==**(const [BMXError](broken-reference) & error) |
| BMXErrorCode                   | **errorCode**()                                            |
| std::string                    | **description**()                                          |

## Public Functions Documentation

### function BMXError

```cpp
BMXError(
    BMXErrorCode errorCode
)
```

### function \~BMXError

```cpp
virtual ~BMXError()
```

### function operator=

```cpp
BMXError & operator=(
    BMXErrorCode errorCode
)
```

### function operator==

```cpp
bool operator==(
    BMXErrorCode errorCode
)
```

### function operator==

```cpp
bool operator==(
    const BMXError & error
)
```

### function errorCode

```cpp
BMXErrorCode errorCode()
```

### function description

```cpp
std::string description()
```

***

Updated on 2022-01-26 at 17:20:40 +0800
