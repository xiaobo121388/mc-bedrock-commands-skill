# /`music`

> 允许玩家控制音乐。

**加入版本：** 1.16.100

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 该命令仅适用于基岩版和教育版。 |

## 语法

```
music play <trackName: string> [volume: float] [fadeSeconds: float] [repeatMode: MusicRepeatMode] | music queue <trackName: string> [volume: float] [fadeSeconds: float] [repeatMode: MusicRepeatMode] | music stop [fadeSeconds: float] | music volume <volume: float>
```

## 参数详解

- **`trackName`**:string - 指定播放音乐名。必须是单个单词（不含空格）或带引号的字符串。必须为音乐名或为Json路径指向的 <a_resource_pack>/sounds/sound_definitions.json 文件中的 “record.<music_name>” 或 “music.game.<music_name>” （例如使用 record.cat 来播放音乐唱片cat）
- **`volume`**:float - 调整音乐音量。必须为浮点数，最小值为0，最大值为1.00。
- **`fadeSeconds`**:float - 调整音乐淡入/淡出时间。必须为浮点数，最小值为0，最大值为10。
- **`repeatMode`**:MusicRepeatMode - 指定是否循环播放音乐，默认为play_once。所取值必须为 loop 与 play_once 中的一个。
