# /`script`

> 调试GameTest框架选项。

**加入版本：** 1.17.30.23

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 2 |
| **需要作弊** | 是 |
| **额外说明** | 不在命令方块上执行。在1.19.70版本之前属于实验性玩法。 |

## 语法

```
script debugger close | script debugger connect [host: string] [port: int] | script debugger listen <port: int> | script diagnostics startcapture | script diagnostics stopcapture | script profiler start | script profiler stop
```

## 参数详解

- **`host`**:string - 指定主机的名称。必须为单个词或者双引号（"）括起的字符串
- **`port`**:int - 指定调试器的端口，可用端口范围为1024-65535。
