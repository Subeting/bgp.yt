---
description: 速度因人而异，请按照自己的真实情况
---

# 🎈 优选服务器IP

### 不会有安全风险，但是请按照自身情况获取可用IP

**使用第三方软件👉** [**XIU2/CloudflareSpeedTest**](https://github.com/XIU2/CloudflareSpeedTest/releases/)



`CloudflareST -f ip.txt -dn 20 -p 5 -url https://jp-mirror.pinochet.tk/`

`CloudflareST -f ipv6.txt -dn 20 -p 5 -url https://sg-mirror.pinochet.tk/1gb.test`

`CloudflareST.exe -o "result_hosts.txt" -url https://download-proxy.zhaofengying.com/api/download?url=http://speedtest-sfo3.digitalocean.com/1gb.test -dn 20`

本处仅为示例，更多功能请参考👆的GitHub repo

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption><p>获取到优选的Cloudflare IP</p></figcaption></figure>



### 懒人包：

```
/////////请确认您的网络是否支持IPV6///////////////
//// 电信：
2606:4700:10::6814:f3c
2606:4700:10::6814:105f
2606:4700:10::6814:10e8
2606:4700:10::6814:14b6
198.41.194.217
104.22.79.212
172.64.49.110
104.24.28.80

//// 移动：
2606:4700:a0:c745:830c:d7bc:67ba:2c5
2606:4700:a0:c745:830c:d788:db63:d961
2606:4700:a0:c7bf:b8e9:3152:c2d4:152c
2606:4700:90:0:31ca:bf4c:2729:517d
2606:4700:90:0:2f6b:6f38:136d:5e5a
2606:4700:90:0:3626:d0ff:6957:de1
172.64.156.31
172.64.156.68
172.64.156.129

//// 联通：
104.20.27.7 
162.159.136.66
172.67.71.209
104.26.0.8
172.67.64.136
172.65.224.86

//// 台湾hinet(三网走台湾hinet)
104.29.64.37
```



然后修改hosts文件，新建一行：**`优选的IP media.nijigem.by`**

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption><p>记事本打开页面</p></figcaption></figure>

至于借用某些机场移动转发的CF，这种太刑了，不做推荐。
