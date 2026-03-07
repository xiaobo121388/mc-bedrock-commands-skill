# /`place`

> 以指定位置为生成原点，放置地物、结构地物、结构模板或结构池。

**⚠️ 注意：该指令在 1.21.50.26 (实验性玩法) 版本加入，属于 1.20.50 之后的较新指令。**

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 2 |
| **需要作弊** | 是 |
| **额外说明** | jigsaw和structure子命令在1.21.80.22版本后不再属于实验性玩法。feature和featurerule子命令在1.21.70.22版本后不再属于实验性玩法。 |

## 语法

```
place feature <feature: features> [position: x y z] | place featurerule <featurerule: featureRules> [position: x y z] | place jigsaw <pool: filepath> <jigsawTarget: string> <maxDepth: int> [pos: x y z] [keepJigsaws: Boolean] [includeEntities: Boolean] [liquidSettings: LiquidSettings] | place structure <structure: string> [pos: x y z] [ignoreStartHeight: Boolean] [keepJigsaws: Boolean] [includeEntities: Boolean] [liquidSettings: LiquidSettings]
```

## 参数详解

- **`feature`**:features - 指定地物
- **`position`**:x y z - 指定放置时使用的生成原点
- **`featurerule`**:featureRules - 指定地物规则
- **`pool`**:filepath - 指定要放置的结构池
- **`jigsawTarget`**:string - 指定放置结构池时的结构中的起始拼图方块
- **`maxDepth`**:int - 指定要展开拼图方块的最大深度，必须在1和7之间（含）
- **`pos`**:x y z - 指定放置时使用的生成原点
- **`keepJigsaws`**:Boolean - 指定被放置结构是否保留拼图方块，默认为false
- **`includeEntities`**:Boolean - 指定被放置结构是否包含实体，默认为false
- **`liquidSettings`**:LiquidSettings - 指定流体处理方式，默认为apply_waterlogging
- **`structure`**:string - 指定要放置的结构地物，只能为 minecraft:trail_ruins 或 minecraft:trial_chambers
- **`ignoreStartHeight`**:Boolean - 指定放置结构时是否忽略起始高度，默认为false
