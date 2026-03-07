# /`fog`

> 用于更改玩家的迷雾效果。

**加入版本：** 1.16.100

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 仅适用于基岩版和教育版 |

## 语法

```
fog <victim: target> push <fogId: string> <userProvidedId: string> | fog <victim: target> <mode: delete> <userProvidedId: string>
```

## 参数详解

- **`victim`**:target - 指定修改玩家迷雾效果的目标，必须为一个玩家名或目标选择器
- **`fogId`**:string - 指定修改的迷雾ID
- **`userProvidedId`**:string - 指定迷雾设置的名称，包含空格的值必须用英文双引号括起来
- **`mode`**:delete - 必须为pop或remove，指定是只移除第一个还是移除所有名称为<userProvidedId: string>的迷雾
