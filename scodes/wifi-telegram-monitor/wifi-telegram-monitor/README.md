# wifi-telegram-monitor
This script uses Telegram to notify you about the devices connected to your network.<br>

# Installation
This program in meant to be running on the PC connected to the network you want to monitor.

`cd wifi-telegram-monitor` <br><br>
After downloading you have to install dependencies:<br>
`pip install -r requirements.txt`

# Configuration

You need to create a bot via BotFather using the Telegram app to get the access token.<br>
You need to get your user chat id.<br>

You need to create `conf.json` file containing the following config.

```
{
    "TOKEN": YOUR_TELEGRAM_TOKEN,   //str
    "CHAT_ID": YOUR_USER_CHAT_ID,   //str
    "NETWORK": NETWORK_TO_MONITOR,  //str: "192.168.1.0/24"
    "INTERVAL": SCAN_NETWORK_INTERVAL  //int: 60
}
```

# How to use

`python wifi-telegram-monitor.py`
