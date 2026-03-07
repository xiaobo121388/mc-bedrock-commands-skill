# /`recipe`

> 给予或剥夺（解锁或锁定）玩家的配方。

**加入版本：** 1.20.10.21 (实验性玩法), 1.20.30 (正式版)

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 在基岩版中，<recipe: string>参数必须为一个配方的ID，命名空间不可省略（如果有）或添加（如果没有）。 |

## 语法

```
recipe give <player: target> * | recipe give <player: target> "*" | recipe take <player: target> * | recipe take <player: target> "*" | recipe give <player: target> <recipe: string> | recipe take <player: target> <recipe: string>
```

## 参数详解

- **`player`**:target: CommandSelector<Player> - 指定要给予或剥夺配方的玩家，必须为玩家名或目标选择器
- **`recipe`**:string: basic_string - 指定要给予或剥夺的配方，必须为一个配方的ID。
