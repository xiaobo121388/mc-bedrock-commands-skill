# /`ride`

> 用于使实体骑乘或停止骑乘其他实体。在基岩版中，某些实体不允许其他实体对其进行骑乘，主要是靠数据驱动。可通过行为包文件中的`minecraft:rideable`组件来控制。

**加入版本：** 1.16.100

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 在基岩版中，某些实体不允许其他实体对其进行骑乘，主要是靠数据驱动。可通过行为包文件中的`minecraft:rideable`组件来控制。 |

## 语法

```
ride <riders: target> start_riding <ride: target> [teleportRules: TeleportRules] [howToFill: FillType] | ride <riders: target> stop_riding | ride <rides: target> evict_riders | ride <rides: target> summon_rider <entityType: EntityType> [spawnEvent: string] [nameTag: string] | ride <riders: target> summon_ride <entityType: EntityType> [rideRules: RideRules] [spawnEvent: string] [nameTag: string]
```

## 参数详解

- **`riders`**:target: CommandSelector<Actor> - 指定乘客。如果处于start_riding模式并且teleportRules: TeleportRules是teleport_ride时，应仅有一个实体。必须为玩家名或目标选择器。
- **`ride`**:target: CommandSelector<Actor> - 指定坐骑。应仅有一个实体。必须为玩家名或目标选择器。
- **`rides`**:target: CommandSelector<Actor> - 指定坐骑。必须为玩家名或目标选择器。
- **`teleportRules`**:TeleportRules: enum - 指定将被传送的实体。必须是teleport_ride（传送坐骑至乘客）或teleport_rider（传送乘客至坐骑）。如果未指定，默认为teleport_rider。
- **`howToFill`**:FillType: enum - 必须是if_group_fits或until_full。if_group_fits只会在指定的所有<riders: target>都能一起骑上指定的坐骑时才会使它们骑乘。until_full让指定的<riders: target>逐个尝试骑乘至指定的坐骑上，直到该坐骑满载。如果未指定，默认为until_full。
- **`entityType`**:EntityType: enum - 指定召唤的实体。必须是一个实体类型的ID。只有特定实体类型允许被召唤。允许召唤的实体类型可见于命令的自动补全建议列表。指定列表外的实体类型会是命令无法解析。
- **`spawnEvent`**:string: basic_string - 指定实体生成时执行的事件。应为一个生成事件（行为包中的实体事件）的名称。
- **`nameTag`**:string: basic_string - 指定实体生成时的名字。必须为 字符串。必须为单个词或者双引号（"）括起的字符串。引号内的字符可以使用\进行转义。
- **`rideRules`**:RideRules: enum - 必须是no_ride_change， reassign_rides或 skip_riders。skip_riders仅为没有在骑乘的<riders: target>召唤实体。no_ride_change仅为没有骑乘且没有被骑乘的<riders: target>召唤实体。reassign_rides使正在骑乘的<riders: target>停止骑乘，然后为所有<riders: target>召唤实体。如果未指定，默认为reassign_rides。
