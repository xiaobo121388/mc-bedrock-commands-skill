# /`enchant`

> 为一个实体手持的物品添加魔咒。

**加入版本：** 0.16.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 受限于铁砧机制。 |

## 语法

```
enchant <player: target> <enchantmentId: int> [level: int] | enchant <player: target> <enchantmentName: Enchant> [level: int]
```

## 参数详解

- **`player`**:target: CommandSelector<Actor> - 指定目标，必须为玩家名或目标选择器
- **`enchantmentId`**:int - 指定魔咒，必须是一个魔咒的ID（无命名空间）
- **`enchantmentName`**:Enchant - 指定魔咒，必须是一个魔咒的ID（无命名空间）
- **`level`**:int - 指定魔咒的等级，不应大于最大等级，默认为1，必须大于等于1
