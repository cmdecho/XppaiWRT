## Commands

Commands list
 * /aria2add      | Add task
 * /aria2stats    | Aria2 status
 * /aria2pause    | Pause all
 * /aria2resume   | Resume all
 * /oc        | OC Information
 * /proxies   | Proxies status 
 * /rules     | Rule list 
 * /vnstat    | Bandwidth usage 
 * /memory    | Memory status 
 * /myip      | Get ip details 
 * /myxl 087x | MyXL Info
 * /speedtest | Speedtest 
 * /ping      | Ping bot
 * /sysinfo   | System Information

## How To Update XppaiWRT
```shell
git reset --hard
git pull
chmod +x src/plugins/*.sh
```
 
##### Edit `Xppai.WRT` with your own Bot Token
![bottoken](https://i.ibb.co/vP7csgQ/TokenBot.png)
##### Starting Bot
![Startingbot](https://i.ibb.co/mcYqq3S/startbot.png)
##### /start | /cmdlist
![Start cmdlist](https://i.ibb.co/y4wqFwb/cmdlist.png)
##### /memory
![Memory](https://i.ibb.co/cwQ8m1C/memory.png)
##### /myip
![Myip](https://i.ibb.co/PQVB3DH/myip.png)
##### /myxl `number`
![MyXL](https://i.ibb.co/bBMf0rg/myxl.png)
##### /proxies
![Proxies](https://i.ibb.co/0fmXhjX/proxies.png)
##### /rules
![Rules](https://i.ibb.co/8DtrH3n/rules.png)
##### /speedtest `(depend on what speedtest installed)`
![Speedtest](https://i.ibb.co/r3cV90Y/speedtest.png)
##### /sysinfo
![sysinfo](https://i.ibb.co/2tqS3cM/sysinfo.png)
##### /vnstat `-d or -h or -m` 
![sysinfo](https://i.ibb.co/0ycJhvP/vnstat.png)

## Requirements
- git
- screen
- php8-cli
- php8-mod-curl
- Telegram Bot API Token - Talk to [@BotFather](https://telegram.me/@BotFather)

### Install from Terminal

Make sure all requirements is installed on your `OpenWRT`:

```bash
opkg update
opkg install git
opkg install git-http
opkg install php8-cli
opkg install php8-mod-curl
git clone https://github.com/cmdecho/XppaiWRT &&  chmod +x XppaiWRT/src/plugins/*.sh
```

## Usage
### Edit `Xppai.WRT` before running
```
Edit Xppai.WRT with your Bot Token & Bot Username (without @)
```

Start Screen
```shell
screen -S bot
```

Enter XppaiWRT Directory
```shell
cd XppaiWRT
```

Start bot
```shell
php8-cli index.php 
```

Auto Start Bot after reboot / internet off
```
add scheduled tasks
*/5 * * * * cd XppaiWRT && php8-cli index.php
```
