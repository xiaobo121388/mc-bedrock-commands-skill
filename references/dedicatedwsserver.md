# /`dedicatedwsserver`

> 用于连接到WebSocket服务器，主要在教育版中使用。

| 属性 | 值 |
|---|---|
| **别名** | `wsserver,connect` |
| **权限等级** | 0 |
| **需要作弊** | 是 |
| **额外说明** | 该指令仅适用于基岩版和教育版。自基岩版1.21.60起，该功能默认禁用，需要通过更改选项来启用。 |

## 语法

```
dedicatedwsserver <serverUri: message> | wsserver <serverUri: text> | connect <serverUri: text>
```

## 参数详解

- **`serverUri`**:message/text - 指向WebSocket服务器的URI。这是一个贪婪字符串参数，可以包含空格。输入任意字符串会断开当前连接。
