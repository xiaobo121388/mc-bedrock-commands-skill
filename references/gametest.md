# /`gametest`

> 管理和运行游戏测试框架。

**加入版本：** 1.16.210.60

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 在1.19.40版本之前，该指令属于实验性玩法。 |

## 语法

```
gametest runthis | gametest run <testName: string> <stopOnFailure: Boolean> <repeatCount: int> [rotationSteps: int] | gametest run <testName: string> [rotationSteps: int] | gametest runsetuntilfail [tag: string] [rotationSteps: int] | gametest runset [tag: string] [rotationSteps: int] | gametest clearall | gametest pos | gametest stopall | gametest create <testName: string> [width: int] [height: int] [depth: int] | gametest runthese
```

## 参数详解

- **`testName`**:string - 指定测试的名称。必须为字符串。必须为单个词或者双引号（"）括起的字符串。引号内的字符可以使用\进行转义。
- **`repeatCount`**:int - 指定测试的执行次数。必须为32位整数。且必须大于0。
- **`stopOnFailure`**:Boolean - 必须为布尔值（true或false）。
- **`rotationSteps`**:int - 指定测试的旋转角度。1为顺时针旋转90度；2为顺时针旋转180度；3为顺时针旋转270度。其他值不会使测试旋转。必须为32位整数。
- **`tag`**:string - 指定要执行的测试的名称。必须为字符串。必须为单个词或者双引号（"）括起的字符串。引号内的字符可以使用\进行转义。
- **`width`**:int - 指定结构的X轴大小。默认为5。必须为32位整数。
- **`height`**:int - 指定结构的Y轴大小。默认为5。必须为32位整数。
- **`depth`**:int - 指定结构的Z轴大小。默认为5。必须为32位整数。
