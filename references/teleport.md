# /`teleport`

> 传送实体（玩家、生物等）到指定的地点，并修改其旋转角度。

**加入版本：** 0.16.0

| 属性 | 值 |
|---|---|
| **别名** | `tp` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 无 |

## 语法

```
teleport <destination: target> | teleport <victim: target> <destination: target> [checkForBlocks: Boolean] | teleport <destination: x y z> [checkForBlocks: Boolean] | teleport <victim: target> <destination: x y z> [checkForBlocks: Boolean] | teleport <destination: x y z> [yRot: value] [xRot: value] [checkForBlocks: Boolean] | teleport <destination: x y z> facing <lookAtPosition: x y z> [checkForBlocks: Boolean] | teleport <destination: x y z> facing <lookAtEntity: target> [checkForBlocks: Boolean] | teleport <victim: target> <destination: x y z> [yRot: value] [xRot: value] [checkForBlocks: Boolean] | teleport <victim: target> <destination: x y z> facing <lookAtPosition: x y z> [checkForBlocks: Boolean] | teleport <victim: target> <destination: x y z> facing <lookAtEntity: target> [checkForBlocks: Boolean]
```

## 参数详解

- **`victim`**:target: CommandSelector<Actor> - 指定要被传送的实体。如果未指定，默认为命令执行者。必须为玩家名或目标选择器
- **`destination`**:x y z: CommandPositionFloat - 指定要被传送到的坐标。必须为三维坐标，元素为单精度浮点数。允许相对坐标（~ ~ ~）或局部坐标（^ ^ ^）
- **`destination`**:target: CommandSelector<Actor> - 指定要被传送到的实体。必须为玩家名或目标选择器
- **`yRot`**:value: RelativeFloat - 指定实体传送后的绕Y轴旋转角度
- **`xRot`**:value: RelativeFloat - 指定实体传送后的绕X轴旋转角度
- **`lookAtPosition`**:x y z: CommandPositionFloat - 指定实体传送后朝向的坐标
- **`lookAtEntity`**:target: CommandSelector<Actor> - 指定实体传送后朝向的实体
- **`checkForBlocks`**:Boolean: enum - 如果为true，只当目的地不会被方块碰撞箱阻挡时，传送才会生效。如果为false或未指定，则不进行该检查，直接进行传送。
