# /`loot`

> 将指定的战利品放入物品栏或世界。

**加入版本：** 1.18.0.21

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | mine语法在1.21.50.20版本中作为实验性玩法加入，在1.21.60.23版本中不再属于实验性玩法。 |

## 语法

```
loot give <player: target> kill <entity: target> ["<tool>|mainhand|offhand": string] | loot give <player: target> loot <loot_table: string> ["<tool>|mainhand|offhand": string] | loot give <player: target> mine <TargetBlockPosition: x y z> ["<tool>|mainhand|offhand": string] | loot insert <position: x y z> kill <entity: target> ["<tool>|mainhand|offhand": string] | loot insert <position: x y z> loot <loot_table: string> ["<tool>|mainhand|offhand": string] | loot insert <position: x y z> mine <TargetBlockPosition: x y z> ["<tool>|mainhand|offhand": string] | loot spawn <position: x y z> kill <entity: target> ["<tool>|mainhand|offhand": string] | loot spawn <position: x y z> loot <loot_table: string> ["<tool>|mainhand|offhand": string] | loot spawn <position: x y z> mine <TargetBlockPosition: x y z> ["<tool>|mainhand|offhand": string] | loot replace block <position: x y z> slot.container <slotId: int> [count: int] kill <entity: target> ["<tool>|mainhand|offhand": string] | loot replace block <position: x y z> slot.container <slotId: int> [count: int] loot <loot_table: string> ["<tool>|mainhand|offhand": string] | loot replace block <position: x y z> slot.container <slotId: int> [count: int] mine <TargetBlockPosition: x y z> ["<tool>|mainhand|offhand": string] | loot replace entity <entity: target> <slotType: EntityEquipmentSlot> <slotId: int> [count: int] kill <entity: target> ["<tool>|mainhand|offhand": string] | loot replace entity <entity: target> <slotType: EntityEquipmentSlot> <slotId: int> [count: int] loot <loot_table: string> ["<tool>|mainhand|offhand": string] | loot replace entity <entity: target> <slotType: EntityEquipmentSlot> <slotId: int> [count: int] mine <TargetBlockPosition: x y z> ["<tool>|mainhand|offhand": string]
```

## 参数详解

- **`loot_table`**:string - 指定所使用的战利品表
- **`"<tool>|mainhand|offhand"`**:string - 指定用来模拟杀死生物或获取战利品的工具
- **`entity`**:target: CommandSelector<Actor> - 指定要模拟杀死的实体
- **`player`**:target: CommandSelector<Player> - 指定要给予物品的一个或多个玩家
- **`TargetBlockPosition`**:x y z: CommandPositionFloat - 指定方块坐标
- **`position`**:x y z: CommandPositionFloat - 指定方块坐标
- **`entity`**:target: CommandSelector<Actor> - 指定要修改的一个或多个实体
- **`count`**:int: int - 指定要清空并放入物品的连续槽位数
- **`slotType`**:EntityEquipmentSlot: enum - 指定要修改的物品栏槽位
- **`slot.container`**:- 指定要修改的物品栏槽位
- **`slotId`**:int: int - 指定要修改的物品栏槽位。
