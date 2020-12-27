# 添加插件 URL 

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 此教程让用户统一学习关于 `添加插件` 中填写的 URL 的格式要求及其内容要求

## 一、对 URL 格式及其内容的要求

- 对 URL 格式的要求

  - 文件上传至github库的，订阅地址 URL 必须以 `http://raw` 开头
  
- 对 URL 内容的要求

  - 必须拥有 Loon 配置文件的格式，目前暂时支持 `[Rule]` 、 `[URL Rewrite]` 、 `[Script]` 、 `[MITM]` 模块，后续会扩展更多模块
  
## 二、URL 内容示范

```
[Rule]
DOMAIN,google.com,PROXY

[URL Rewrite]
^https?:\/\/(www.)?(g|google)\.cn https://www.google.com 302

[Script]
http-request ^https?:\/\/(www.)?(example)\.com script-path=localscript.js,tag = requestScript,enable=true
http-response ^https?:\/\/(www.)?(example)\.com script-path=https://example.com/loon.js,timeout=10,requires-body = true,tag = responseScript,enable=true
cron "0 8 * * *" script-path=cron.js,tag = responseScript,enable=true

[MITM]
hostname = *.example.com,*.sample.com
```

## 三、URL 实例文件示范

```
[Rule]
DOMAIN-KEYWORD,baidu,DIRECT

[URL Rewrite]
^https?:\/\/(www.)?(g|google)\.cn https://www.google.com 302

[Script]
# 京东京豆签到脚本

cron "5 0 * * *" tag=京东多合一签到, script-path=https://raw.githubusercontent.com/NobyDa/Script/master/JD-DailyBonus/JD_DailyBonus.js
http-request https:\/\/api\.m\.jd\.com\/client\.action.*functionId=signBean tag=获取京东Cookie, script-path=https://raw.githubusercontent.com/NobyDa/Script/master/JD-DailyBonus/JD_DailyBonus.js

# 京东东东农场脚本

cron "5 6-18/6 * * *" script-path=https://raw.githubusercontent.com/lxk0301/scripts/master/jd_fruit.js,tag=东东农场

# 美团签到脚本
http-request ^https:\/\/promotion.waimai.meituan.com\/playcenter\/signIn\/entry script-path=https://raw.githubusercontent.com/chavyleung/scripts/master/wmmeituan/wmmeituan.cookie.js
http-request ^https:\/\/promotion.waimai.meituan.com\/playcenter\/signIn\/doaction script-path=https://raw.githubusercontent.com/chavyleung/scripts/master/wmmeituan/wmmeituan.cookie.js,requires-body=true
cron "10 0 0 * * *" script-path=https://raw.githubusercontent.com/chavyleung/scripts/master/wmmeituan/wmmeituan.js

[MITM]
hostname = api.m.jd.com,promotion.waimai.meituan.com
```

## 四、获取正确的 URL 链接的方法

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击需要订阅脚本的文件

![image](https://raw.githubusercontent.com/TiyNa/LoonManualimg/main/Plus/Plugin_Raw_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 Raw

![image](https://raw.githubusercontent.com/TiyNa/LoonManualimg/main/Plus/Plugin_Raw_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 长按地址栏，点击 `拷贝` 即可

![image](https://raw.githubusercontent.com/TiyNa/LoonManualimg/main/Plus/Plugin_Raw_3.jpg)

# 多说几句

- 虽然支持 `[Script]` 模块，但是不建议将**签到类脚本**的脚本配置代码写入插件文件内，原因是通过此方式添加脚本不允许用户修改脚本执行时间

- 建议将类似于 `京东、淘宝历史价格脚本` 的脚本配置代码写入插件文件内，因为此类脚本不会有弹窗提醒，也不需要修改执行时间
