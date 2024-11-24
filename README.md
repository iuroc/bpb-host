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
const newWindow = window.open('', '', 'width=500, height=500')
newWindow.document.body.style.margin = 0
const container = newWindow.document.createElement('textarea')
container.value = rules
container.style.display = 'block'
container.style.wordBreak = 'break-all'
container.style.width = '100%'
container.style.height = '100%'
container.style.padding = '30px'
container.style.fontFamily = 'consolas'
container.disabled = true
newWindow.document.body.appendChild(container)
```

## 订阅转换

https://acl4ssr-sub.github.io/
