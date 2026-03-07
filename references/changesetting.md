# /`changesetting`

> 在基岩版专用服务器（BDS）上运行时更改服务器设置。

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 4 |
| **需要作弊** | 否 |
| **额外说明** | 只能在BDS控制台运行，仅适用于基岩版专用服务器。 |

## 语法

```
changesetting allow-cheats <value: Boolean> | changesetting difficulty <value: Difficulty> | changesetting difficulty <value: int>
```

## 参数详解

- **`value`**:Difficulty/int - 指定一个新的难度，必须是以下之一：peaceful (p, 0), easy (e, 1), normal (n, 2), hard (h, 3)
- **`value`**:Boolean - 指定服务器是否允许作弊，必须是布尔值 (true 或 false)
