# /`fill`

> 用特定方块填充一个区域的全部或部分。

**加入版本：** 携带版Alpha 0.16.0 build 1

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 无 |

## 语法

```
fill <from: x y z> <to: x y z> <tileName: Block> <blockStates: block states> [oldBlockHandling: FillMode] | fill <from: x y z> <to: x y z> <tileName: Block> [oldBlockHandling: FillMode] | fill <from: x y z> <to: x y z> <tileName: Block> <blockStates: block states> replace [replaceTileName: Block] [replaceBlockStates: block states] | fill <from: x y z> <to: x y z> <tileName: Block> replace [replaceTileName: Block] [replaceBlockStates: block states]
```

## 参数详解

- **`from`**:x y z: CommandPosition - 定义填充区域的起始点坐标
- **`to`**:x y z: CommandPosition - 定义填充区域的结束点坐标
- **`tileName`**:Block - 指定用于填充该区域的方块
- **`blockStates`**:block states - 指定方块要使用的方块状态
- **`oldBlockHandling`**:FillMode - 指定方块更改的处理方式，可选值为 destroy, hollow, outline, keep, replace
- **`replaceTileName`**:Block - （当oldBlockHandling为replace时）指定将要替换的方块
- **`replaceBlockStates`**:block states - （当oldBlockHandling为replace时）指定要替换的方块的方块状态
