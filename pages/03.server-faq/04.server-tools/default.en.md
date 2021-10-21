---
title: 'Server Tools'
metadata:
    'og:url': 'https://scpsl-faq.com/en/server-faq/server-tools'
    'og:type': website
    'og:title': 'Server Tools | SCP:SL FAQ'
    'og:author': 'SCP: Secret Laboratory Unofficial FAQ'
    'twitter:card': summary_large_image
    'twitter:title': 'Server Tools | SCP:SL FAQ'
    'article:author': 'SCP: Secret Laboratory Unofficial FAQ'
    'og:image': 'https://scpsl-faq.com/user/themes/quarklight/images/favicon.png'
    description: 'Unofficial SCP:SL FAQ'
    'og:site_name': scpsl-faq.com
    theme-color: '#3BB9FF'
recaptchacontact:
    enabled: false
aura:
    pagetype: website
    metadata:
        'og:site_name': scpsl-faq.com
media_order: 79122823.jpg
---

# **FAQ | Server Tools <i class="fas fa-wrench"></i>**


### This section is made for helping server hosts or developers with modding a server!


***

## **Plugin Frameworks**

#### EXILED
Probably one of the best frameworks for SCP:SL, Here is their description on EXILED's github,

EXILED is a low-level plugin framework for SCP: Secret Laboratory servers. It offers an event system for developers to hook in order to manipulate or change game code, or implement their own functions. All EXILED events are coded with Harmony, meaning they require no direct editing of server Assemblies to function, which allows for two unique benefits. 

* Firstly, the entirety of the frameworks code can be freely published and shared, allowing developers to better understand how it works, as well as offer suggestions for adding to or changing it's features. 
* Secondly, since all of the code related to the framework are done outside of the server assembly, things like small game updates will have little, if any, effect on the framework. Making it most likely to be compatible with future game updates, as well as making it easier to update when it is necessary to do so.

Also if you didn't know EXILED has their own [hosting service](http://exiled.host) for SCP:SL servers with EXILED already installed, Terraria servers, SCP:ET and Minecraft servers!

This is [EXILED's Github](https://github.com/Exiled-Team/EXILED), A lot of information is on it to help new users and plugin developers.

Here is [EXILED's Discord](https://discord.gg/PyUkWTg), They have a lot of helpful channels such as FAQ, Resources, Support channels for normal EXILED users and plugin developers & my favorite channel "tinybrain-sanctum" where you can find some pretty interesting plugins by plugin devs ~~whitenames~~. They also have a category for most plugins made by known EXILED plugin developers.


#### Synapse
This framework is almost a year old and not the most known one, I recently found it and it looks pretty epic, Here is their descripition on Synapse's github,

What is Synapse?

Synapse is a project created by two german official community Server-Hosters. We used Harmony to create a framework which makes us easier to implement new functions, game updates and overall a new experience a player.
Features & Configs

Synapse itself has a ton of features some of these include:

* Permission System which replaces the Permission System of Scp:Sl
* Api to create own Roles
* Api to create own Items
* Api to interact with the Features of Scp:SL
* Database support
* Command System

Synapse created a really cool website with a bunch of info such as changelogs, Documentation for developers, FAQ for new users and more! Website can be viewed [here](https://docs.synapsesl.xyz).

This is [Synapse's Github](https://github.com/SynapseSL/Synapse) which includes a installation guide & section for developers.

This is [Synapse's Discord](https://discord.com/invite/wSBHXwy), They have a good amount of channels such as FAQ, Suggestions for the framework, Known-bugs/bug-report, Support category for both normal Synapse users and plugin developers and a community channel for plugin developers to post tools they created for Synapse. Lastly they have a category for plugins, Official plugins and upcoming plugins!

***

## **Recommended Plugins (EXILED)**

### SCPStats
SCPStats is a plugin providing global and server-specific stat tracking and server management/moderation tools such as Rolesync and Ban Management, [Github here](https://github.com/SCPStats/Plugin).

It allows players to view their server stats (stats specific to your server) as well as their global stats, and how they rank against other players through the [SCPStats Site](https://scpstats.com/) or the [SCPStats Bot](https://top.gg/bot/741924143070707732).
It also provides moderation/management features, such as Rolesync, which helps with giving server members/boosters/donators/staff roles on your server, and a ban management panel ([SCPStats Bans](https://bans.scpstats.com/)).
To set it up, take a look at the [Setup Guide](https://scpstats.com/guides/server).

SCPStats includes the following features:
* Global and server global and server-specific stat tracking.
* Rolesync to give players role on your server based on what roles they have on their discord server, or what stats they have.
* A ban management panel, to help you and your staff manage punishments, as well as allowing you to view a specific player's punishment history.
* Discord-based reserved slots and whitelist, allowing you to give players a reserved slot or whitelist spot based on their roles on your discord server.
* Server status messages including server info and a player list inside of a discord message.
* Hats, which can be used as donator perks.
* Modifying role names to embed stats, such as displaying a player's level next to their role.
* Round summary messages, showing the top players in certain leaderboard for the round (ex. who got the most kills, who escaped first, etc).


### AdminTools
An SCP:SL EXILED plugin that gives server owners fun commands and logging functionality for their servers, [Github here](https://github.com/Exiled-Team/AdminTools).

Features (God this is gonna be long)
- Log commands in your server files!
- Quickly send a message to all staff
- Set AHP of players with ease
- Spawn a SCP-018 ball on players with a jingle when everyone gets a SCP-018 instance
- Break down doors, gates, bulletproof lockers, every door related item in the game
- Cleanup all item pickups and ragdolls from the server manually with ease
- Reload your permission and game config files to ensure nothing goes wrong
- Drop a certain amount of items on players
- Drop an item with a custom size on players
- Spawn a dummy character on players
- Set players to be invisible / in ghost mode
- Set a custom timed Flash grenade, Frag grenade, or SCP-018 ball on players
- Set HP of players with ease
- Grab ID's of players with ease
- Instantly kill any user you see with your weapons
- Drop items from player inventories or see what items players have in their inventory
- Jail users to help with enforicing server rules
- Kick users with custom messages
- Kill players for whatever reason you want
- Quickly send a message to a user
- Mute all users from using voice or intercom with ease
- Get and mofidy positions of players with ease
- Give players the ability to pry gates open
- Randomly teleport users to a random part of the facility
- Give players the ability to regenerate health
- Send players up high in the sky as a rocket and watch them explode
- Scale players hitboxes to whatever you want
- Send a message easily to all staff, a specific user group, or a user
- Change player sizes to whatever you want
- Spawn ragdolls on players
- Spawn a workbench on players
- Remove all items from players instantly with ease
- Show or hide all staff tags instantly with ease
- Teleport all users to a specific user, or a user to another user, with ease
- Set yourself or other users as a tutorial with ease
- Unmute all users from intercom or voice with ease


### DiscordIntegration
A bot and server plugin to allow server logs to be sent to Discord channels, and for server commands to be run via the Discord bot, [Github here](https://github.com/Exiled-Team/DiscordIntegration).

This plugin is really helpful for game logs to see if someone broke a rule or command logs to see if your staff are abusing, Make sure to fully read the install guide on the github since you will need to install nodejs because the Discord bot itself is created with discord.js

Currently on the github it does not say how to create a Discord bot but I created a pull for it, Below is how to create a Discord bot

1. Go to https://discord.com/developers/applications and create a new application.
2. Inside of the application page under "settings" click Bot & build the bot.
3. After creating the bot you can change the bots username and avatar if you wish.

Bot token is located on the Bot page under username, Do NOT share the token because people can control the bot if they get it.


### Common-Utils
Common Utils is a plugin that serves many common utilites in a day to day server life, [Github here](https://github.com/Exiled-Team/Common-Utils).

- Ability to change 914's class upgrading (ex, DClass goes in; scientist comes out.)
- Ability to add custom 914 recipies.
- Ability to completly configure a welcome message.
- Ability to completly configure a broadcast message, this can appear every 'x' amount seconds.
- Ability to add custom inventories to all the main classes.
- Allowing SCP-049 to speak with V
- Autonuke
- Auto cleanup for ragdolls & items
- Custom health values for certain classes
- Health on kill


## **Recommended Plugins (Synapse)**

### MoreTools
MoreTools is a plugin for Scp:SL that add a ton of new Command in order to manage the Server or just having more fun, [Github here](https://github.com/SynapseSL/MoreTools).

- A command which makes you invisible (like SCP-268 but for everyone even spectators)
- Send a TextHint to all players
- jailing system
- Change the walkspeed for players
- Spawning a grenade/flash on players
- And more!


### Syncord
Syncord is there to offer you a way of logging specific Events from within your SCP SL Server to your Discord Server, [Github here](https://github.com/AlmightyLks/Syncord).

Both the bot and plugin use .NET Framework

Below is how to create a Discord bot

1. Go to https://discord.com/developers/applications and create a new application.
2. Inside of the application page under "settings" click Bot & build the bot.
3. After creating the bot you can change the bots username and avatar if you wish.

Bot token is located on the Bot page under username, Do NOT share the token because people can control the bot if they get it.


### BroadcastsPlus
Adds Broadcasts which play over time, [Github here](https://github.com/TheVoidNebula/BroadcastsPlus).

- MOTD that is shown on a player join for the player
- Broadcasts in a given intervall
- C.A.S.S.I.E Announcements in a given intervall
- Manage the Broadcasts/C.A.S.S.I.E Announcements ingame

***


## **Other Tools**

### MultiAdmin

MultiAdmin is a replacement server tool for SCP: Secret Laboratory, which was built to help enable servers to have multiple configurations per server instance, [Github here](https://github.com/ServerMod/MultiAdmin).

- Config Generator: Generates a full default MultiAdmin config file
- Config Reload: Reloads the MultiAdmin configuration file
- Exit Command: Adds a graceful exit command
- Folder Copy Round Queue: Copies files from folders in a queue
- GitHub Generator: Generates a GitHub README file outlining all the features/commands
- Help: Display a full list of MultiAdmin commands and in game commands
- Restart On Low Memory: Restarts the server if the working memory becomes too low
- MultiAdminInfo: Prints MultiAdmin license and version information
- New Server: Adds a command to start a new server given a config folder and a config to start a new server when one is full [Config Requires Modding]
- Restart Command: Allows the game to be restarted without restarting MultiAdmin
- Restart After a Number of Rounds: Restarts the server after a number rounds completed [Requires Modding]
- TitleBar: Updates the title bar with instance based information


! If you have a issue with anything here please contact Denty (Since I made this)
