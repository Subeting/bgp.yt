---
description: ⚠️⚠️⚠️请仔细阅读免责声明
---

# 🎖 破解Premium授权

安装证书有风险

思路就是做一个假的mb3admin站点来返回认证信息。

${伪站IP地址}=njigem.by的IP

修改hosts文件，添加两行内容

```
// 新开一行
${伪站IP地址}         mb3admin.com
${伪站IP地址} www.mb3admin.com
```

Windows：下载根证书，安装证书→**本地计算机**→将证书放入下列存储→**受信任的根证书颁发机构**

其他：类似Charles证书的安装方法，详情自行百度不赘述

