# Introduction

```
```

#### 命令

1. 连接远程主机
```
ssh username@8.8.8.8 -p 22
ssh 8.8.8.8 -p 22 -l username
```

2. 本地端口转发
```
ssh -L 8888:6.6.6.6:22 username@8.8.8.8 -p 22
```

3. 远程端口转发
```
将本地 127.0.0.1 的主机的端口 80 转发到 8.8.8.8 主机的 8888 端口
ssh -L 8888:127.0.0.1:80 username@8.8.8.8 -p 22
```

4. 动态端口转发
```
本地实现 socks5 代理
ssh -D username@8.8.8.8 -p 22
```

5. x11 端口转发
```
实现运行图形化程序 , 例如 firefox , burpsuite 等等
ssh -X username@8.8.8.8 -p 22
```
