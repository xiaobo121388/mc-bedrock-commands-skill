# /`wsserver`

> 用于连接WebSocket服务器，WebSocket服务器使用命令信息与客户端交互。

**加入版本：** 0.16.0

| 属性 | 值 |
|---|---|
| **别名** | `connect, dedicatedwsserver` |
| **权限等级** | 2 |
| **需要作弊** | 是 |
| **额外说明** | 仅适用于基岩版和教育版。自1.21.60版本起，该命令默认禁用，需要在世界选项中开启“启用Websocket”才能使用。不能在命令方块中使用。 |

## 语法

```
wsserver <serverUri: text> | connect <serverUri: text> | dedicatedwsserver <serverUri: message>
```

## 参数详解

- **`serverUri`**:text/message - 指向WebSocket服务器的URI，输入任意字符串断开当前的连接。该参数为贪婪字符串，可以包含空格。
