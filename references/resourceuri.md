# /`resourceuri`

> 设定或清除暂停菜单下的资源链接。

**加入版本：** 1.14.60

| 属性 | 值 |
|---|---|
| **别名** | `无` |
| **权限等级** | 1 |
| **需要作弊** | 是 |
| **额外说明** | 本条目所述内容仅适用于教育版。 |

## 语法

```
resourceuri | resourceuri clear | resourceuri default [uri: text] | resourceuri named <name: string> [uri: text]
```

## 参数详解

- **`name`**:string - 指定资源链接的按钮文本。必须为单个词或者双引号（"）括起的字符串。引号内的字符可以使用\进行转义。
- **`uri`**:text - 指定资源链接的URI，默认为空。此参数为贪婪字符串参数，即命令的剩余部分全部视作该字符串参数，可以包含空格。
