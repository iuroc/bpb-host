# BPB Panel Hosts

## 构建脚本

```javascript
const hosts = `
s1.asrnoor.ir
x.asrnoor.ir
p.asrnoor.ir
f.asrnoor.ir
test.xiao888.us.kg
bwp.ittot.us.kg
anjwang.us.kg
zou886699.us.kg
leon001.ggff.net
bpb.6889692.us.kg
plusmusicsg.vmsys.ggff.net
fcspring.ggff.net
bpb.my79801.com
`
const rules = hosts.split('\n').filter(i => i.trim()).map(host => {
    return `trojan://bpb-trojan@www.vpslook.com:443?security=tls&sni=${host}&alpn=h3&fp=randomized&allowlnsecure=1&type=ws&host=${host}&path=%2Ftr%3Fed%3D2560#${host}`
}).join('\n')
console.log(btoa(rules))
```

## 订阅地址

运行上方脚本，将生成的 Base64 写入到 rules.txt 文件，然后将下面的地址输入到订阅转换工具。

```
https://iuroc.github.io/bpb-host/rules.txt
```

## 订阅转换

https://acl4ssr-sub.github.io/

## 发现域名

[443 端口](https://fofa.info/result?qbase64=aWNvbl9oYXNoPSItMTM1NDAyNzMxOSIgJiYgYXNuPSIxMzMzNSIgJiYgcG9ydD0iNDQzIg%3D%3D)

[80 端口](https://fofa.info/result?qbase64=aWNvbl9oYXNoPSItMTM1NDAyNzMxOSIgJiYgYXNuPSIxMzMzNSIgJiYgcG9ydD0iODAi)

## 参考文章

[批量获取免费的VPN节点，用不完真用不完….. BPB-Worker-Panel 面板BUG利用！！](https://www.freedidi.com/17131.html)
