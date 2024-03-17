## 简介
最好的内网穿透工具，没什么好解释的了
github：https://github.com/fatedier/frp
中文文档：https://gofrp.org/zh-cn/

## 安装
**安装systemd**
```
apt install systemd
```

创建 frps.service 文件，写入以下内容
```
[Unit]
# 服务名称，可自定义
Description = frp server
After = network.target syslog.target
Wants = network.target

[Service]
Type = simple
# 启动frps的命令，需修改为您的frps的安装路径
ExecStart = /path/to/frps -c /path/to/frps.toml

[Install]
WantedBy = multi-user.target
```

**使用 systemd 命令管理 frps 服务**
```
# 启动frp
sudo systemctl start frps
# 停止frp
sudo systemctl stop frps
# 重启frp
sudo systemctl restart frps
# 查看frp状态
sudo systemctl status frps
```

**设置 frps 开机自启动**
```
sudo systemctl enable frps
```
