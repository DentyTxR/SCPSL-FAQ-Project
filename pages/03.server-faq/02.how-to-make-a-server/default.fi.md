---
title: 'How To Make A Server'
metadata:
    'og:url': 'https://scpsl-faq.com/en/server-faq/how-to-make-a-server'
    'og:type': website
    'og:title': 'How To Make A Server | SCP:SL FAQ'
    'og:author': 'SCP: Secret Laboratory Unofficial FAQ'
    'twitter:card': summary_large_image
    'twitter:title': 'How To Make A Server | SCP:SL FAQ'
    'article:author': 'SCP: Secret Laboratory Unofficial FAQ'
    description: 'Unofficial SCP:SL FAQ'
    'og:site_name': scpsl-faq.com
---

# **FAQ | How To Make A Server**

### Before doing anything you need to port forward.

## Windows 10 / PC
Install the SteamCMD from [here](https://steamcdn-a.akamaihd.net/client/installer/steamcmd.zip), This will allow you to install the server from steam, Once downloaded drag the SteamCMD executable into a new folder and run it. 
Upon running it will proceed with the first time setup and you should see Loading Steam API...ok followed by <kbd>Steam></kbd>

Make a new folder somewhere for your server, the recommendation is making a desktop folder and calling it something simple such as <mark>SCP:SL Server</mark>

Head to the SteamCMD and enter the following commands in order,
- <kbd>login anonymous</kbd>
- <kbd>force_install_dir (your server directory where you want to install the server)</kbd>
- <kbd>app_update 996560</kbd>

Your server folder should now contain 17 new files and 5 new folders

Your server is officially created but will need to be configured in order to accept players, Please goto **Server FAQ -> Server Configration** on how to get 
To start the SCP:SL server open the **LocalAdmin.exe** file inside of the server files.



## Linux 
Before we get into this, **Do Not Install The SCP Server On The Root User!!! Make A SCPSERVER User Or Something Else!!!**

First you will need to install **mono** for the server to work, Go [here](https://www.mono-project.com/download/stable/#download-lin-ubuntu) and read the guide on installing mono.

Then you will need to install SteamCMD, Type the following command <kbd>sudo apt install steamcmd</kbd>, That will allow you to connect to Steams servers to install the SCP:SL server.

#### (Optional)

For some people installing SteamCMD might not work with apt, Such as CentOS, And other Linux distros, If you are one of those people you will need to install curl and use curl to install SteamCMD, Type the following command to install curl, <kbd>sudo apt install curl</kbd>

Then you will need to use curl to install SteamCMD, Type the following command, <kbd>curl -sqL "https://steamcdn-a.akamaihd.net /client/installer/steamcmd_linux.tar.gz" | tar zxvf -</kbd>

That will create a folder called <mark>linux32</mark> and a <mark>steamcmd.sh</mark> file.


Now that you have SteamCMD install you will need to type <kbd>steamcmd</kbd>, If you had the issue as above you will need to type <kbd>./steamcmd</kbd>.

Now that you are inside of SteamCMD you will first need to login, Simply type <kbd>login anonymous</kbd>.

Now you will need to set the install directory for the SCP Server, Simply type <kbd>force_install_dir (your server directory)</kbd> replacing <mark>(your server directory)</mark> with the folder of where you want the server installed

Now you can finally install the SCP Server, Yet again simply type <kbd>app_update 996560</kbd>.

Thats it! You have installed the SCP:SL Server! To run the server type <kbd>./LocalAdmin</kbd> followed with the servers port

## How to make the server visible on list? (Verification)

1. Set your email as <kbd>contact_email</kbd> in <kbd>config_gameplay.txt</kbd> (if the line is missing - create it anywhere in this file).
2. Send the following information to server.verification@scpslgame.com
* Public IPv4 of the server (make sure that this IP is working - eg. ask friend to join)
* Is it static or dynamic IP
3. After around 24 hours (sometimes up to 72 hours) you will received message that your server has been verified.
4. Click on the link printed in the server console and agree to the verified server rules.
