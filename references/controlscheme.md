# /`controlscheme`

> 修改相机预设的控制方案。

**⚠️ 注意：该指令在 1.21.80.27 版本加入，属于 1.20.50 之后的较新指令。**

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 此命令需与/camera命令一同使用。 |

## 语法

```
controlscheme <players: target> clear | controlscheme <players: target> set <control scheme: controlscheme>
```

## 参数详解

- **`players`**:target: CommandSelector<Player> - 指定要被修改控制方案的玩家。必须为玩家名或目标选择器。且要求目标选择器为玩家类型，若不是则在命令执行时会执行失败。
- **`control scheme`**:controlscheme: Enum - 指定控制方案。必须为字符串，且必须为单个词。必须为以下其中之一：camera_relative, camera_relative_strafe, locked_player_relative_strafe, player_relative, player_relative_strafe
