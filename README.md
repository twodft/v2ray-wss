搭建 Shadowsocks-libev， V2ray+ Nginx + WebSocket 和 Reality 代理脚本，支持 Debian、Ubuntu、Centos，并支持甲骨文 ARM 平台。

简单点讲，没域名的用户可以安装 Shadowsocks-libev 和 Reality 代理，有域名的可以安装 V2ray+ Nginx + WebSocket 代理，各取所需。

WSS 代理，443 和 8080 端口都是可用端口，8080 是免流端口，关闭 tls 后，只要在伪装域名里填上运营商免流链接就可以免流了。

运行脚本：

```
wget https://raw.githubusercontent.com/twodft/v2ray-wss/mod/tcp-wss.sh && bash tcp-wss.sh
```

便宜 VPS 推荐：https://hostalk.net/deals.html

![image](https://user-images.githubusercontent.com/13328328/235636662-5df2a97d-dd2c-4ca1-af0d-1b4e69119111.png)

已测试系统如下：

Debian 9, 10, 11

Ubuntu 16.04, 18.04, 20.04

CentOS 7

WSS 客户端配置信息保存在：
`cat /usr/local/etc/v2ray/client.json`

Shadowsocks 客户端配置信息：
`cat /etc/shadowsocks-libev/config.json`

Reality 客户端配置信息保存在：
`cat /usr/local/etc/xray/reclient.json`

卸载方法如下：
https://1024.day/d/1296
