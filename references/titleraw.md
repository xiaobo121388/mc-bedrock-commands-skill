# /`titleraw`

> 控制屏幕标题。

**加入版本：** 1.9.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 无 |

## 语法

```
titleraw <player: target> <clear|reset> | titleraw <player: target> <titleLocation: TileRawSet> <raw json titleText: json> | titleraw <player: target> times <fadeIn: int> <stay: int> <fadeOut: int>
```

## 参数详解

- **`player`**:target: CommandSelector<Player> - 指定要显示屏幕标题的玩家，必须为玩家名或目标选择器
- **`titleLocation`**:TileRawSet - 指定屏幕标题的类型，必须为actionbar、subtitle或title
- **`raw json titleText`**:json: Json::Value - 指定标题、副标题、动作栏上方要显示的文本，必须为JSON对象
- **`fadeIn`**:int: int - 指定屏幕标题淡入时间的时长，单位为游戏刻，小于0的值将被视为0
- **`stay`**:int: int - 指定屏幕标题持续显示时间的时长，单位为游戏刻，小于0的值将被视为0
- **`fadeOut`**:int: int - 指定屏幕标题淡出时间的时长，单位为游戏刻，小于0的值将被视为0
