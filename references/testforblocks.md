# /`testforblocks`

> 测试两个区域中的方块是否相同。

**加入版本：** 0.16.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 在Java版1.13中被/execute if blocks取代。 |

## 语法

```
testforblocks <begin: x y z> <end: x y z> <destination: x y z> [masked|all]
```

## 参数详解

- **`begin`**:x y z 与 end: x y z: 指定作为样式基准的区域（源区域）的两个对角方块
- **`destination`**:x y z: 指定待检查区域（目标区域）的下西北角（具有最小坐标值的边角）
- **`masked|all`**:指定测试模式，all表示两个区域的所有方块必须完全相同，masked表示源区域的空气方块可匹配目标区域的任意方块，默认为all
