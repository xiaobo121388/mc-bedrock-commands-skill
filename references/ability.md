# /`ability`

> 赋予或剥夺玩家的能力。

**加入版本：** 0.16.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 该特性仅在教育版和开启了“Education Edition”选项的基岩版世界中可用。 |

## 语法

```
ability <player: target> <ability: Ability> <value: Boolean> | ability <player: target> [ability: Ability]
```

## 参数详解

- **`player`**:target: CommandSelector<Player> - 指定要赋予或剥夺能力的玩家。必须为玩家名或目标选择器
- **`ability`**:Ability: enum - 指定要操作的能力，可选值为 worldbuilder、mayfly、mute
- **`value`**:Boolean: enum - 指定此能力是否对玩家可用，必须为布尔值（true或false）
