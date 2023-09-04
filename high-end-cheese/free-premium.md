---
description: 伪授权
---

# 免费开启高级emby功能

```
server {
    listen 443 ssl;
    server_name mb3admin.com;

    ssl_certificate /home/ssl/emby.crt;
    ssl_certificate_key /home/ssl/emby.key;
    add_header Access-Control-Allow-Origin *;
    add_header Access-Control-Allow-Headers *;
    add_header Access-Control-Allow-Method *;
    add_header Access-Control-Allow-Credentials true;
    location /admin/service/registration/validateDevice {
        default_type application/json;
        return 200 '{"cacheExpirationDays": 3650,"message": "Device Valid","resultCode": "GOOD"}';
    }

    location /admin/service/registration/validate {
        default_type application/json;
        return 200 '{"featId": "","registered": true,"expDate": "2099-01-01","key": ""}';
    }

    location /admin/service/registration/getStatus {
        default_type application/json;
        return 200 '{"planType": "Lifetime", "deviceStatus": 0, "subscriptions": []}';
    }

    location /admin/service/appstore/register {
        default_type application/json;
        return 200 '{"featId": "","registered": true,"expDate": "2099-01-01","key": ""}';
    }

    location /emby/Plugins/SecurityInfo {
        default_type application/json;
        return 200 '{"SupporterKey": "", "IsMBSupporter": true}';
    }
    location /{
        proxy_redirect off;
        proxy_pass https://mb3admin.com;
        proxy_ssl_protocols TLSv1.3 TLSv1.2;
        proxy_ssl_server_name on;
        proxy_ssl_name mb3admin.com;
        proxy_http_version 1.1;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection "upgrade";
        proxy_set_header Host mb3admin.com;

        # Show realip in v2ray access.log
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
    }
}
```

更换hosts请自行百度或参考[优选服务器IP](<../high end cheese/CF IP choosing.md>)，添加hosts记录为`您的IP mb3admin.com`



本站提供证书与伪站IP。

[点击下载伪站证书](https://bgp.yt/.public/myCA.crt)（风险自负）

伪站IP: `209.141.38.134`
