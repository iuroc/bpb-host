# BPB Panel Hosts

## 构建脚本

```javascript
const hosts = `
s1.asrnoor.ir
x.asrnoor.ir
p.asrnoor.ir
f.asrnoor.ir
test.xiao888.us.kg
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
