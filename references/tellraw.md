# /`tellraw`

> 向一个或多个玩家发送一条以文本组件表示的消息。

**加入版本：** 1.9.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 无 |

## 语法

```
tellraw <target: target> <raw json message: json>
```

## 参数详解

- **`target`**:CommandSelector<Player> - 指定该消息的接收玩家，必须为玩家名或目标选择器
- **`raw json message`**:Json::Value - 指定要发送的文本组件消息，必须为JSON对象。
