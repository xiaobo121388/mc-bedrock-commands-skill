# /`replaceitem`

> 替换方块（箱子、熔炉等）或实体（玩家或生物）物品栏内的物品。

**加入版本：** 1.0.5.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 在1.16.0版本中加入了destroy和keep两个新的替换模式。 |

## 语法

```
replaceitem block <position: x y z> slot.container <slotId: int> <itemName: Item> [amount: int] [data: int] [components: json] | replaceitem block <position: x y z> slot.container <slotId: int> <oldItemHandling: ReplaceMode> <itemName: Item> [amount: int] [data: int] [components: json] | replaceitem entity <target: target> <slotType: EntityEquipmentSlot> <slotId: int> <itemName: Item> [amount: int] [data: int] [components: json] | replaceitem entity <target: target> <slotType: EntityEquipmentSlot> <slotId: int> <oldItemHandling: ReplaceMode> <itemName: Item> [amount: int] [data: int] [components: json]
```

## 参数详解

- **`position`**:x y z - (仅block模式)指定要改变的方块的位置。可用波浪号（~ ~ ~）或脱字符（^ ^ ^）来指定一个相对于命令执行处的位置。
- **`target`**:target - (仅entity模式)指定要改变的实体。必须为一个玩家名或目标选择器。
- **`slotType`**:EntityEquipmentSlot, slot.container, slotId: int - 指定要改变的物品栏槽位。有效值取决于要改变的方块或实体。
- **`itemName`**:Item - 指定被放置于方块或实体的物品栏槽位内的物品。必须为物品ID。
- **`amount`**:int - (可选)指定被放置物品的数量。必须在1至64间（含），可以突破物品的堆叠限制。
- **`data`**:int - (可选)指定被放置物品的物品数据。必须为一个在-2,147,483,648至2,147,483,647间（含，不输入逗号）的整数，且在对指定物品无效时被重置为0。若未指定，默认为0。
- **`components`**:json - (可选)指定被放置物品的物品堆叠组件。类似于NBT标签，但仅支持minecraft:can_place_on、minecraft:can_destroy、minecraft:item_lock、minecraft:keep_on_death。
- **`oldItemHandling`**:ReplaceMode - (可选)必须是下列之一：destroy - 忽略指定槽位中的原始物品，直接进行替换。keep - 如果一个物品占用了该槽位，则不进行替换。
