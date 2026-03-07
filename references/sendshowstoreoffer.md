# /`sendshowstoreoffer`

> 向玩家发送显示商店特惠的请求。

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 4 |
| **需要作弊** | 是 |
| **额外说明** | 仅专用服务端 |

## 语法

```
sendshowstoreoffer <player: target> <redirectType: RedirectLocation> <offerId: string> | sendshowstoreoffer <player: target> server
```

## 参数详解

- **`player`**:target - 必须为玩家名或目标选择器。且要求目标选择器为玩家类型
- **`redirectType`**:RedirectLocation - 指定请求类型，可用值有：marketplace, character
- **`offerId`**:string - 指定商店特惠ID
