---
title: FAQ
metadata:
    'og:url': 'https://scpsl-faq.com/en/server-faq/faq'
    'og:type': website
    'og:title': 'FAQ | SCP:SL FAQ'
    'og:author': 'SCP: Secret Laboratory Unofficial FAQ'
    'twitter:card': summary_large_image
    'twitter:title': 'FAQ | SCP:SL FAQ'
    'article:published_time': '2020-07-24T13:45:45-04:00'
    'article:modified_time': '2020-07-26T11:10:29-04:00'
    'article:author': 'SCP: Secret Laboratory Unofficial FAQ'
    description: 'Unofficial SCP:SL FAQ'
    'og:site_name': scpsl-faq.com
---

# **Server FAQ | FAQ**



### **1. What should I use to host a server?**
Not your PC for sure, the server is technically "free" but you pay with your parts' lifetime. The best to use is VPS, OVH has a great offer however only servers with the price > $5 will hold the server without problems.

Your second choice is using a hosting, Exiled hosting is the best if there isn't one hosted in your country. If you are from Poland, you can use LiveServer.
You also need to have somekind of DDoS protection, all OVH servers come with free DDoS protection and it hasn't let me down!

!! We recommend you to choose a hosting carefully. There are hosts where users report a lot of problems, never pay for more than one month if it's your first time using this hosting.
### **2. Could not update data on server list (legacy)- Blacklisted IP address (internal).**

Solution 1. Set <kbd>server_ip:</kbd> to auto inside of your gameplay config.
### **3. How do I make myself admin without going into files?**

Type <kbd>adminme</kbd> in client console.
! Command works only on non-dedicated servers (Create Game).

### **4. How do I update my server?**

Open SteamCMD and type the following, 
- <kbd>login anonymous</kbd>

- <kbd>force_install_dir (server directory) </kbd> 

- <kbd>app_update 996560 validate</kbd>

### **5. How do I disable FF Detector?**

Set these to false
> <code>ff_detector_round_enabled: false
> <br> ff_detector_life_enabled: false
> <br> ff_detector_window_enabled: false
> <br> ff_detector_spawn_enabled: false
> </code>

***

# Official Server FAQ
Made by Northwood

!!! Please note, that this FAQ is made by the official Tech Support, not us. We have only added it here, the information may be outdated like every other question.

### **1. MultiAdmin and ServerMod?**
If you want to get more information you can join their [discord](https://discord.gg/8nvmMTr).

* [ServerMod2](https://github.com/Grover-c13/Smod2) is a server side plugin system with a bunch of additional configuration options, bug fixes, security patches and some optimisations built in.
* [MultiAdmin](https://github.com/Grover-c13/MultiAdmin) is a replacement server tool, which was built to help enable servers to have multiple configurations per server instance.

### **2. What’s the command to install or update game server on Linux?**

Follow this guide:[How to make a server](https://scpsl-faq.xyz/server-faq/how-to-make-a-server)

### **3. I get a "Server not verified" message when starting the server. How do I verify my server?**

1. Set your email as <kbd>contact_email</kbd> in <kbd>config_gameplay.txt</kbd> (if the line is missing - create it anywhere in this file).
2. Send the following information to server.verification@scpslgame.com
* Public IPv4 of the server (make sure that this IP is working - eg. ask friend to join)
* Is it static or dynamic IP
3. After around 24 hours (sometimes up to 72 hours) you will received message that your server has been verified.
4. Click on the link printed in the server console and agree to the verified server rules.

### **4. How do I edit config?**

Open up config_gameplay.txt file in
* Windows -> AppData\Roaming\SCP Secret Laboratory\config\<port>
* Linux -> \.config\SCP Secret Laboratory\config\<port>

### **5. How do I color my server name?**

Use styled text - [https://docs.unity3d.com/Manual/StyledText.html](https://docs.unity3d.com/Manual/StyledText.html)

### **6. How do I change server info?**

You need to create new pastebin - https://pastebin.com/
Let’s say the the new pastebin link is - https://pastebin.com/ABC
Then you need to change config_gameplay.txt variable:
<kbd>serverinfo_pastebin_id: ABC</kbd>

Documentation: [http://digitalnativestudios.com/textmeshpro/docs/rich-text/ ](http://digitalnativestudios.com/textmeshpro/docs/rich-text/)

### **7. Where I can find online server list?**

You can find it here: https://servers.scpslgame.com
You can see more info on a specific server by clicking on it!

The server list is ordered as follows:
> 1. Official class score - DESCENDING
>   a) Global official: 3
>     b) Regional official and same continent: 2
>       c) Local official and same country: 1
>         d) Other cases: 0
>           e) Not official and different country: -1
> 2. Distance - ASCENDING
> 3. Server ID (newer servers, have higher IDs) - ASCENDING
> 4. Server port - ASCENDING

TL:DR
> Official server
> <br>	↳ Regional server
> <br>		↳ Distance
> <br>			↳ Server ID (Newer servers are lower on the list.
> <br>				↳ Server port (7777-7784)

### **8. How do I add my email in the config file?**

Open up <kbd>config_gameplay.txt</kbd> file.
Add the following line anywhere in the file and replace value with your email.
contact_email: email@place.network

### **9. My server console is stuck on this:**

You have made a typo in either config_gameplay or config_remoteadmin.
You should try starting server with default config and progressively change next options to see where is the problem.
![](https://cdn.discordapp.com/attachments/468799519811829761/601489595527462912/e55a1cd3a1af846571c8c5cc0cc415a2.png)

### **10. How to add more ranks on the server?**
Open config_remoteadmin.txt.

**Let's say we want to add rank ABC - you need to write it on the list**
> Roles:
> - owner
> - abc

**Next configure it**
> abc_badge: ABC
> <br>abc_color: silver
> <br>abc_cover: true
> <br>abc_hiden: false
> <br>abc_kick_power: 0</kbd>
> <br>abc_required_kick_power: 1

**And assign SteamID/Discord ID to it**
> Members:
> - 7656119801xxxxxxx@steam: abc
> - 16194927652xxxxxx@discord: abc

### **11. Where do I add myself and/or others as an Owner, Admin or Moderator on my servers?**
Open config_remoteadmin.txt

**At the bottom add the SteamID64 or DiscordID (Get it [here](https://steamid.xyz)) from the users that you want to give access like this**
> Members:
>  - 7656119801009xxxx@steam: owner
>  - 7656119811115xxxx@steam: admin
>  - 7656119804579xxxx@steam: moderator
>  - 7656119813399xxxx@steam: moderator
>  - 10291198045579xxxx@discord: moderator
>  - 19261198113919xxxx@discord: moderator

!! Make sure to remove the  "SomeSteamId64" placeholders!

### **12. As a server owner, what colours can I use for role tags?**

##### List of Colors

| Color                        | Sample                        | Restricted 
| :-------------------------- | :---------------------------: | -------------------: |
| gold                          | {c:#EFC01A}█████{/c} | Yes
| teal                           | {c:#008080}█████{/c} | Yes
| blue                          | {c:#005EBC}█████{/c} | Yes
| purple                       | {c:#8137CE}█████{/c} | Yes
| light_red                   | {c:#FD8272}█████{/c} | Yes
| silver_blue              | {c:#666699}█████{/c} | Yes
| police_blue             | {c:#002DB3}█████{/c} | Yes
| pink                          | {c:#FF96DE}█████{/c} | 
| red                           | {c:#C50000}█████{/c} | 
| brown                      | {c:#944710}█████{/c} | 
| silver                       | {c:#A0A0A0}█████{/c} | 
| light_green              | {c:#32CD32}█████{/c} | 
| crimson                   | {c:#DC143C}█████{/c} | 
| cyan                        | {c:#00B7EB}█████{/c} | 
| aqua                       | {c:#00FFFF}█████{/c} | 
| deep_pink              | {c:#FF1493}█████{/c} | 
| tomato                    | {c:#FF6448}█████{/c} | 
| yellow                     | {c:#FAFF86}█████{/c} | 
| magenta                 | {c:#FF0090}█████{/c} | 
| blue_green             | {c:#4DFFB8}█████{/c} | 
| orange                    | {c:#FF9966}█████{/c} | 
| lime                        | {c:#BFFF00}█████{/c} | 
| green                      | {c:#228B22}█████{/c} | 
| emerald                  | {c:#50C878}█████{/c} | 
| carmine                  | {c:#960018}█████{/c} | 
| nickel                      | {c:#727472}█████{/c} | 
| mint                        | {c:#98FB98}█████{/c} | 
| army_green            | {c:#4B5320}█████{/c} | 
| pumpkin                 | {c:#EE7600}█████{/c} | 

**What are restricted colors?** _They are used in Game Staff badges, if you try to use them on your own server - they will not be visible._
![](https://cdn.discordapp.com/attachments/468799519811829761/601490386569003019/Colors.png)

### **13. I have problems with missing permissions after update.**

You should add the following options to the config_remoteadmin.txt and customize them.

https://en.scpslgame.com/index.php?title=Docs:Permissions

### **14. Config Gameplay Settings**

#### A) Main Server Settings

> server_name: The name of the server. (Default: My Server Name)
> 
> serverinfo_pastebin_id: The Pastebin id for the info section of your server (https://www.pastebin.com). This supports Unity Rich Text Formatting (https://docs.unity3d.com/Manual/StyledText.html). (Default: 7wV681fT)
> 
> server_ip: The ip of your server, you can leave it as auto or set it to your external IPv4 address (http://www.whatsmyip.org). (Default: auto)
> 
> max_players: The maximum amount of players that can play in your server. (Default: 20)

#### B) Spawn Settings

> minimum_MTF_time_to_spawn: The minimum amount of seconds for a MTF spawn. (Default: 280)
> 
> maximum_MTF_time_to_spawn: The maximum amount of seconds for a MTF spawn. (Default: 350)
> 
> ci_respawn_percent: The percentage chance that CI will spawn instead of MTF. (Default: 35)
> 
> ci_on_start_percent: The percentage chance that CI will spawn on match start. (Default: 10)
> 
> team_respawn_queue: The classes able to respawn (Do not change this unless if you know how it works, as it can break MTF and CI respawns). (Default: 40143140314414041340)
> 
> contact_email: The email that SCP:SL staff can use to contact you (if need be). This is required for server verification.

#### C) Pocket Dimension Settings

> pd_random_exits: Whether the Pocket Dimension should use random exits instead of SCP-106s spawn room. (Default: false)
> 
> pd_exit_count: The amount of exits in the pocket dimension. (Default: 2)
> 
> pd_random_exit_rids: The Room IDs that should be used if pd_random_exits is set to true.
> 
> pd_random_exit_rids_after_decontamination: The Room IDs that should be used if Light Containment has decontaminated and pd_random_exits is set to true.
> 
> pd_refresh_exit: Whether the server should refresh the exit door location(s) after someone escapes the Pocket Dimension. (Default: false)

#### D) Miscellaneous Gameplay Settings

> intercom_cooldown: The amount of time the intercom cannot be activated once used. (Default: 120)
> 
> intercom_max_speech_time: Maximum amount of time the intercom can be used before cooldown. (Default: 20)
> 
> auto_round_restart_time: Amount of time after end-game for round restart to occur. (Default: 10)
> 
> friendly_fire: Whether players of the same class can damage each other. (Default: false)
> 
> warhead_tminus_start_duration: Amount of time (seconds) before onsite warhead detonates once activated. (Default: 90)
> 
> human_grenade_multiplier: The multiplier of damage grenades do towards human classes. (Default: 0.7)
> 
> scp_grenade_multiplier: The multiplier of damage grenades do towards SCPs. (Default: 1)
> 
> lock_gates_on_countdown: Whether the entrance and light containment gates lock open during onsite warhead countdown. (Default: true)
> 
> server_forced_class: The class forced on match start. Setting this to -1 means the starting class will be random. (Default: -1)
> 
> map_seed: The map layout each round. Setting this to -1 means the map will be random each match. (Default: -1)

### **15. Config Remote-Admin Settings**

#### A) Server Role Permissions

Permissions: The permissions of all the roles. For multiple roles, add a comma and space before the next role (e.x. xxxx, xxx). 
<br> The list of permissions and formatting is below.

> Permissions:
>  - KickingAndShortTermBanning: [xxxx, xxxxxx, xxx]
>  - BanningUpToDay: [xxxxxx, xxx]
>  - LongTermBanning: [xxxxx]
>  - ForceclassSelf: [xxxx]
>  - ForceclassToSpectator: [xxxxxx, xxx]
>  - ForceclassWithoutRestrictions: [xxxxxx, xxxxx, xxx]
>  - GivingItems: [xxxx, xxx]
>  - WarheadEvents: [xxxxx]
>  - RespawnEvents: [xxxxxx, xxxxxx]
>  - RoundEvents: [xxxxxx]
>  - SetGroup: [xxxx, xxxxxx, xxx]
>  - GameplayData: [xxxxxx]
>  - Overwatch: [xxxxxx]
>  - FacilityManagement: [xxxx, xxxxxx, xxx]
>  - PlayersManagement: [xxxx, xxxxxx]
>  - PermissionsManagement: [xxx]
>  - Noclip: [xxxx]

#### B) Miscellaneous Remote Admin Configuration Settings

> xxxx_badge: The text displayed in-game for badge of the role specified (i.e. this_badge, moderator_badge, xyz_badge, etc.)
> 
> xxxx_color: The color of the specified role's in-game badge. A list of colors can by found in server-faq 12.
> 
> xxxx_cover: Whether the specified role's in-game badge covers Global Badges (if applicable).
> 
> xxxx_hidden: Whether the the specified role's badge in game is hidden by default.
> 
> enable_staff_access: Whether SCP Secret Laboratory Studio Staff and Studio Developers should have Remote Admin access on your server. (Default: false)
> 
> enable_manager_access: Whether SCP Secret Laboratory Studio Directors and Managers should have Remote Admin access on your server. (Default: true)
> 
> enable_banteam_access: Whether the SCP Secret Laboratory Global Banning Team should have Remote Admin access on your server. This is required to be set to true for your server to be verified and appear within the server list. (Default: true)
> 
> override_password: The password used for Remote Admin access without a role set inside config_remoteadmin. Set to none to disable. (Default: none)
> 
> override_password_role: The role given upon using the correct override password. (Default: owner)

### **16. How do I change the amount of memory allocated to my server?**
This is only possible with MultiAdmin which you can download on the smod discord.

* Next to the MultiAdmin.exe file,  create a file <kbd>called scp_multiadmin.cfg</kbd> if it doesn't already exist.
* Add the line max_memory [value in MB]

ex:  <kbd>max_memory: 4096</kbd>
This would allocate 4GB of ram to your server.

### **17. I'm running my server on a Linux distribution other than Ubuntu or Debian and i'm getting SSL errors**

Make sure that:
1. Curl is installed
2. /etc/ssl/certs/ca-certificates.crt exists. If this file doesnt exist run the following command: 
mkdir -p /etc/ssl/certs && ln -s (Your distributions certificate store, look below) /etc/ssl/certs/ca-certificates.crt

Certificate store locations for different distributions:
> * "/etc/pki/tls/certs/ca-bundle.crt"                  // Fedora/RHEL 6
> * "/etc/ssl/ca-bundle.pem"                            // OpenSUSE
> * "/etc/pki/tls/cacert.pem"                           // OpenELEC
> * "/etc/pki/ca-trust/extracted/pem/tls-ca-bundle.pem" // CentOS/RHEL 7

For example on Fedora the command would be "mkdir -p /etc/ssl/certs && ln -s /etc/pki/tls/certs/ca-bundle.crt /etc/ssl/certs/ca-certificates.crt"

Although this fix should work distributions other than Ubuntu are not officially supported by Unity or SCP:SL. A guaranteed way to fix problems such as this is to move to Ubuntu.

### **18. How do I portforward?**

The way you portforward can depend on what type and brand of router you have so there is no straightforward answer for this question. You can either: 
1. Google "how to portforward on (my router name here)"
2. Watch this video: [https://www.youtube.com/watch?v=ExrSULINq9c](https://www.youtube.com/watch?v=ExrSULINq9c)
3. Read this guide [https://www.lifewire.com/how-to-port-forward-4163829](https://www.lifewire.com/how-to-port-forward-4163829)

! Beyond this we cannot help you with portforwarding, you have to do this part yourself so please do not contact tech support members about it as we will only tell you to re-read this FAQ.

### **19. How do I update my server?**
It's actually surprisingly simple to update your server to MP2.
Just follow these steps:
1. Open SteamCMD
2. Type: <kbd>login anonymous</kbd>
3. Type: <kbd>force_install_dir (install directory)</kbd>
4. Type: <kbd>app_update 996560 validate</kbd>
5. When that's done type <kbd>exit</kbd> and you're all done

### **20. How do I make a server?**
The following links are guides that will show you how to create a server and get it on the public server list.

Windows > https://steamcommunity.com/sharedfiles/filedetails/?id=1940790742
Linux   > https://steamcommunity.com/sharedfiles/filedetails/?id=1940772492

### **21. I keep getting the message "The specified host is not available" trying to connect to my server.**

**Before all**
<br>Make sure the server is up to date and isn't using smod
<br>Make sure the server has fully loaded, ie. the last console message should be "Waiting for players..."

#### Connecting
* Hosted on the same PC the game is played on -> connect using localhost or 127.0.0.1 as the IP
* Hosted on a different PC in the same LAN -> connect using the host PC's internal IP
* Hosted on a VPS or something outside your LAN -> connect using the server's external IP

#### Config
* ipv4_bind_ip: 0.0.0.0 - It's best to leave this as 0.0.0.0 but can be set to your machines LOCAL IP. If you have a VPS/VDS this can also be set to your external IP
* ipv6_bind_ip: :: - ALWAYS Leave this setting as it is.
* server_ip: auto - This can also just be left as auto however it can be set to your server EXTERNAL IP

#### "Still doesn't work"
* Allow LocalAdmin (or MultiAdmin) through your firewall and/or antivirus
* Port-forward it properly, see server-faq 18
* Make sure there are no ghost processes running you can do this by looking for the in task manager (top/htop on Linux) or restarting the machine.

!!! If you're currently running on an LTE network (mobile network connection) your ISP may be blocking certain connections. You can check with their support to see if this is the case. 

### **22. My configs dont work! / I want an easier way to edit configs.**
You can use this nifty little program to edit your configs within a comfortable GUI [https://github.com/Takail/Omicron](https://github.com/Takail/Omicron/releases).
<br> Download then extract "Release.rar".

If you have any issues with the program be sure to contact @Takail#6969 for help with it.
