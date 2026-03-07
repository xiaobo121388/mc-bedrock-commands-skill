# /`tag`

> 管理单个实体的记分板标签。

**加入版本：** 1.9.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 无 |

## 语法

```
tag <entity: target> add <name: string> | tag <entity: target> remove <name: string> | tag <entity: target> list
```

## 参数详解

- **`entity`**:target: WildcardCommandSelector<Actor> - 指定要操作的实体目标，必须为一个目标选择器、一个玩家名，或者用一个*来代表所有正被记分板跟踪的实体。
- **`name`**:string: basic_string - 指定要被添加或被移除的标签名称，必须为单个词或者双引号（"）括起的字符串。引号内的字符可以使用\进行转义。
