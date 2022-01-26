# floo::BMXNetworkListener

Inherited by [floo::BMXClient](broken-reference)

## Public Functions

|              | Name                                                         |
| ------------ | ------------------------------------------------------------ |
| virtual      | **\~BMXNetworkListener**()                                   |
| virtual void | **onNetworkChanged**(BMXNetworkType type, bool reconnect) =0 |

## Public Functions Documentation

### function \~BMXNetworkListener

```cpp
inline virtual ~BMXNetworkListener()
```

### function onNetworkChanged

```cpp
virtual void onNetworkChanged(
    BMXNetworkType type,
    bool reconnect
) =0
```

**Reimplemented by**: floo::BMXClient::onNetworkChanged

***

Updated on 2022-01-26 at 17:20:40 +0800
