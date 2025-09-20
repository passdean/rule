配置文件必须配合sub-store生成订阅文件.sub-store安装参照1.11.x的README.md
配置文件只适合openwrt的路由设备并且安装momo插件使用，其他singbox插件以及其他设备不适用（比如手机等）。

momo插件仓库：

```https://github.com/nikkinikki-org/OpenWrt-momo```

singbox内核仓库：

```https://github.com/SagerNet/sing-box```

脚本代码:

```https://raw.githubusercontent.com/xream/scripts/main/surge/modules/sub-store-scripts/sing-box/template.js#type=组合订阅&name=singbox&outbound=🕳ℹ️🐸 手动选择|♻️ 自动选择🏷ℹ️^(?!.*(?:官网|剩余|流量|套餐|免费|订阅|站|箱||到期时间|全球直连|GB|Expire Date|Traffic|ExpireDate)).*🕳ℹ️🇭🇰 香港手动🏷ℹ️^(?!.*(?:us)).*(🇭🇰|HK|hk|香港|港|HongKong)🕳ℹ️🇯🇵 日本手动🏷ℹ️^(?!.*(?:us|NG)).*(🇯🇵|JP|jp|日本|日|Japan)🕳ℹ️🇸🇬 狮城手动🏷ℹ️^(?!.*(?:us)).*(新加坡|坡|狮城|SG|Singapore)🕳ℹ️🇺🇲 美国手动🏷ℹ️^(?!.*(?:AUS|RUS)).*(🇺🇸|US|us|美国|美|United States)```
