# /`gamerule`

> 设置或查询游戏规则。

**加入版本：** 1.0.5

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 仅对于某些规则需要启用作弊 |
| **额外说明** | 自基岩版1.8起，只有拥有管理员权限的玩家能够使用。不再接受自定义游戏规则。`alwaysday`/`daylock` 是独立命令，可用于锁定或解锁昼夜更替。 |

## 语法

```
gamerule
gamerule <rule: BoolGameRule> [value: Boolean]
gamerule <rule: IntGameRule> [value: int]
gamerule playerWaypoints <value: playerwaypointsValues>
```

不带参数时列出所有游戏规则。指定规则但省略 `value` 时查询该规则当前值。

> `playerWaypoints` 及其独立枚举语法为基岩版 26.30 新增内容。

## 参数详解

- **`rule`**: BoolGameRule / IntGameRule - enum - 指定要设置或查询的游戏规则。基岩版输入时不区分大小写，本文使用小驼峰命名。
- **`value`**: Boolean / int - 指定游戏规则的新值。布尔值为 `true` 或 `false`；整型值为有符号32位整数。
- **`value`**: playerwaypointsValues - enum - 仅用于 `playerWaypoints`，可为 `off` 或 `everyone`。

## 基岩版游戏规则

资料依据中文 Minecraft Wiki 的“游戏规则”和“命令/gamerule”页面整理。`UI位置` 按“经典UI / Ore UI”标注；`命令专用` 表示该规则不显示在对应编辑界面中，只能通过 `/gamerule` 修改。

| 规则ID | 类型 | 默认值 | UI位置 | 作用 |
|---|---|---:|---|---|
| `commandBlockOutput` | 布尔值 | `true` | 命令专用 | 命令方块执行命令时，是否在聊天框中向管理员显示输出。 |
| `commandBlocksEnabled` | 布尔值 | `true` | 作弊 / 无敌模式 | 命令方块是否启用并可运行。 |
| `doDaylightCycle` | 布尔值 | `true` | 作弊 / 无敌模式 | 是否进行昼夜更替和月相变化。 |
| `doEntityDrops` | 布尔值 | `true` | 作弊 / 无敌模式 | 非生物实体被破坏时是否掉落物品。 |
| `doFireTick` | 布尔值 | `true` | 世界选项 / 高级 | 火是否蔓延及自然熄灭。 |
| `doImmediateRespawn` | 布尔值 | `false` | 世界选项 / 高级 | 玩家死亡时是否跳过死亡界面并立即重生。 |
| `doInsomnia` | 布尔值 | `true` | 命令专用 | 幻翼是否会在夜晚生成。 |
| `doLimitedCrafting` | 布尔值 | `false` | 命令专用 | 玩家是否只能使用已解锁的配方合成。 |
| `doMobLoot` | 布尔值 | `true` | 世界选项 / 高级 | 生物死亡时是否掉落物品。 |
| `doMobSpawning` | 布尔值 | `true` | 作弊 / 无敌模式 | 生物是否自然生成；不影响刷怪笼和 `/summon`。 |
| `doTileDrops` | 布尔值 | `true` | 世界选项 / 高级 | 方块被破坏时是否掉落物品。 |
| `doWeatherCycle` | 布尔值 | `true` | 作弊 / 无敌模式 | 天气是否自然变化。 |
| `drowningDamage` | 布尔值 | `true` | 命令专用 | 玩家是否承受溺水伤害。 |
| `fallDamage` | 布尔值 | `true` | 命令专用 | 玩家是否承受摔落伤害。 |
| `fireDamage` | 布尔值 | `true` | 命令专用 | 玩家是否承受火焰伤害。 |
| `freezeDamage` | 布尔值 | `true` | 命令专用 | 玩家是否承受冰冻伤害。 |
| `functionCommandLimit` | 整型 | `10000` | 命令专用 | 单次 `/function` 可执行的最大命令数量。 |
| `keepInventory` | 布尔值 | `false` | 作弊 / 无敌模式 | 玩家死亡后是否保留物品栏物品和经验。 |
| `locatorBar` | 布尔值 | `true` | 世界选项 / 多人游戏 | 是否显示定位栏。 |
| `maxCommandChainLength` | 整型 | `65536` | 命令专用 | 连锁命令方块和函数可连锁执行的最大命令数量。 |
| `mobGriefing` | 布尔值 | `true` | 作弊 / 无敌模式 | 生物是否能进行破坏性行为、捡拾物品、寻找海龟蛋等；不影响TNT。 |
| `naturalRegeneration` | 布尔值 | `true` | 世界选项 / 高级 | 玩家饥饿值足够时是否自然恢复生命值。 |
| `playerWaypoints` | 枚举值 | `everyone` | 世界选项 / 多人游戏 | 控制玩家是否显示在定位栏上：`off` 为不显示，`everyone` 为所有玩家显示。 |
| `playersSleepingPercentage` | 整型 | `100` | 世界选项 / 高级 | 跳过夜晚所需的入睡玩家占比。`0` 表示1名玩家入睡即可跳过夜晚；大于 `100` 会阻止通过入睡跳过夜晚。 |
| `projectilesCanBreakBlocks` | 布尔值 | `true` | 命令专用 | 弹射物是否能破坏其可破坏的方块，如紫颂花、滴水石锥和饰纹陶罐。 |
| `pvp` | 布尔值 | `true` | 世界选项 / 多人游戏 | 玩家之间是否能互相造成伤害。 |
| `randomTickSpeed` | 整型 | `3` | 作弊 / 无敌模式 | 每游戏刻每区段中随机方块刻的频率；`0` 会禁用随机刻。 |
| `recipesUnlock` | 布尔值 | `true` | 世界选项 / 高级 | 配方是否会随材料收集而解锁。 |
| `respawnBlocksExplode` | 布尔值 | `true` | 世界选项 / 高级 | 在不兼容维度使用床或重生锚时是否爆炸。 |
| `sendCommandFeedback` | 布尔值 | `true` | 命令专用 | 玩家执行命令的反馈是否显示在聊天框中，并影响命令方块是否保存输出文本。 |
| `showBorderEffect` | 布尔值 | `true` | 命令专用 | 世界边界是否显示红色粒子效果。 |
| `showCoordinates` | 布尔值 | `true` | 世界选项 / 高级 | 是否持续显示玩家坐标。 |
| `showDaysPlayed` | 布尔值 | `false` | 世界选项 / 高级 | 是否显示世界中的游玩天数。 |
| `showDeathMessages` | 布尔值 | `true` | 命令专用 | 是否在聊天框中显示玩家死亡消息，并影响宠物死亡通知。 |
| `showRecipeMessages` | 布尔值 | `true` | 命令专用 | 解锁新配方时是否显示消息。 |
| `showTags` | 布尔值 | `true` | 命令专用 | 是否显示物品的物品组件信息。 |
| `spawnRadius` | 整型 | `10` | 世界选项 / 高级 | 没有自定义重生点的玩家，围绕世界出生点随机重生的半径。经典UI最大值为 `128`。 |
| `tntExplodes` | 布尔值 | `true` | 世界选项 / 高级 | TNT是否会爆炸。 |
| `tntExplosionDropDecay` | 布尔值 | `false` | 命令专用 | TNT爆炸破坏的方块是否会有概率不掉落。 |

## 常用示例

```
gamerule
gamerule doDaylightCycle false
gamerule keepInventory true
gamerule mobGriefing false
gamerule randomTickSpeed 3
gamerule spawnRadius 25
gamerule pvp false
gamerule playerWaypoints off
```
