# /`give`

> 给予玩家指定数量的物品。

**加入版本：** 0.16.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 无 |

## 语法

```
give <player: target> <itemName: Item> [amount: int] [data: int] [components: json]
```

## 参数详解

- **`player`**:target: CommandSelector<Player> - 必须为玩家名或目标选择器
- **`itemName`**:Item: CommandItem - 指定给予的物品，必须为物品ID或存在其物品形式的方块ID
- **`amount`**:int: int - 指定给予的物品数量，范围为1-32767，若未指定则默认为1
- **`data`**:int: int - 指定所给予物品的数据值，范围为0-32767，若未指定则默认为0
- **`components`**:json: Json::Value - 指定所给予物品的物品堆叠组件，必须为JSON对象
