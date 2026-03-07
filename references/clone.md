# /`clone`

> 在指定区域之间复制方块结构。

**加入版本：** 0.16.0 (携带版Alpha)

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 源区域被选中的方块数量不能超过655360。 |

## 语法

```
clone <begin: x y z> <end: x y z> <destination: x y z> [maskMode: MaskMode] | clone <begin: x y z> <end: x y z> <destination: x y z> <maskMode: MaskMode> [cloneMode: CloneMode] | clone <begin: x y z> <end: x y z> <destination: x y z> filtered <cloneMode: CloneMode> <tileName: Block> [blockStates: block states]
```

## 参数详解

- **`begin`**:x y z: CommandPosition - 定义源区域的对角方块坐标
- **`end`**:x y z: CommandPosition - 定义源区域的另一个对角方块坐标
- **`destination`**:x y z: CommandPosition - 定义目标区域西北方向较低点的坐标
- **`maskMode`**:MaskMode - 指定过滤模式，可选值为 masked (仅复制非空气方块) 或 replace (复制所有方块)
- **`cloneMode`**:CloneMode - 指定克隆模式，可选值为 force (强制复制), move (移动) 或 normal (普通)
- **`tileName`**:Block - 在filtered模式下指定要复制的方块ID
- **`blockStates`**:block states - 指定复制时需要符合的方块状态
