# /`inputpermission`

> 对玩家的权限状态进行指定操作。

**加入版本：** 1.19.80

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 本条目所述内容仅适用于基岩版和教育版。 |

## 语法

```
inputpermission query <targets: target> <permission: permission> [state: state] | inputpermission set <targets: target> <permission: permission> <state: state>
```

## 参数详解

- **`targets`**:CommandSelector<Player> - 指定权限的拥有者。必须为玩家名或目标选择器。且要求目标选择器为玩家类型，若不是则在命令执行时会执行失败。
- **`permission`**:enum - 指定操作所作用的权限。必须为以下其中之一：camera, dismount, jump, lateral_movement, mount, move_backward, move_forward, move_left, move_right, movement, sneak
- **`state`**:enum - 指定权限的状态。必须为enabled（启用）或disabled（禁用）。
