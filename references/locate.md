# /`locate`

> 在聊天框中为命令执行者显示给定的结构、生物群系的最近坐标。

**加入版本：** 1.0.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 无 |

## 语法

```
locate biome <biome: Biome> | locate structure <structure: Structure> [useNewChunksOnly: Boolean]
```

## 参数详解

- **`biome`**:Biome - 指定要定位的生物群系的命名空间ID（1.21.100 起必须包含命名空间，如 `minecraft:plains`）
- **`structure`**:Structure - 指定要定位的结构的命名空间ID
- **`useNewChunksOnly`**:Boolean - 仅定位在尚未生成的区块中的结构，默认为false，必须为布尔值（true或false）。
