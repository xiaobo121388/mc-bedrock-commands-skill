# /`camera`

> 修改玩家的相机视角。

**加入版本：** 1.20.30

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 部分功能需要开启实验性玩法“创建者照相机的实验性功能”。 |

## 语法

```
/camera <players: target> attach_to_entity <entity: target> | /camera <players: target> clear | /camera <players: target> detach_from_entity | /camera <players: target> fade [time <fadeInSeconds: float> <holdSeconds: float> <fadeOutSeconds: float>] [color <red: int> <green: int> <blue: int>] | /camera <players: target> fov_clear [fovEaseTime: float] [fovEaseType: Easing] | /camera <players: target> fov_set <fov_value: float> [fovEaseTime: float] [fovEaseType: Easing] | /camera <players: target> play_spline <name: string> | /camera <players: target> remove_target | /camera <players: target> set <preset: string> [ease <easeTime: float> <easeType: Easing>] [pos <position: x y z>] [rot <xRot: value> <yRot: value>] [facing <lookAtEntity: target>|<lookAtPosition: x y z>] [default: default] [entity_offset <xEntityOffset: float> <yEntityOffset: float> <zEntityOffset: float>] [view_offset <xViewOffset: float> <yViewOffset: float>] | /camera <players: target> target_entity <entity: target> [target_center_offset <xTargetCenterOffset: float> <yTargetCenterOffset: float> <zTargetCenterOffset: float>]
```

## 参数详解

- **`players`**:target - 指定将被修改相机视角的玩家
- **`entity`**:target - 指定相机将要固定于的实体
- **`red`**:int, green: int, blue: int - 指定相机视角的RGB颜色 (0-255)
- **`fadeInSeconds`**:float, holdSeconds: float, fadeOutSeconds: float - 指定相机视角的淡入、保持和淡出持续时间 (0.0-10.0秒)
- **`fov_value`**:float - 指定相机视场角 (30-110)
- **`fovEaseTime`**:float - 指定相机视场角平滑过渡的持续时间 (秒)
- **`fovEaseType`**:Easing - 指定用于相机视场角的运镜函数/类型
- **`name`**:string - 指定样条ID
- **`preset`**:string - 指定相机视角/预设
- **`easeTime`**:float - 指定相机视角平滑过渡的持续时间 (秒)
- **`easeType`**:Easing - 指定用于相机视角的运镜函数/类型
- **`default`**:default - 将自由视角的位置和朝向改为默认值
- **`lookAtEntity`**:target - 指定相机视角朝向的实体
- **`lookAtPosition`**:x y z - 指定相机视角朝向的坐标
- **`position`**:x y z - 指定相机视角的位置
- **`xRot`**:value, yRot: value - 指定相机视角的垂直和水平旋转角度
- **`xViewOffset`**:float, yViewOffset: float - 指定相机视角的偏移量
- **`xEntityOffset`**:float, yEntityOffset: float, zEntityOffset: float - 指定相机视角相对于实体的偏移量
- **`xTargetCenterOffset`**:float, yTargetCenterOffset: float, zTargetCenterOffset: float - 指定相机视角相对于聚焦/目标实体中心的偏移量。
