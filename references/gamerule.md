# /`gamerule`

> 设置或查询游戏规则。

**加入版本：** 1.0.5

| 属性 | 值 |
|---|---|
| **别名** | `daylock,alwaysday` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 仅对于某些规则需要启用作弊。自基岩版1.8起，只有拥有管理员权限的玩家能够使用。不再接受自定义游戏规则。 |

## 语法

```
gamerule | gamerule <rule: BoolGameRule> [value: Boolean] | gamerule <rule: IntGameRule> [value: int]
```

## 参数详解

- **`rule`**:BoolGameRule/IntGameRule - enum - 指定要设置或查询的游戏规则
- **`value`**:Boolean/int - 指定将游戏规则设置的值
