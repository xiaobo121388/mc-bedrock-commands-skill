# /`dialogue`

> 为玩家打开或改变NPC的对话框。

**加入版本：** 1.17.10

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 本条目所述内容仅适用于基岩版和​教育版。 |

## 语法

```
dialogue open <npc: target> <player: target> [sceneName: string] | dialogue change <npc: target> <sceneName: string> [players: target]
```

## 参数详解

- **`npc`**:target: CommandSelector<Actor> - 指定要打开或改变的NPC目标。必须为玩家名或目标选择器。且必须为单个NPC。
- **`sceneName`**:string: basic_string - 指定从导入的行为包中对话文件显示的场景。必须为字符串。必须为单个词或者双引号（“）括起的字符串。引号内的字符可以使用\进行转义。
- **`player`**:target: CommandSelector<Player> - 指定打开NPC对话框的目标玩家，必须为玩家名或目标选择器。且要求目标选择器为玩家类型，若不是则在命令执行时会执行失败。
