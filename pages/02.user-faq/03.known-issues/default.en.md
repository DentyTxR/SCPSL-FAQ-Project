---
title: 'Known Issues'
metadata:
    'og:url': 'https://scpsl-faq.com/en/user-faq/game-requirements'
    'og:type': website
    'og:title': 'Known Issues | SCP:SL FAQ'
    'og:author': 'SCP: Secret Laboratory Unofficial FAQ'
    'og:image': 'https://scpsl-faq.com/user/themes/quarklight/images/favicon.png'
    'twitter:card': summary_large_image
    'twitter:title': 'Known Issues | SCP:SL FAQ'
    'article:author': 'SCP: Secret Laboratory Unofficial FAQ'
    description: 'Unofficial SCP:SL FAQ'
    'og:site_name': scpsl-faq.com
    theme-color: '#3BB9FF'
---

<head>
    <script async src="https://arc.io/widget.min.js#fcrqEmJg"></script>
</head>

## User FAQ | Known Issues

***

!!! If the solutions here do not work please join the official SCP:SL Discord [here](discord.gg/scpsl) and ask the tech support

##### **Server list response has expired! Set correct time and timezone on your PC**
DST (Daylight Savings) causes the issue, change your timezone by 1 hour forward or behind to fix it.


#### **"Publisher/ASN ban or Spoofer Detected"**
Check out this article https://steamcommunity.com/app/700330/discussions/0/3061870378081558108/


##### **Game started but not loading!!!**
Just wait for the game to launch, This is a known issue with the AC. If you have a SSD we suggest that you install the game on that.


#### **My game is refusing to launch, but I meet the minimum requirements**
 * Solution 1. Check if you have a folder named SCP Secret Laboratory in your Roaming folder, You can access this by hitting Windows Key + r and typing in %appdata%. If it is not there, create a folder named SCP Secret Laboratory and launch the game again.
 * Solution 2. If that does not work and install [this](https://aka.ms/vs/16/release/vc_redist.x64.exe)


#### **“Client failed to authenticate in time”**
 * Solution 1. Inside of the client console <kbd>(`) or (~)</kbd> and type the command <kbd>ar</kbd>
 * Solution 2. In the games launch options (Steam->library->right-click SCP:SL->properties) and add <kbd>-httpproxy</kbd>
    * If that does not work, Please replace <kbd>-httpproxy</kbd> with <kbd>--unitywebrequest</kbd>, If that doesnt work replace it with <kbd>-unitywebrequestdispatcher</kbd>


#### **Connection lost (Timed out)**
This is usually caused by having a bad internet connection, If your internet speeds are fine and it happens on all servers please open a ticket in the official SCP:SL Discord [here](discord.gg/scpsl)


#### **Stuck on connecting to central servers/No Servers Available**
Try disabling all unused network adapters by going to Control Panel, clicking on "Network and Internet", click on "Network and Sharing Center", and on the left hand side you will see "Change adapter settings", click on that and it will bring you to a list of network adapters, Right click on any unused ones (Ex. VMWare, VirtualBox, etc.) and hit disable.




##### **Game keeps crashing on Windows 7**
Windows 7 is unsupported, Please upgrade to 8.1 or 10.


##### **The game does not work on Linux**
The game is **not** supported on Linux.