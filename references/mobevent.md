# /`mobevent`

> 控制或查询允许运行的生物事件。

**加入版本：** 1.11.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 本条目所述内容仅适用于基岩版和​教育版。 |

## 语法

```
mobevent <event: MobEvent> [value: Boolean]
```

## 参数详解

- **`event`**:MobEvent - 指定要控制或查询的事件。可以是以下之一：minecraft:ender_dragon_event, minecraft:pillager_patrols_event, minecraft:wandering_trader_event, events_enabled
- **`value`**:Boolean - 如果指定，则true启用事件，false禁用事件。如果忽略，则显示当前启用状态。
