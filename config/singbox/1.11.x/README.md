2025年9月singbox客户端  IOS版本只有1.11版还没有更新到1.12版，iPhone手机适配此配置文件。Android手机版已经可以更新到1.12，1.12版也可以使用此版本配置文件。
config_android.json适用于IOS的iPhone手机和Android手机,配置文件不能单独使用,需要docker安装sub-store进行二次转换.

substore搭建命令:

```docker run -it -d \
--restart=always \
-e SUB_STORE_FRONTEND_BACKEND_PATH=/CKg3abstVnOeRpm1aB5G \
-p 3001:3001 \
-v /opt/sub-store:/opt/app/data \
--name sub-store \
xream/sub-store
```
以上代码注意修改20位密匙和端口

后端访问地址:

```http://192.168.10.9:3001?api=http://192.168.10.9:3001/CKg3abstVnOeRpm1aB5G  ```

或者域名访问

```https://sub.gogotest.org?api=https://sub.gogotest.org/CKg3abstVnOeRpm1aB5G```

注意修改成自己的ip或者反代域名和相应的密匙

sub-store脚本命令：（适用于config_android.josn）
```
https://raw.githubusercontent.com/xream/scripts/main/surge/modules/sub-store-scripts/sing-box/template.js#type=组合订阅&name=singbox&outbound=🕳ℹ️🐸 手动切换|♻️ 自动选择|🌍GLOBAL🏷ℹ️^(?!.*(?:官网|剩余|流量|套餐|免费|订阅|站|箱|到期时间|全球直连|GB|Expire Date|Traffic|ExpireDate)).*🕳ℹ️🇭🇰 香港节点🏷ℹ️^(?!.*(?:us)).*(🇭🇰|HK|hk|香港|港|HongKong)🕳ℹ️🇯🇵 日本节点🏷ℹ️^(?!.*(?:us|尼|NG)).*(🇯🇵|JP|jp|日本|日|Japan)🕳ℹ️🇺🇲 美国节点🏷ℹ️^(?!.*(?:AUS|RUS)).*(🇺🇸|US|us|美国|美|United States)🕳ℹ️🇸🇬 新加坡节点🏷ℹ️^(?!.*(?:us)).*(新加坡|坡|狮城|SG|Singapore)

```
