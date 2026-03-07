# /`hud`

> 修改HUD的可见性。

**⚠️ 注意：该指令在 1.20.60.23 版本加入，属于 1.20.50 之后的较新指令。**

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 本条目所述内容仅适用于基岩版和​教育版。 |

## 语法

```
hud <target: target> <visible: HudVisibility> [hud_element: HudElement]
```

## 参数详解

- **`target`**:CommandSelector<Player> - 指定将被修改HUD可见性的目标。必须为玩家名或目标选择器。且要求目标选择器为玩家类型，若不是则在命令执行时会执行失败。
- **`visible`**:HudVisibility - 指定将对HUD可见性做出的修改。必须为`hide`（隐藏）或`reset`（重置）。
- **`hud_element`**:HudElement - 指定将被修改的HUD元素。必须为以下之一：`air_bubbles`、`all`、`armor`、`crosshair`、`health`、`horse_health`、`hotbar`、`hunger`、`item_text`、`paperdoll`、`progress_bar`、`status_effects`、`tooltips`、`touch_controls`。如果未指定，默认为`all`。
