---
description: '@nijigemby_helbot'
---

# 🖇 绑定Telegram账号到emby服务器/解绑

[使用Telegram机器人注册](<register via bot.md>)的用户已默认绑定到emby服务器，本篇仅为其他渠道注册的用户使用。

绑定机器人为可选操作，但是说不定呢？

{% embed url="https://t.me/nijigemby_helbot" %}
点击食用
{% endembed %}

首先需要您的emby uid：登陆[emby服务器](http://media.nijigem.by)网页，点击右上角小齿轮⚙️→[应用程序设置](https://media.nijigem.by/web/index.html#!/settings)密码

观察您的地址栏，会有一串类似 `https://media.nijigem.by/web/index.html#!/settings/password.html?userId=`**`****************************`**`&serverId=123456789123456`

**`****************************`**为您的uid



打开[机器人](https://t.me/nijigemby\_helbot)使用命令 `/bind ****************************` 即可完成绑定（前题是您的Telegram账号未绑定或已解绑本emby服务器）

当然直接运行 `/bind https://media.nijigem.by/web/index.html#!/settings/password.html?userId=`**`****************************`**`&serverId=123456789123456` 也可以捏



解绑运行`/unbind`即可

## <mark style="color:red;">uid很重要，请妥善保管</mark>



