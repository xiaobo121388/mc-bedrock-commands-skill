# /`schedule`

> 计划一个函数在指定区域加载完毕后执行，或在一段时间后执行。

**加入版本：** 1.16.100

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 在1.21.40版本中加入了清除队列函数的语法，在1.21.50版本中加入了延时运行函数的语法。 |

## 语法

```
schedule delay add <function: filepath> <time: int> [replace|append] | schedule delay add <function: filepath> <time: int>D [replace|append] | schedule delay add <function: filepath> <time: int>S [replace|append] | schedule delay add <function: filepath> <time: int>T [replace|append] | schedule on_area_loaded add <from: x y z> <to: x y z> <function: filepath> | schedule on_area_loaded add circle <center: x y z> <radius: int> <function: filepath> | schedule on_area_loaded add tickingarea <name: string> <function: filepath> | schedule clear <function: filepath> | schedule on_area_loaded clear function <function: filepath> | schedule on_area_loaded clear tickingarea <name: string> [function: filepath] | schedule delay clear <function: filepath>
```

## 参数详解

- **`function`**:filepath: CommandFilePath - 指定要计划运行的函数，必须为函数文件路径
- **`time`**:int: int - 指定等待的时间，必须为32位整数
- **`replace|append`**:- 指定是添加新计划还是取代现有计划
- **`from`**:x y z: CommandPosition - 定义矩形加载区域的对角坐标
- **`to`**:x y z: CommandPosition - 定义矩形加载区域的对角坐标
- **`center`**:x y z: CommandPosition - 定义圆形加载区域的圆心坐标
- **`radius`**:int: int - 定义圆形加载区域的半径
- **`name`**:string: basic_string - 指定常加载区域的名称
