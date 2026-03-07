# /`spreadplayers`

> 把实体随机传送到区域内地表的某个位置。

**加入版本：** 1.0.5.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 在基岩版中，该命令仅更改实体的坐标，而不改变维度，但有效位置仍基于命令的执行维度判断。熔岩、水、气泡柱、火、岩浆块、凋灵玫瑰、营火、灵魂营火、甜浆果丛、下界传送门、末地传送门和末地折跃门上不是有效位置。 |

## 语法

```
spreadplayers <x: value> <z: value> <spreadDistance: float> <maxRange: float> <victim: target> [maxHeight: value]
```

## 参数详解

- **`x`**:value: RelativeFloat - 指定传送目的地区域的中心的x坐标
- **`z`**:value: RelativeFloat - 指定传送目的地区域的中心的z坐标
- **`spreadDistance`**:float: float - 指定传送目标之间的最小间距
- **`maxRange`**:float: float - 指定目标区域边界与区域中心在X和Z轴上的距离
- **`victim`**:target: CommandSelector<Actor> - 指定需要随机传送的目标
- **`maxHeight`**:value: RelativeFloat - 限制传送位置的最大高度
