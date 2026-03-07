---
name: mc-bedrock-commands
description: 提供《我的世界》基岩版（Bedrock Edition）所有指令的详细语法、参数、权限等级和版本信息。当用户需要查询、编写或调试基岩版指令（如 /execute, /tp, /gamemode, /scoreboard 等）时使用此技能。
---

# 《我的世界》基岩版指令详解

基岩版指令的完整参考。涵盖语法、参数类型、权限等级、版本信息。数据来源：中文 Minecraft Wiki。

## 查询方式

根据指令名称读取 `references/<指令名>.md`。例如查询 `/execute`：

```
/home/ubuntu/skills/mc-bedrock-commands/references/execute.md
```

若指令有别名（如 `tp` 和 `teleport`），两者均有独立文件。

中国版ModApi指令相关接口文档请参见 [references/modapi.md](references/modapi.md)。

## 语法约定（基岩版）

- `字面量`：按原样输入
- `名称: 类型`：需替换为合适值的参数
- `<输入项>`：必选
- `[输入项]`：可选（仅出现在命令末尾）
- `字面量|字面量`：选择其一

## 1.20.50 后加入的新指令

以下指令在 1.20.50 之后的版本中加入，在 reference 文件中有额外版本标注：

| 指令 | 加入版本 | 描述 |
|---|---|---|
| aimassist | 1.21.50 | 修改玩家的瞄准辅助 |
| controlscheme | 1.21.80.27 | 修改相机预设的控制方案 |
| gametips | 1.20.80.20 | 启用或禁用游戏提示 |
| hud | 1.20.60.23 | 修改 HUD 的可见性 |
| place | 1.21.50.26 | 放置地物、结构模板或结构池 |
| reloadpacketlimitconfig | 1.21.100.20 | 重新加载数据包限制配置 |
| set_movement_authority | 1.21.50.20 | 控制移动权威端 |

## 完整指令列表

| 指令 | 描述 | 新指令 |
|---|---|---|
| ability | 赋予或剥夺玩家的能力 | |
| aimassist | 修改玩家的瞄准辅助 | ✅ |
| allowlist | 管理服务器白名单 | |
| alwaysday | 锁定或解锁终为白日（别名：daylock） | |
| camera | 修改玩家的相机视角 | |
| camerashake | 启用镜头抖动效果 | |
| changesetting | 更改 BDS 服务器设置 | |
| clear | 清除玩家物品栏的物品 | |
| clearspawnpoint | 清除玩家的重生点 | |
| clone | 复制方块区域到另一处 | |
| connect | 连接至 WebSocket 服务器（别名：wsserver） | |
| controlscheme | 修改相机预设的控制方案 | ✅ |
| damage | 对指定实体造成伤害 | |
| daylock | 锁定或解锁终为白日（别名：alwaysday） | |
| dedicatedwsserver | 连接至 WebSocket 服务器 | |
| deop | 撤销玩家的管理员权限 | |
| dialogue | 打开或改变 NPC 对话框 | |
| difficulty | 设定世界难度等级 | |
| effect | 管理实体上的状态效果 | |
| enchant | 为实体手持物品添加魔咒 | |
| execute | 改变执行上下文并执行命令 | |
| fill | 用方块填充区域 | |
| fog | 更改玩家的迷雾效果 | |
| function | 运行一个函数 | |
| gamemode | 设置玩家的游戏模式 | |
| gamerule | 设置或查询游戏规则 | |
| gametest | 管理和运行 GameTest 框架 | |
| gametips | 启用或禁用游戏提示 | ✅ |
| give | 给予玩家物品 | |
| help | 获取命令帮助信息（别名：?） | |
| hud | 修改 HUD 的可见性 | ✅ |
| immutableworld | 设置世界不可变状态 | |
| inputpermission | 管理玩家的输入权限 | |
| kick | 将玩家踢出服务器 | |
| kill | 杀死实体 | |
| list | 列出服务器中的玩家 | |
| locate | 定位结构或生物群系 | |
| loot | 生成战利品 | |
| me | 广播关于自己的信息 | |
| mobevent | 控制生物事件 | |
| msg | 发送私聊消息（别名：tell, w） | |
| music | 控制音乐播放 | |
| op | 给予玩家管理员权限 | |
| ops | 管理操作员状态 | |
| particle | 显示粒子效果 | |
| permission | 管理权限列表 | |
| place | 放置地物、结构模板或结构池 | ✅ |
| playanimation | 播放实体动画 | |
| playsound | 播放声音事件 | |
| project | 管理编辑器项目 | |
| recipe | 管理玩家的配方 | |
| reload | 重新加载行为包函数和脚本 | |
| reloadconfig | 重新加载配置文件 | |
| reloadpacketlimitconfig | 重新加载数据包限制配置 | ✅ |
| remove | 移除实体 | |
| replaceitem | 替换物品栏中的物品 | |
| resourceuri | 管理暂停菜单资源链接 | |
| ride | 管理实体骑乘关系 | |
| save | 管理服务器备份 | |
| say | 向所有玩家发送消息 | |
| schedule | 计划延迟执行函数 | |
| scoreboard | 管理记分板 | |
| script | 调试 GameTest 框架 | |
| scriptevent | 触发脚本事件 | |
| sendshowstoreoffer | 发送商店特惠请求 | |
| set_movement_authority | 控制移动权威端 | ✅ |
| setblock | 设置指定位置的方块 | |
| setworldspawn | 设置世界出生点 | |
| spawnpoint | 设置玩家出生点 | |
| spreadplayers | 随机传送实体 | |
| stop | 关闭服务器 | |
| stopsound | 停止声音播放 | |
| structure | 保存或加载结构 | |
| summon | 召唤实体 | |
| tag | 管理实体标签 | |
| teleport | 传送实体（别名：tp） | |
| tell | 发送私聊消息（别名：msg, w） | |
| tellraw | 发送 JSON 文本消息 | |
| testfor | 检测符合条件的实体 | |
| testforblock | 检测指定位置的方块 | |
| testforblocks | 比较两个区域的方块 | |
| tickingarea | 管理常加载区域 | |
| time | 控制或查询世界时间 | |
| title | 管理屏幕标题 | |
| titleraw | 使用 JSON 管理屏幕标题 | |
| toggledownfall | 切换天气 | |
| tp | 传送实体（别名：teleport） | |
| transfer | 转移玩家到其他服务器 | |
| weather | 更改天气 | |
| worldbuilder | 管理世界建造者能力（别名：wb） | |
| wsserver | 连接 WebSocket 服务器（别名：connect） | |
| xp | 管理玩家经验值 | |

## 中国版Python适配说明
在中国版开发环境中（Python 2.7），一般使用ModApi的SetCommand接口来执行指令. 以下是中国版指令使用注意事项：
- 目前中国版版本为1.20.50，请注意指令版本兼容性，避免使用1.20.50之后加入的指令。
- 调用指令时候需要时刻注意调用主体(entityId)，如果不设置则随机选择玩家，可能会导致指令执行失败或者作用于错误的玩家。
- 作用于世界方块的指令需要区块被加载，否则指令会执行失败。一般要使用者需要先使用 `tickingarea` 指令创建常加载区域，或者确保玩家在指令作用范围内。
- 对维度有要求先使用 `execute` 指令切换到正确的维度上下文.




