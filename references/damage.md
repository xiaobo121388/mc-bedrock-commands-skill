# /`damage`

> 对指定实体造成指定类型的伤害。

**加入版本：** 1.18.10

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 无 |

## 语法

```
damage <target: target> <amount: int> <cause: DamageCause> entity <damager: target> | damage <target: target> <amount: int> [cause: DamageCause]
```

## 参数详解

- **`target`**:CommandSelector<Actor> - 指定要被伤害的目标实体，必须为玩家名或目标选择器
- **`amount`**:int - 指定要造成的伤害值，必须为32位整数
- **`cause`**:DamageCause - 指定伤害的成因，默认为none，必须为单个词的字符串
- **`damager`**:target - 指定伤害的直接来源，必须为玩家名或目标选择器
