# /`playsound`

> 以特定的音量和音高，在指定位置向玩家播放声音事件实例。

**加入版本：** 1.0.5.0

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 无 |

## 语法

```
playsound <sound: string> [player: target] [position: x y z] [volume: float] [pitch: float] [minimumVolume: float]
```

## 参数详解

- **`sound`**:string - 指定要播放的声音事件
- **`player`**:target - 指定播放声音的目标，必须为玩家名、目标选择器或UUID
- **`position`**:x y z - 指定声音发出的方位
- **`volume`**:float - 指定声音能被听见的距离，必须至少为0.0
- **`pitch`**:float - 指定声音的音高，默认为1.0
- **`minimumVolume`**:float - 指定在声音可闻范围外的目标能听到的音量，默认为0.0
