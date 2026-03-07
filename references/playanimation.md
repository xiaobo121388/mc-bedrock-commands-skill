# /`playanimation`

> 在一个或多个实体上播放一次性动画。

**加入版本：** 1.16.100

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 本条目所述内容仅适用于基岩版和​教育版。 |

## 语法

```
playanimation <entity: target> <animation: string> [next_state: string] [blend_out_time: float] [stop_expression: string] [controller: string]
```

## 参数详解

- **`entity`**:target: CommandSelector<Actor> - 指定目标。必须为玩家名或目标选择器。
- **`animation`**:string: basic_string - 指定动画。由<资源包>/entity/<实体名称>.entity.json文件内“minecraft:client_entity”.“animations”的参数定义。必须为字符串。必须为单个词或者双引号（“）括起的字符串。引号内的字符可以使用\进行转义。
- **`next_state`**:string: basic_string - 指定动画播放完毕后的状态。由<资源包>/animation_controllers/<控制器>.json文件内“animation_controllers”.“<控制器名称>”.“states”的参数定义。必须为字符串。必须为单个词或者双引号（“）括起的字符串。引号内的字符可以使用\进行转义。
- **`blend_out_time`**:float: float - 指定动画渐变的持续时间。必须为单精度浮点数。
- **`stop_expression`**:string: basic_string - 指定动画播放终止的条件。应为Molang表达式。必须为字符串。必须为单个词或者双引号（“）括起的字符串。引号内的字符可以使用\进行转义。
- **`controller`**:string: basic_string - 指定动画控制器。由<资源包>/entity/<实体名称>.entity.json文件内“minecraft:client_entity”.“render_controllers”的参数定义。必须为字符串。必须为单个词或者双引号（“）括起的字符串。引号内的字符可以使用\进行转义。
