# /`transfer`

> 将玩家转移到另一个服务器上。

**加入版本：** 1.20.30

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 4 |
| **需要作弊** | 是 |
| **额外说明** | 仅专用服务端 |

## 语法

```
transfer <pfidOrMSA: string> <server: string> <port: int>
```

## 参数详解

- **`pfidOrMSA`**:string - 要转移的玩家，可以为Microsoft账户名称（玩家名），或PlayFab ID（当玩家加入或断开与服务器的连接时显示）
- **`server`**:string - 要连接到的服务器的主机名
- **`port`**:int - 要连接到的服务器的端口编号，应在0和65535之间（含）
