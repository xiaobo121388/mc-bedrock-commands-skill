# mc-bedrock-commands

《我的世界》基岩版（Bedrock Edition）指令参考 skill，用于在 GitHub Copilot / VS Code 中查询、编写和调试基岩版指令。

本 skill 覆盖常用命令语法、参数类型、权限等级、加入版本、基础概念和中国版开发适配说明，适合用于命令编写、行为包开发、地图制作、服务器管理和网易中国版 Mod 开发场景。

## 内容概览

- `SKILL.md`：skill 入口文件，包含触发描述、查询方式、语法约定、完整指令列表和中国版 Python 适配说明。
- `references/`：具体参考文档目录，包含 97 份 Markdown 文档。
- `references/<command>.md`：单个指令的详细说明，例如 `/execute` 对应 `references/execute.md`。
- `references/target-selector.md`：目标选择器参考，覆盖 `@a`、`@e`、`@s`、`@p`、`@r` 及常见筛选参数。
- `references/coordinate-system.md`：坐标系统参考，覆盖绝对坐标、相对坐标 `~` 和局部坐标 `^`。
- `references/modapi.md`：网易中国版 ModAPI 执行指令相关说明。

## 使用方式

将本目录作为一个 Copilot skill 使用时，询问基岩版指令相关问题即可触发。例如：

```text
基岩版 /execute 怎么切换维度执行命令？
给我写一个 /scoreboard 计分板示例。
网易中国版 Python 里怎么安全调用 /tp？
解释 @e[type=zombie,r=10] 的含义。
```

也可以直接查阅对应 Markdown 文件：

```text
references/execute.md
references/gamerule.md
references/target-selector.md
references/coordinate-system.md
```

## 文档格式

单个指令文档通常包含：

- 指令用途简介
- 加入版本
- 别名、权限等级、作弊要求和额外说明
- 基岩版语法
- 参数详解
- 常用示例
- 必要时补充版本差异、中国版适配或注意事项

## 版本与兼容性

文档以基岩版指令语法为主，并在 `SKILL.md` 和具体 reference 文件中标注新版本指令或语法差异。用于网易中国版开发时，请优先确认当前中国版基岩版本，并避免使用高于目标运行环境的指令或参数。

在中国版 Python 2.7 Mod 开发中，一般通过 ModAPI 的 `SetCommand` 接口执行指令。涉及实体、方块区域或维度上下文的指令，应特别注意执行主体、区块加载和维度切换。

## 维护建议

新增或更新指令时，建议同步维护以下内容：

- 在 `references/` 中新增或更新对应指令文档。
- 在 `SKILL.md` 的完整指令列表中更新描述。
- 对新加入的版本指令，补充加入版本和兼容性说明。
- 对别名指令，保留独立文档或清晰指向主命令。

## 许可证

本项目使用 MIT License。详见 [LICENSE](LICENSE)。