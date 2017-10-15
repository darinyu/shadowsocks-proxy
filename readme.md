
# Server-side set up

## Requirement

* linux server
* connect to internet

## How to set up

1. Put `shadowsocks.json` under `/etc/` folder
2. Initiate screen by doing `screen -s kcptun`
3. Copy `kcp_config.json` file into current folder
4. In the screen process, start up `kcptun` with `sudo ./server_linux_amd64 -c kcp_config.json`
5. Detach from screen and run `ssserver -c /etc/shadowsocks.json -d start`

# Client-side set up

## Mac OS
 1. Install `shadowsocksX-NG`
 2. Import `export.json` and modify `server_ip`
 3. Turn on `shadowsocks` with your config
 4. Verify by checking your ip. If it matches `server_ip`, then you are good

## Windows
 * [This might work](https://github.com/shadowsocks/shadowsocks-windows)
