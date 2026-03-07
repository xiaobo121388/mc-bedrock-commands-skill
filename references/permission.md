# /`permission`

> 枚举或重新加载权限列表，或设置玩家的权限等级。

**加入版本：** 1.10.0

| 属性 | 值 |
|---|---|
| **别名** | `ops` |
| **权限等级** | 4 |
| **需要作弊** | 是 |
| **额外说明** | permission list 和 permission reload 仅BDS可用。permission set 仅非BDS可用，但通常无法执行，因为其权限等级要求过高。 |

## 语法

```
permission list | permission reload | permission set <player: target> [permission: PermissionLevel]
```

## 参数详解

- **`player`**:target: CommandSelector<Player> - 必须为玩家名或目标选择器。
- **`permission`**:PermissionLevel: enum - 指定权限等级所对应的身份，必须为以下其中之一：member、operator、visitor。
