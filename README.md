# discord-uptime
Discord bot to monitor uptime and ping addresses

Built using discord.py and ping3 libraries

## Installation
**Requires Python 3.6+, tested with 3.7**

Install dependencies: 

`pip install -r requirements.txt`

Bot setup (Rename config.example.json and edit the default values):
* `token` - Discord bot token
* `notification_channel` - Channel ID where down/up notifications will be sent
* `role_to_mention` - Role ID which will be tagged in down/up notifications
* `secs_between_ping` - How many seconds between each uptime check

Servers setup:

To add more servers to ping, simply add a new object and specify the `name` and `address` in servers.json

## Commands
> Default Prefix: >

* `ping <address> [pings]` - Pings an address once, or for the amount specified via pings
* `status` - Displays the status of all servers

## Screenshots
> Status Command

![status](https://i.gyazo.com/7a7a72ecea79b38410ca114fe8719952.png)
> Uptime & Downtime Notifications

![uptime](https://i.gyazo.com/92a3d1e8119751fd7f128606d246911c.png)