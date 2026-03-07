# /`msg`

> 将一条私聊消息发送给一个或多个玩家。

**加入版本：** Alpha 0.16.0

| 属性 | 值 |
|---|---|
| **别名** | `tell,w` |
| **权限等级** | 0 |
| **需要作弊** | 是 |
| **额外说明** | 无 |

## 语法

```
tell <target: target> <message: message> | msg <target: target> <message: message> | w <target: target> <message: message>
```

## 参数详解

- **`target`**:CommandSelector<Player> - 指定私聊消息的接收玩家，必须为玩家名或目标选择器，且目标选择器必须为玩家类型
- **`message`**:CommandMessage - 指定要发送的消息，可以包含空格与目标选择器。
