# /`summon`

> 召唤一个实体。

**加入版本：** 0.16.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 无 |

## 语法

```
summon <entityType: EntityType> [spawnPos: x y z] [yRot: float] [xRot: float] [spawnEvent: string] [nameTag: string] | summon <entityType: EntityType> <nameTag: string> [spawnPos: x y z] | summon <entityType: EntityType> [spawnPos: x y z] facing <lookAtEntity: target> [spawnEvent: string] [nameTag: string] | summon <entityType: EntityType> [spawnPos: x y z] facing <position: x y z> [spawnEvent: string] [nameTag: string]
```

## 参数详解

- **`entityType`**:EntityType - 指定要被召唤的实体类型
- **`spawnPos`**:x y z - 指定该实体的召唤位置
- **`yRot`**:float - 指定该实体生成时的绕Y轴旋转
- **`xRot`**:float - 指定该实体生成时的绕X轴旋转
- **`spawnEvent`**:string - 指定该实体的召唤时附带的实体事件
- **`nameTag`**:string - 指定该实体的名称
- **`lookAtEntity`**:target - 指定该实体生成时的要朝向的实体
- **`lookAtPosition`**:x y z - 指定该实体生成时的要朝向的坐标
