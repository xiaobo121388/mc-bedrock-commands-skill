# /`structure`

> 用于在不使用结构方块的情况下保存或加载结构。

**加入版本：** 1.16.100.52

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 使用 /structure save 时，选定的区域不能大于64x384x64个方块。 |

## 语法

```
structure save <name: string> <from: x y z> <to: x y z> [saveMode: StructureSaveMode] | structure save <name: string> <from: x y z> <to: x y z> [includeEntities: Boolean] [saveMode: StructureSaveMode] [includeBlocks: Boolean] | structure load <name: string> <to: x y z> [rotation: Rotation] [mirror: Mirror] [includeEntities: Boolean] [includeBlocks: Boolean] [waterlogged: Boolean] [integrity: float] [seed: string] | structure load <name: string> <to: x y z> [rotation: Rotation] [mirror: Mirror] [animationMode: StructureAnimationMode] [animationSeconds: float] [includeEntities: Boolean] [includeBlocks: Boolean] [waterlogged: Boolean] [integrity: float] [seed: string] | structure delete <name: string>
```

## 参数详解

- **`name`**:string - 指定结构名称，格式为name或namespace:name
- **`from`**:x y z - 定义源区域的对角方块坐标
- **`to`**:x y z - 定义源区域的对角方块坐标或目标区域西北下角的坐标
- **`saveMode`**:StructureSaveMode - 指定结构的存储位置 (memory 或 disk)
- **`includeEntities`**:Boolean - 是否加载或保存实体
- **`includeBlocks`**:Boolean - 是否加载或保存方块
- **`rotation`**:Rotation - 指定结构旋转角度 (0_degrees, 90_degrees, 180_degrees, 270_degrees)
- **`mirror`**:Mirror - 指定结构的镜像模式 (none, x, z, xz)
- **`animationMode`**:StructureAnimationMode - 指定生成结构使用的动画 (block_by_block 或 layer_by_layer)
- **`animationSeconds`**:float - 指定动画的时长
- **`integrity`**:float - 指定结构的完整性 (0-100)
- **`seed`**:string - 指定随机种子
- **`waterlogged`**:Boolean - 指定生成的含水结构是否正确含水
