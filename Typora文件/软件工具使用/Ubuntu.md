###  unburnt 防火墙命令

```shell
ufw status  # 状态
ufw disable # 关闭
ufw enable  #开启 
ufw allow 53 # 允许外部访问53号端口
ufw reload   # 重启
lsof -i:80  # 查看80端口是否开放
```

