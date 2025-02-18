# BPB Panel Hosts

## 构建脚本

```javascript
const hosts = `
sixbox.ahotapp.com
b.yawuni.us.kg
bpb27.unixtea.com
yw.xn--ghqy4wtm5b.us.kg
ymrb.xiangyanlian.dynv6.net
2412.sun2412.us.kg
bpb1.850425.xyz
anjwang.us.kg
leon001.ggff.net
plusmusicsg.vmsys.ggff.net
`
const rules = hosts.split('\n').filter(i => i.trim()).map(host => {
    return `trojan://bpb-trojan@www.vpslook.com:443?security=tls&sni=${host}&alpn=h3&fp=randomized&allowlnsecure=1&type=ws&host=${host}&path=%2Ftr%3Fed%3D2560#${host}`
}).join('\n')
console.log(btoa(rules))
```

## 订阅地址

1. 运行上面的脚本，生成 Base64 订阅信息
2. 将订阅信息覆盖本仓库的 rules.txt 文件
3. 启用本仓库的 Pages 服务
4. 将订阅地址 `https://iuroc.github.io/bpb-host/rules.txt` 填入订阅转换工具，获得订阅链接

## 订阅转换

[https://acl4ssr-sub.github.io/](https://acl4ssr-sub.github.io/)

## 发现域名

[443 端口](https://fofa.info/result?qbase64=aWNvbl9oYXNoPSItMTM1NDAyNzMxOSIgJiYgYXNuPSIxMzMzNSIgJiYgcG9ydD0iNDQzIg%3D%3D)

[80 端口](https://fofa.info/result?qbase64=aWNvbl9oYXNoPSItMTM1NDAyNzMxOSIgJiYgYXNuPSIxMzMzNSIgJiYgcG9ydD0iODAi)

## 参考文章

[批量获取免费的VPN节点，用不完真用不完….. BPB-Worker-Panel 面板BUG利用！！](https://www.freedidi.com/17131.html)
