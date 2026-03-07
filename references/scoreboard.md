# /`scoreboard`

> 管理记分板中的记分项和分数持有者。

**加入版本：** 1.7.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 在基岩版中，dummy是当前唯一支持的准则。 |

## 语法

```
scoreboard objectives list | scoreboard objectives add <objective: string> dummy [displayName: string] | scoreboard objectives remove <objective: string> | scoreboard objectives setdisplay <list|sidebar> [objective: string] [ascending|descending] | scoreboard objectives setdisplay belowname [objective: string] | scoreboard players list [playername: target] | scoreboard players set <player: target> <objective: string> <count: int> | scoreboard players add <player: target> <objective: string> <count: int> | scoreboard players remove <player: target> <objective: string> <count: int> | scoreboard players random <player: target> <objective: string> <min: int> <max: int> | scoreboard players reset <player: target> [objective: string] | scoreboard players test <player: target> <objective: string> <min: wildcard int> [max: wildcard int] | scoreboard players operation <player: target> <targetObjective: string> <operation: operator> <selector: target> <objective: string>
```

## 参数详解

- **`objective`**:string - 记分项的名称
- **`displayName`**:string - 记分项的显示名称
- list|sidebar|belowname - 显示位置
- ascending|descending - 排列顺序
- **`playername`**:target / player: target / selector: target - 分数持有者
- **`count`**:int - 分数
- **`min`**:int / max: int - 随机数范围
- **`min`**:wildcard int / max: wildcard int - 分数范围
- **`targetObjective`**:string - 目标记分项
- **`operation`**:operator - 算术操作
