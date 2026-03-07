# /`testforblock`

> 探测某个方块是否在特定位置。

**加入版本：** 0.16.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 在Java版中，该命令已被/execute if block取代。在基岩版1.19.70中移除了dataValue: int参数。 |

## 语法

```
testforblock <position: x y z> <tileName: Block> [blockStates: block states]
```

## 参数详解

- **`position`**:x y z: CommandPosition - 指定待探测的方块的坐标。必须为三维的坐标，格式为<X> <Y> <Z>，三个值必须是浮点数、相对坐标或局部坐标。不可超出正常游戏范围。
- **`tileName`**:Block: enum - 指定要探测的方块类型。必须为方块ID。
- **`blockStates`**:block states: BlockStateCommandParam - 指定要探测的方块状态。必须为格式为["<键1>"=<值1>,"<键2>"=<值2>,...]的方块状态。
