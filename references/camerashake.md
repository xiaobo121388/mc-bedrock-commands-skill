# /`camerashake`

> 对玩家视野施以一定强度和时间的摇晃效果。

**加入版本：** 1.16.100

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 本条目所述内容仅适用于基岩版和​教育版。若玩家在无障碍设置中禁用了视角摇晃，则不会看到此效果。 |

## 语法

```
camerashake add <player: target> [intensity: float] [seconds: float] [shakeType: CameraShakeType] | camerashake stop [player: target]
```

## 参数详解

- **`player`**:target: CommandSelector<Player> - 必须为玩家名或目标选择器，如果未指定，默认为命令执行者
- **`intensity`**:float: float - 必须是0到4以内的单精度浮点数，指定视野摇晃的强度
- **`seconds`**:float: float - 单精度浮点数，指定视野摇晃的时长（秒）
- **`shakeType`**:CameraShakeType: CameraShakeType - 必须为positional（坐标摇晃）或rotational（角度摇晃），指定视野摇晃的种类
