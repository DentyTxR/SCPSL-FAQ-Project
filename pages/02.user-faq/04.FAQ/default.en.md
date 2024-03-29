---
title: FAQ
media_order: ezgif-6-264b1c1ccfb1.gif
published: true
metadata:
    'og:url': 'https://scpsl-faq.com/en/user-faq/faq'
    'og:type': website
    'og:title': 'FAQ | SCP:SL FAQ'
    'og:author': 'SCP: Secret Laboratory Unofficial FAQ'
    'og:image': 'https://scpsl-faq.com/user/themes/quarklight/images/favicon.png'
    'twitter:card': summary_large_image
    'twitter:title': 'FAQ | SCP:SL FAQ'
    'article:author': 'SCP: Secret Laboratory Unofficial FAQ'
    description: 'Unofficial SCP:SL FAQ'
    'og:site_name': scpsl-faq.com
    theme-color: '#3BB9FF'
visible: true
---

<head>
    <script async src="https://arc.io/widget.min.js#fcrqEmJg"></script>
</head>


# **User | FAQ**


### **"Publisher/ASN ban or Spoofer Detected" error/Global ban**

Simply vist the site [here](https://steamcommunity.com/app/700330/discussions/0/3061870378081558108/) and **READ**, If you have a global ban you can try to appeal it [here](https://support.scpslgame.com/ban-appeal)


### **This server requires authentication from central server.**
#### This usually happens when your authentication token which is used to join a server gets expired or just didn't get assigned to you, Below are solutions.
Solution 1. Restart the Game or Steam, Or open Task Manager and close all the SCP:SL processors.
    
Solution 2. Open the client console by clicking <kbd>`</kbd> or <kbd>~</kbd> on your keyboard and type <kbd>ar</kbd> and press <kbd>Enter</kbd> on your keyboard

Solution 3. (This for steam) Change the launch game option by doing a right click on SCP:SL **Properties => Set launch options**, Then add <mark>-fdiscord</mark> in the launch option, By adding <mark>-fdiscord</mark> it will force the authentication server from Steam to Discord, Below is a gif to show you how. 

![](ezgif-6-264b1c1ccfb1.gif)

Solution 4. If you still can not fix the issue check to see if the authentication servers are down by [clicking here](https://status.scpslgame.com/).



### **Server List has an invalid signature.**
​
Solution 1. Restart the game/PC
​
​
​
​
### **No Translation**
​
Solution 1. Remove translation files from <kbd>Steam\steamapps\common\SCP Secret Laboratory\Translations</kbd> and verify your files.

***

# Official User FAQ
Made by Northwood

!!! Please note, that this FAQ is made by the official Tech Support, not us. We have only added it here, the information may be outdated like every other question.

### **1. What are the default keybinds?**

* W, A, S, D -  Movement controls: W - Forward, A - Left, S - Backward, D - Right
* E - Interact
* C - Silent walk
* [SPACE] - Jump
* [TAB] - Inventory
* [LMB] - Shoot
* [RMB] - Aim
* M - Remote Admin Console
* N - Toggle Player List
* Q - Voice Chat Activation
* R - Weapon Reload
* V - Special Ability

### **2. Game Requirements**

Head over to [Game Requirements](https://scpsl-faq.xyz/en/user-faq/game-requirements) Page in order to check the game requirements.

### **3. My game crashes after I join a server or start the game!**

Solution 1. 
> Make sure that your pc meets the minimum requirements for the game.
> Turn off Fast Menu. (Steps to do so in point 11 )
> Close all unnecessary programs and applications. 
> Verify your game files on steam.

### **4. I'm getting kicked from servers**

* Check that Steam is running
* Check that Steam is in online mode
* The server has reserved slots and may be full
* You may of been banned by the server administrator

Solution 1.
> * Verify the integrity of your game files (Steps in point 6)
> * Run the game through Steam and not it’s executable
> * Restart Steam
> * Restart your PC

Solution 2.
> * Go to Program Files/Steam/steamapps/common/SCP Secret Laboratory
> * Right-click SCPSL.exe
> * Click Properties
> * Go to the Compatibility tab
> * Check "Run as Administrator"
> * Hit Change for all users
> * Start the game via your Steam Library
 
### **5.  I'm being kicked because of VAC ERROR!**

> This occurs when your PC is put to sleep or hibernation mode and is caused by VAC issue, you can fix it by just turning off your PC and turning it on again and when you launch your game you should not see the error anymore. If that doesn't help disable your antivirus. 
> There is one more solution if the previous to didn't help. Close steam, go to CMD (Windows + R > CMD) and put this command in with your steam localisation: 
> “C:\Program Files (x86)\Steam\bin\SteamService.exe” /repair.

!!! Steam has maintenance every Tuesday, if you experience difficulty with the game please wait 10-30 minutes!

### **6. How do I verify my game files?**

> * Go to your Library in the Steam app
> * Right-click on SCP: Secret Laboratory and select "Properties" at the bottom of the list
> * Click on the "Local Files" tab
> * Click "Verify Integrity of Game Files"

### **7. Why is my character moving without input?**

> * Disconnect any controllers you may have connected.
> * Uninstall a program called "vJoy"

### **8. How can I play the beta version of the game?**

> Steam Library > SCP: Secret Laboratory > Properties > BETA and choose from menu: “beta – Public beta branch"

### **9. How can I play the scpsl_first_version_on_steam beta?**

> Follow the steps in 8  but select "first_version_of_sl_published_on_steam" instead of the public beta branch, then if it doesn’t work, follow these steps:
> * Switch to the branch 
> * Navigate to local files 
> * Rename <kbd>SCP Secret Laboratory.exe</kbd> to <kbd>SCPSL.exe</kbd> 
> * Delete <kbd>SCPSL_Data</kbd> 
> * Rename <kbd>SCP_Secret Laboratory Data</kbd> to <kbd>SCPSL_Data</kbd>
> * Launch game through steam

### **10. Where should I post bugs that I found?**

> If you experience a bug you can report it here: https://staff.scpslgame.com/forms/reportbug.php
> If you are experiencing map generator bugs, remember to include the SEED.
> Current stable version is 9.1.3

### **11. If you're having issues getting back into the game after changing some graphics settings:**

> You can run this program to reset your settings:
> https://cdn.discordapp.com/attachments/422385982235475968/716220084414185562/ResetSettings.bat

! The link will only work if you are a member of SCP:SL Official Discord. 

### **12. Why is the server list not showing up? Why am I getting disconnected?**

> To fix server list not showing up and/or disconnecting from timeouts, navigate to your <kbd>%AppData%\SCP Secret Laboratory\Internal</kbd> and delete CentralServers, then relaunch your game.
> 
> If this doesn't work try turning off any active anti-virus and installing Malwarebytes from: https://www.malwarebytes.com/mwb-download/thankyou/
> Once Malwarebytes is installed run a full scan and quarantine any detected threats.
 
### **13. Why is my screen black?**

> Depending on which hardware you run, please try the following:
> Intel:
> * Intel Control panel and switch the 'Scaling' option from "Maintain Display Scaling" to "Maintain Aspect Ratio"
> Nvidia:
> * Nvidia Control Panel. Change "Aspect ratio" to "No scaling" on the Adjust desktop size and position page (with "perform scaling on Display")
> AMD:
> * AMD Radeon settings and under "Display" change scaling mode from "preserve aspect ratio" to "full panel"
> This can also occur when your PC doesn’t meet minimum requirements.

### **14. My Voice Chat is not working!**

> The first thing to check is if your mic is set as your default device. to do that follow this guide:\
> [Changing default sound input device in Windows 10](https://www.tenforums.com/tutorials/111310-change-default-sound-input-device-windows-10-a.html)
> 
> If the above doesn't work also make sure that "Exclusive mode" is disabled on your mic. Follow this guide to do that:
> [How do I turn off exclusive mode for a Windows Audio Playback Device](https://audible.custhelp.com/app/answers/detail/a_id/9463/~/how-do-i-turn-off-exclusive-mode-for-a-windows-audio-playback-device%3F)
> 
> If the above 2 do not help installing mono can fix this issue. To install mono simply:
> 1. Right click SCP:SL in Steam and click properties.
> 2. Navigate to the "Local Files" tab.
> 3. Click the "Browse Local Files" button
> 4. Run the file named "mono" or "mono.msi" if you have file extensions turned on. (Do not run monoinstall.vdf)
> 5. Go through the mono install wizzard and when it's finished restart your PC.
> 
> If you still have no voice chat, look at your log from point 15 and you find this: 
> * "Important system file that is needed for voice chat is missing, please install all windows updates." You have to install the updates either by using Windows Update tool and installing all updates (preferred), or by > installing them manually.

> One last thing you can try is to go to the games folder, open the SCPCL_Data folder and delete AudioPluginDissonance then verify the games integrity.

### **15. How do I find my player log?**
> 
> Player log:
> * Steam Library > SCP: Secret Laboratory > Properties > Local Files > Browse local files
> * Run the windows batch file titled ‘log.bat’
> * The output log will be a text file titled ‘Player.log’

### **16. Where I can find translations repository?**
> 
> https://github.com/northwood-studios/SCPSL-Translations

### **17. I've received the message: The ASN you are connecting from is globally blocked or You have been globally banned: Proxy has been detected.**
> 
> If you have received an error message similar to one of these when joining a server, it means that the ASN you are connecting from has been globally banned. In order to no longer receive this message when > connecting to a server, you must meet at least ONE (1) of the following criteria:
> 1. Level account must not be 0. (Requires a public profile)
> 2. Your account age must be older than 2 months. (Requires a public profile)
> 3. You must have had SCP: Secret Laboratory in your steam library for greater than 2 weeks.
> 4. You must not have a VPN enabled. (or any other IP changing software)
> 
> You have been globally banned: Unauthorized. or You have been globally banned: Missing Steam Profile.
> If you are receiving this message when connecting to a server, it means that you have not set up your steam profile. Make sure that you have set your profile up correctly.
> https://www.reddit.com/r/Steam/comments/6ppu1y/how_to_setup_steam_profile/
> 
> You have been globally banned: Publisher Ban.
> If you are receiving this message, it means that you have been globally banned from the game, and will be unable to play on any public server. If you wish to appeal your ban, please visit this link for more information: https://scpslgame.com/Ban_Policy.pdf

### **18. I keep timing out while trying to connect to a server.**

> Doing a clean re-install can solve this problem, to do a clean re-install follow these steps:
> 1. Uninstall the game in Steam
> 2. Follow the process in user-faq 11
> 3. Delete C:\Users\(your username)\AppData\Roaming\SCP Secret Laboratory
> 4. Delete C:\Users\(your username)\AppData\LocalLow\Hubert Moszka
> 5. Restart your PC
> 6. Install the game on steam again


***

![](https://cdn.discordapp.com/attachments/716067178939416617/746830105338445925/haha_message_go_brrr.png)
