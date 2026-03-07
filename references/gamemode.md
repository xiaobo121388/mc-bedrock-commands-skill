# /`gamemode`

> 设置玩家的游戏模式。

**加入版本：** 0.16.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 在基岩版中，游戏模式参数可以使用简写，如s, c, a, d，或者使用数字0, 1, 2, 5。 |

## 语法

```
gamemode <gameMode: GameMode> [player: target] | gamemode <gameMode: int> [player: target]
```

## 参数详解

- **`gameMode`**:GameMode / int - 指定玩家的新游戏模式，必须为以下其中之一：survival (s 或 0), creative (c 或 1), adventure (a 或 2), default (d 或 5), spectator
- **`player`**:target - 指定要被修改游戏模式的玩家。如果未指定，默认为命令执行者。必须为玩家名或目标选择器。
