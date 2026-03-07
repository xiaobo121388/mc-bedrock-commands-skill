# /`title`

> 控制屏幕标题。

**加入版本：** 1.0.5.0

| 属性 | 值 |
|---|---|
| **别名** | `titleraw` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | titleraw是用于显示JSON格式文本的变体。 |

## 语法

```
title <player: target> <clear|reset> | title <player: target> <title|subtitle|actionbar> <titleText: message> | title <player: target> times <fadeIn: int> <stay: int> <fadeOut: int> | titleraw <player: target> <clear|reset> | titleraw <player: target> <titleLocation: TileRawSet> <raw json titleText: json> | titleraw <player: target> times <fadeIn: int> <stay: int> <fadeOut: int>
```

## 参数详解

- **`player`**:target: CommandSelector<Player> - 指定要显示屏幕标题的玩家
- **`titleText`**:message: CommandMessage - 指定标题、副标题、动作栏上方要显示的文本
- **`raw json titleText`**:json: Json::Value - 指定标题、副标题、动作栏上方要显示的JSON格式文本
- **`fadeIn`**:int: int - 指定屏幕标题的淡入时间（游戏刻）
- **`stay`**:int: int - 指定屏幕标题的持续时间（游戏刻）
- **`fadeOut`**:int: int - 指定屏幕标题的淡出时间（游戏刻）
- **`titleLocation`**:TileRawSet: enum - 指定屏幕标题的类型，可为actionbar、subtitle或title
