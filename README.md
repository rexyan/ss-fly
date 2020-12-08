### 拉取代吗
git clone https://github.com/suniceman/ss-fly

### 运行搭建ssr脚本代码
ss-fly/ss-fly.sh -ssr

### 相关操作ssr命令
```
 启动：/etc/init.d/shadowsocks start
 停止：/etc/init.d/shadowsocks stop
 重启：/etc/init.d/shadowsocks restart
 状态：/etc/init.d/shadowsocks status
 配置文件路径：/etc/shadowsocks.json
 日志文件路径：/var/log/shadowsocks.log
 代码安装目录：/usr/local/shadowsocks
```

### 卸载ssr服务
./shadowsocksR.sh uninstall

### 一键开启BBR加速
ss-fly/ss-fly.sh -bbr  装完后需要重启系统，输入y即可立即重启，或者之后输入reboot命令重启.判断BBR加速有没有开启成功。输入以下命令：sysctl net.ipv4.tcp_available_congestion_control 如果返回值为：net.ipv4.tcp_available_congestion_control = bbr cubic reno  后面有bbr，则说明已经开启成功了。
