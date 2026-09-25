# emby-rules

自己用的 Emby 分流规则，Surge / Loon / Clash 通用的文本规则格式。

`Emby.list` 由两部分组成：

- blackmatrix7/ios_rule_script 的 Emby 规则。上游这一类很久没更新，我不再同步，改成手动维护
- 自己在用的 Emby 线路域名，以前分散在各个客户端的配置里，现在统一放这里

新线路直接加到文件末尾。加之前看一眼有没有被已有的 `DOMAIN-KEYWORD` 或 `DOMAIN-SUFFIX` 覆盖，避免重复。

`PROCESS-NAME,com.mb.android` 只对安卓上的 Clash 有用，Surge iOS 会忽略这一行。

## 用法

Surge：

```
RULE-SET,https://raw.githubusercontent.com/godsonkg/emby-rules/main/Emby.list,Emby
```

Loon：

```
https://raw.githubusercontent.com/godsonkg/emby-rules/main/Emby.list, policy=Emby, tag=Emby, enabled=true
```

`Emby` 换成你配置里的策略组名。
