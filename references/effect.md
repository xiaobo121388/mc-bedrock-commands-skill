# /`effect`

> 管理玩家及其他实体上的状态效果。

**加入版本：** 1.0.5.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 在1.21.40.20版本中加入了无限时长的语法和移除特定效果的语法。 |

## 语法

```
effect <player: target> <effect: Effect> [seconds: int] | effect <player: target> <effect: Effect> <seconds: int> [amplifier: int] | effect <player: target> <effect: Effect> <seconds: int> <amplifier: int> [hideParticles: Boolean] | effect <player: target> <effect: Effect> infinite [amplifier: int] [hideParticles: Boolean] | effect <player: target> clear [effect: Effect]
```

## 参数详解

- **`player`**:target: CommandSelector<Actor> - 指定目标，必须为玩家名或目标选择器
- **`effect`**:Effect - 指定要给予或移除的状态效果ID
- **`seconds`**:int - 指定效果时长，以秒为单位，可设为infinite表示无限
- **`amplifier`**:int - 指定效果的放大倍率，范围为0-255
- **`hideParticles`**:Boolean - 是否隐藏效果粒子。
