# debian9安装shadowsocks

```
apt-get update
apt-get install net-tools
apt-get install shadowsocks
cd /etc/shadowsocks
vi server.json
# backup the server.json. The file is for the shadowsocks server
# change the password and port for you or add some with json format
ssserver -d start -c server.json
# or
ssserver -d start -c /etc/shadowsocks/server.json
# for stop
ssserver -d stop
# restart
ssserver -d restart -c server.json

```

## server.json

```
{
 "server": "::",
"timeout": 300,
"method": "aes-256-cfb",   //默认，也可以根据自己需求改
"port_password": {"your_port":"your_password"}}

```
