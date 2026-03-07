# /`setblock`

> 将指定位置的方块更改为另一个方块。

**加入版本：** 0.16.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 无 |

## 语法

```
setblock <position: x y z> <tileName: Block> [blockStates: block states] [destroy|keep|replace]
```

## 参数详解

- **`position`**:x y z: CommandPosition - 指定要被更改方块的位置，格式为<X> <Y> <Z>，三个值必须是浮点数、相对坐标或局部坐标
- **`tileName`**:Block: Block - 指定更改后的新方块，必须为方块ID
- **`blockStates`**:block states: BlockStateCommandParam - 指定新方块的方块状态，格式为["<键1>"=<值1>,"<键2>"=<值2>,...]
- **`destroy|keep|replace`**:- 指定方块更改的处理方式，destroy为破坏原方块并掉落物品，keep为仅在原方块为空气时才放置，replace为直接替换且不掉落物品
