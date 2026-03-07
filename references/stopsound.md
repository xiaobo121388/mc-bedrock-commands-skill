# /`stopsound`

> 停止声音事件播放。

**加入版本：** 1.0.5.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 无 |

## 语法

```
stopsound <player: target> [sound: string]
```

## 参数详解

- **`player`**:target: CommandSelector<Player> - 指定声音的接收者。必须为玩家名或目标选择器
- **`sound`**:string - 指定要停止的声音。若未指定，则停止所有声音。必须为单个词或者双引号括起的字符串。应为一个声音事件（例如，mob.pig.say）。
