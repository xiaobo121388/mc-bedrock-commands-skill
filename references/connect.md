# /`connect`

> 用于连接到WebSocket服务器，主要在教育版中使用。

**加入版本：** 1.0.0

| 属性 | 值 |
|---|---|
| **别名** | `wsserver,dedicatedwsserver` |
| **权限等级** | 0 |
| **需要作弊** | 否 |
| **额外说明** | 在基岩版 1.21.60 及更高版本中，该指令默认禁用，需要更改选项才能启用。 |

## 语法

```
connect <serverUri: text>
```

## 参数详解

- **`serverUri`**:text/message - 指向WebSocket服务器的URI。这是一个贪婪字符串参数，可以包含空格。输入任意字符串会断开当前连接。
