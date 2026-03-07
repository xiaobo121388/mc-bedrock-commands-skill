# /`execute`

> 改变命令执行上下文，执行逻辑判断，并在此基础上执行任意其他命令。

**加入版本：** 1.19.50

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 该命令在基岩版1.19.10中作为实验性玩法加入，在1.19.50中正式发布。 |

## 语法

```
execute align <axes: string> <chainedCommand: ExecuteChainedOption_0> | execute anchored <eyes|feet> <chainedCommand: ExecuteChainedOption_0> | execute as <origin: target> <chainedCommand: ExecuteChainedOption_0> | execute at <origin: target> <chainedCommand: ExecuteChainedOption_0> | execute facing <position: x y z> <chainedCommand: ExecuteChainedOption_0> | execute facing entity <origin: target> <eyes|feet> <chainedCommand: ExecuteChainedOption_0> | execute in <dimension: Dimension> <chainedCommand: ExecuteChainedOption_0> | execute positioned <position: x y z> <chainedCommand: ExecuteChainedOption_0> | execute positioned as <origin: target> <chainedCommand: ExecuteChainedOption_0> | execute rotated <yaw: value> <pitch: value> <chainedCommand: ExecuteChainedOption_0> | execute rotated as <origin: target> <chainedCommand: ExecuteChainedOption_0> | execute <subcommand: Option_If_Unless> block <position: x y z> <block: Block> [chainedCommand: ExecuteChainedOption_0] | execute <subcommand: Option_If_Unless> block <position: x y z> <block: Block> <blockStates: block states> [chainedCommand: ExecuteChainedOption_0] | execute <subcommand: Option_If_Unless> blocks <begin: x y z> <end: x y z> <destination: x y z> <scan mode: BlockScanMode> [chainedCommand: ExecuteChainedOption_0] | execute <subcommand: Option_If_Unless> entity <target: target> [chainedCommand: ExecuteChainedOption_0] | execute <subcommand: Option_If_Unless> score <target: target> <objective: string> <subcommand: ScoreboardPlayersTest_subcommand_0> <source: target> <objective: string> [chainedCommand: ExecuteChainedOption_0] | execute <subcommand: Option_If_Unless> score <target: target> <objective: string> matches <range: integer range> [chainedCommand: ExecuteChainedOption_0] | execute run <command: command>
```

## 参数详解

- **`axes`**:string - 需要转换的坐标轴，必须为x、y、z三个字符的组合
- **`eyes|feet`**:enum - 需要设置的锚点位置，eyes为眼部，feet为脚部
- **`origin`**:target: CommandSelector<Actor> - 目标选择器，用于指定执行者、位置或旋转来源
- **`position`**:x y z: CommandPositionFloat - 三维坐标
- **`dimension`**:Dimension: enum - 维度ID，如overworld, nether, the_end
- **`yaw`**:value: RelativeFloat - 偏航角
- **`pitch`**:value: RelativeFloat - 俯仰角
- **`subcommand`**:Option_If_Unless: enum - if 或 unless
- **`block`**:Block: Block - 方块ID
- **`blockStates`**:block states: BlockStateCommandParam - 方块状态
- **`begin`**:x y z: CommandPosition - 区域起始坐标
- **`end`**:x y z: CommandPosition - 区域结束坐标
- **`destination`**:x y z: CommandPosition - 对照区域坐标
- **`scan mode`**:BlockScanMode: enum - all 或 masked
- **`target`**:target: CommandSelector<Actor> - 目标选择器
- **`objective`**:string - 记分项名称
- **`ScoreboardPlayersTest_subcommand_0`**:enum - <, <=, =, >=, >
- **`range`**:integer range - 整数范围
- **`command`**:command: unique_ptr<Command> - 另一条完整的命令
