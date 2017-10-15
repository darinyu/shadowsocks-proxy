
put shadowsocks.json under /etc/ folder


In a screen app (screen -s kcptun), run

sudo ./server_linux_amd64 -c kcp_config.json


Then, run

ssserver -c /etc/shadowsocks.json -d start


In Mac OS, install shadowsocksX-NG, then import export.json file
and correct server_ip


It should work now
