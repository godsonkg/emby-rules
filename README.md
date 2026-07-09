# emby-rules

个人维护的 Emby 分流规则集，Surge/Loon/Clash 通用格式（classical text list）。

- `Emby.list` = blackmatrix7/ios_rule_script 原版社区规则(52条) + 本人私有线路域名(15条)，去重合并
- 原版上游更新缓慢（该分类社区不活跃），本仓库改为按需手动维护

## 用法

Surge:
```
RULE-SET,https://raw.githubusercontent.com/godsonkg/emby-rules/main/Emby.list,Emby
```

Loon:
```
https://raw.githubusercontent.com/godsonkg/emby-rules/main/Emby.list, policy=Emby, tag=Emby, enabled=true
```
