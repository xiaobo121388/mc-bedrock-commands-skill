# /`tickingarea`

> 添加、移除、列出或预加载常加载区域。

**加入版本：** 1.2.0.2

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 最多可以定义10个常加载区域。 |

## 语法

```
tickingarea add <from: x y z> <to: x y z> [name: string] [preload: Boolean] | tickingarea add circle <center: x y z> <radius: int> [name: string] [preload: Boolean] | tickingarea remove <position: x y z> | tickingarea remove <name: string> | tickingarea remove_all | tickingarea preload <name: string> [preload: Boolean] | tickingarea preload <position: x y z> [preload: Boolean] | tickingarea list [all-dimensions: AllDimensions]
```

## 参数详解

- **`from`**:x y z: CommandPosition - 指定用于定义矩形常加载区域的两个对角坐标
- **`to`**:x y z: CommandPosition - 指定用于定义矩形常加载区域的两个对角坐标
- **`center`**:x y z: CommandPosition - 指定用于定义圆形常加载区域的圆心的坐标
- **`radius`**:int - 指定圆形常加载区域的半径作为从中心到圆周的区块数，范围为1到4
- **`name`**:string - 指定常加载区域的可选名称
- **`position`**:x y z: CommandPosition - 指定要选择的常加载区域所包含的坐标
- **`preload`**:Boolean - 指定常加载区域是否预加载 (true/false)
- **`all-dimensions`**:AllDimensions - 指定是否列出所有维度中的常加载区域
