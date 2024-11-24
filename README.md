# bpb-host

## Script

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

console.log(rules)
```
