# /`time`

> 控制或查询世界的时间。

**加入版本：** 0.16.0 build 1

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 在1.17.30版本之前，/time set <amount: int> 是通过增加时间来达到指定的当日时间，之后则为直接设置。 |

## 语法

```
time add <amount: int> | time query <daytime|gametime|day> | time set <amount: int> | time set <time: TimeSpec>
```

## 参数详解

- **`amount`**:int - 指定要增加或设置的时间，必须为一个32位整数
- daytime|gametime|day - 指定要查询的数据，可选值为daytime（当日时间）、gametime（游戏时间）或day（游戏天数）
- **`time`**:TimeSpec - 指定要设置的时间节点，可选值为day (1000)、noon (6000)、sunset (12000)、night (13000)、midnight (18000)、sunrise (23000)
