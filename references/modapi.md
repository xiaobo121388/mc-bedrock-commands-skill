# 中国版ModApi指令相关接口文档

## 指令（Command）相关接口

### GetCommandPermissionLevel

作用域：服务端

方法：`mod.server.component.commandCompServer.CommandCompServer.GetCommandPermissionLevel`

- 描述：返回设定使用 `/op` 命令时 OP 的权限等级（对应 server.properties 中的 `op-permission-level` 配置）。
- 参数：无
- 返回值：

| 数据类型 | 说明 |
|---|---|
| int | 权限等级：1-OP 可以绕过重生点保护；2-OP 可以使用所有单人游戏作弊命令；3-OP 可以使用大多数多人游戏中独有的命令；4-OP 可以使用所有命令 |

- 示例：

```python
import mod.server.extraServerApi as serverApi
comp = serverApi.GetEngineCompFactory().CreateCommand(levelId)
opLevel = comp.GetCommandPermissionLevel()
print "GetCommandPermissionLevel oplevel={}".format(opLevel)
```

### GetDefaultPlayerPermissionLevel

作用域：服务端

方法：`mod.server.component.commandCompServer.CommandCompServer.GetDefaultPlayerPermissionLevel`

- 描述：返回新玩家加入时的默认权限身份（对应 `server.properties` 中的 `default-player-permission-level` 配置）。
- 参数：无
- 返回值：

| 数据类型 | 说明 |
|---|---|
| int | 权限身份：0-Visitor；1-Member；2-Operator；3-自定义 |

- 示例：

```python
import mod.server.extraServerApi as serverApi
comp = serverApi.GetEngineCompFactory().CreateCommand(levelId)
opLevel = comp.GetDefaultPlayerPermissionLevel()
print "GetDefaultPlayerPermissionLevel oplevel={}".format(opLevel)
```

### SetCommand

作用域：服务端

方法：`mod.server.component.commandCompServer.CommandCompServer.SetCommand`

- 描述：使用游戏内指令（等同于在聊天框输入命令）。
- 参数：

| 参数名 | 数据类型 | 说明 |
|---|---:|---|
| cmdStr | str | 指令文本，例如："/tp @p 100 5 100" |
| entityId | str | 实体 Id（可选），如果不设置，则由系统随机选择一个玩家 |
| showOutput | bool | 是否输出到聊天窗口（可选，默认 False）。若为 True 且指令执行成功，会像聊天框输入原生命令一样输出返回信息；仅在该参数为 True 时会触发 `OnCommandOutputServerEvent` 与 `OnCommandOutputClientEvent` |

- 返回值：

| 数据类型 | 说明 |
|---|---|
| bool | 命令是否执行成功 |

- 备注：

- 当 `entityId` 指向非玩家实体时，即使 `showOutput` 为 True，也不会输出到聊天窗口，且 `OnCommandOutputClientEvent` 不会被触发。
- 在极限（Hardcore）或受限环境下，某些需开启作弊权限的命令无法调用。

- 示例：

```python
import mod.server.extraServerApi as serverApi
comp = serverApi.GetEngineCompFactory().CreateCommand(levelId)
comp.SetCommand("/tp @p 100 5 100")  # 传送指令
```

### SetCommandPermissionLevel

作用域：服务端

方法：`mod.server.component.commandCompServer.CommandCompServer.SetCommandPermissionLevel`

- 描述：设置当玩家使用 `/op` 时，赋予的新 OP 的权限等级（对应 `server.properties` 的 `op-permission-level`）。
- 参数：

| 参数名 | 数据类型 | 说明 |
|---|---:|---|
| opLevel | int | 权限等级：1-OP 可以绕过重生点保护；2-OP 可以使用所有单人游戏作弊命令；3-OP 可以使用大多数多人游戏中独有的命令；4-OP 可以使用所有命令 |

- 返回值：

| 数据类型 | 说明 |
|---|---|
| bool | 操作是否成功 |

- 备注：此 API 不会改变已经拥有 OP 的玩家的权限等级，仅影响在调用此 API 之后再被赋予 OP 的玩家，建议在游戏初始化阶段调用。

- 示例：

```python
import mod.server.extraServerApi as serverApi
comp = serverApi.GetEngineCompFactory().CreateCommand(levelId)
opLevel = 4
suc = comp.SetCommandPermissionLevel(opLevel)
print "SetCommandPermissionLevel to {} suc={}".format(opLevel, suc)
```

### SetDefaultPlayerPermissionLevel

作用域：服务端

方法：`mod.server.component.commandCompServer.CommandCompServer.SetDefaultPlayerPermissionLevel`

- 描述：设置新玩家加入时的默认权限身份（对应 `server.properties` 的 `default-player-permission-level`）。
- 参数：

| 参数名 | 数据类型 | 说明 |
|---|---:|---|
| opLevel | int | 权限身份：0-Visitor；1-Member；2-Operator；3-自定义 |

- 返回值：

| 数据类型 | 说明 |
|---|---|
| bool | 操作是否成功 |

- 备注：此 API 不会修改已经加入过游戏的玩家的权限，仅影响随后加入的玩家。

- 示例：

```python
import mod.server.extraServerApi as serverApi
comp = serverApi.GetEngineCompFactory().CreateCommand(levelId)
opLevel = 1
suc = comp.SetDefaultPlayerPermissionLevel(opLevel)
print "SetDefaultPlayerPermissionLevel to {} suc={}".format(opLevel, suc)
```

---

## 记分板（Scoreboard）相关接口

说明：以下接口由 `mod.server.component.gameCompServer.GameComponentServer` 与 `mod.client.component.gameCompClient.GameComponentClient` 提供，部分接口在客户端只能在使用 `/scoreboard objectives setdisplay sidebar` 后可见。

### GetAllPlayerScoreboardObjects

作用域：服务端 / 客户端

方法（服务端）：`mod.server.component.gameCompServer.GameComponentServer.GetAllPlayerScoreboardObjects`

方法（客户端）：`mod.client.component.gameCompClient.GameComponentClient.GetAllPlayerScoreboardObjects`

- 描述：获取玩家记分项列表（按玩家分组的记分数据）。
- 参数：无
- 返回值：

| 数据类型 | 说明 |
|---|---|
| list(dict) | 玩家记分项信息字典列表 |

- 客户端备注：只有在使用 `/scoreboard objectives setdisplay sidebar <目标>` 设置显示后，客户端才能获取到对应记分项数据。

- 示例（服务端）：

```python
import mod.server.extraServerApi as serverApi
comp = serverApi.GetEngineCompFactory().CreateGame(levelId)
print(comp.GetAllPlayerScoreboardObjects())
```

- 示例（客户端）：

```python
import mod.client.extraClientApi as clientApi
comp = clientApi.GetEngineCompFactory().CreateGame(levelId)
print(comp.GetAllPlayerScoreboardObjects())
```

### GetAllScoreboardObjects

作用域：服务端 / 客户端

方法（服务端）：`mod.server.component.gameCompServer.GameComponentServer.GetAllScoreboardObjects`

方法（客户端）：`mod.client.component.gameCompClient.GameComponentClient.GetAllScoreboardObjects`

- 描述：获取所有记分板准则（objectives）信息列表。
- 参数：无
- 返回值：

| 数据类型 | 说明 |
|---|---|
| list(dict) | 记分准则信息字典列表 |

- 客户端备注：只有在使用 `/scoreboard objectives setdisplay sidebar <目标>` 设置显示后，客户端才能获取到对应记分准则数据。

- 示例（服务端）：

```python
import mod.server.extraServerApi as serverApi
comp = serverApi.GetEngineCompFactory().CreateGame(levelId)
print(comp.GetAllScoreboardObjects())
```

- 示例（客户端）：

```python
import mod.client.extraClientApi as clientApi
comp = clientApi.GetEngineCompFactory().CreateGame(levelId)
print(comp.GetAllScoreboardObjects())
```

---