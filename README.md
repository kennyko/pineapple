# pineapple
A modular, extendible, discord bot framework based on discord.py.

Check out our Trello page for our progress and plans:
https://trello.com/b/tj0OqFwR/pineapple-feature-timeline

# Installation
This guide will be for installing the bot on Ubuntu.

## Creating a bot account

1. Go to [the discord developers page](https://discordapp.com/developers/applications/me)
2. Click New Application
3. Give your bot a name and an icon, then press Create Application
4. On the next page, click Create a Bot User
5. Next to Token, click Click to reveal to see your token
6. Enter your token inside the configuration file for the bot.

## Running the bot

1. Clone the repo locally using `git clone https://github.com/peter765/pineapple.git`.
2. Edit the config.ini.default with the necessary information.
3. Rename config.ini.default to config.ini.
4. Update pip with `python3.5 -m pip install --upgrade pip` for Ubuntu 14.04 or `python3 -m pip install --upgrade pip` for 16.04 and later.
5. Use `pip install -r requirements.txt` to install dependencies.
6. Run the bot using `python3.5 bot.py` for Ubuntu 14.04 or `python3 bot.py` for 16.04 and later.

## Adding the bot to your server

Self hosted bot:
1. Make sure you have Manage Server permissions.
2. go to [the discord developers page](https://discordapp.com/developers/applications/me) and click on your application. At the top, you will find the bot account's Client ID.
3. Replace "CLIENT_ID" in the following link the Client ID from your application page, and then open that URL in a browser.
https://discordapp.com/oauth2/authorize?&client_id=CLIENT_ID&scope=bot&permissions=0
4. Select your server and add the bot to that server

Pre-hosted bot:
Not yet public. Soon(tm)

Bot setup in server:
5. The server owner can add a group to the bot's rank system, use the "addadmin <groupname>" command. The group name is case sensitive.
6. Add other groups to the admin role with "addadmin" or to moderator with "addmod" or to verified member with "addmember"