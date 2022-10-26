##### Cookie变量设置 Secrets:**

| 名称               | 内容                             | 说明                                                         |
| ------------------ | -------------------------------- | ------------------------------------------------------------ |
| `PAT`              | 使用Github Actions同步和拉取代码 | 利用Github Actions自动同步上游仓库[PAT获取教程](RepoSync.md) |
| `HOSTLOC_USERNAME` | Hostloc账号                      |                                                              |
| `HOSTLOC_PASSWORD` | Hostloc密码                      |                                                              |
| `IQIYI_COOKIE`     | 爱奇艺Cookie                     | F12控制台执行`console.log(document.cookie)`电脑版有效期三个月 |
| `Xiaomi_User`      | 小米运动账号                     | 小米运动账号,多账号请用#分割 例如：13800138000#13800138001   |
| `Xiaomi_Pw`        | 小米运动密码                     | 小米运动密码,多账号请用#分割 例如：abc123qwe#abcqwe2         |
| `Xiaomi_Bs`        | 小米运动步数                     | 默认为1w-2w之间随机 或自定义随机范围`[18000-25000]`          |
| `BILI_USER`        | 哔哩哔哩账号                     | B站账号                                                      |
| `BILI_PASS`        | 哔哩哔哩密码                     | B站密码                                                      |
| `BILI_COOKIE`      | 哔哩哔哩COOKIE`(非必填)`         | 哔哩哔哩COOKIE,如果账号密码无法登陆就用COOKIE,等一段时间再用账号密码即可. |
| `BILI_NUM`         | 哔哩哔哩每日投币数量             | 每日投币数量`可不填`默认0 不投币                             |
| `BILI_TYPE`        | 哔哩哔哩每日投币方式             | 投币方式`可不填`默认1,只给关注的人投币 0 则随机投币          |
| `BILI_S2C`         | 哔哩哔哩每日银瓜子兑换硬币       | `可不填`默认兑换,设置为`任意数值`则不自动兑换                |
| `V_REF_URL`        | 腾讯视频Request URL              | 电脑端搜索auth_refresh复制整段Request url[图片教程](https://cdn.jsdelivr.net/gh/BlueskyClouds/Script/img/2020/11/1/img/v_1.jpg) |
| `V_COOKIE`         | 腾讯视频Cookie                   | 电脑端搜索auth_refresh复制Cookie[图片教程](https://cdn.jsdelivr.net/gh/BlueskyClouds/Script/img/2020/11/1/img/v_2.jpg) |
| `V2EXCK`           | V2EX的Cookie                     | V2EX的Cookie(由于被墙可能会签到失败)                         |
##### 推送通知环境变量(`telegram机器人`)

|       Name        |                                        归属                                        | 属性  | 说明                                                                                                                                                                                                          |
|:-----------------:|:--------------------------------------------------------------------------------:|-----|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|    `SEND_KEY`     |                                       推送开关                                       | 非必须 | 推送开关设置如设置该参数 仅在Cookie失效时推送,不设置则默认全部推送无论是否失败                                                                                                                                                                 |
|  `TG_BOT_TOKEN`   |                                    telegram推送                                    | 非必须 | tg推送(需设备可连接外网),`TG_BOT_TOKEN`和`TG_USER_ID`两者必需,填写自己申请[@BotFather](https://t.me/BotFather)的Token,如`10xxx4:AAFcqxxxxgER5uw` , [具体教程](https://github.com/MayoBlueSky/My-Actions/blob/master/backUp/TG_PUSH.md) |
|   `TG_USER_ID`    |                                    telegram推送                                    | 非必须 | tg推送(需设备可连接外网),`TG_BOT_TOKEN`和`TG_USER_ID`两者必需,填写[@getuseridbot](https://t.me/getuseridbot)中获取到的纯数字ID, [具体教程](https://github.com/MayoBlueSky/My-Actions/blob/master/backUp/TG_PUSH.md)                      |