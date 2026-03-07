# /`aimassist`

> 修改玩家的瞄准辅助。

**⚠️ 注意：该指令在 1.21.50 版本加入，属于 1.20.50 之后的较新指令。**

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 本条目所述内容仅适用于基岩版和​教育版。在1.21.70版本前为实验性玩法。 |

## 语法

```
aimassist <players: target> clear | aimassist <players: target> set [x angle: float] [y angle: float] [max distance: float] [target mode: AimAssistTargetMode] [preset id: string]
```

## 参数详解

- **`players`**:target: CommandSelector<Player> - 指定将被修改瞄准辅助的玩家，必须为玩家名或目标选择器
- **`x angle`**:float - 指定X轴角度，默认为50，必须在10和90之间
- **`y angle`**:float - 指定Y轴角度，默认为50，必须在10和90之间
- **`max distance`**:float - 指定最大距离，默认为8，必须在1和16之间
- **`target mode`**:AimAssistTargetMode - 指定瞄准模式，默认为angle，可选值为angle或distance
- **`preset id`**:string - 指定预设ID
