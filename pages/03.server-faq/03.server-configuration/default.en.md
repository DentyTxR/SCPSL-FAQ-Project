---
title: 'Server Configuration'
metadata:
    'og:url': 'https://scpsl-faq.com/en/server-faq/server-configuration'
    'og:type': website
    'og:title': 'Server Configuration | SCP:SL FAQ'
    'og:author': 'SCP: Secret Laboratory Unofficial FAQ'
    'twitter:card': summary_large_image
    'twitter:title': 'Server Configuration | SCP:SL FAQ'
    'article:author': 'SCP: Secret Laboratory Unofficial FAQ'
    'og:image': 'https://scpsl-faq.com/user/themes/quarklight/images/favicon.png'
    description: 'Unofficial SCP:SL FAQ'
    'og:site_name': scpsl-faq.com
    theme-color: '#3BB9FF'
---

# **Server FAQ | Configuration <i class="fas fa-wrench"></i>**


### **1. 914 Options**
<kbd>DroppedAndPlayerTeleport</kbd>, <kbd>Inventory</kbd>, <kbd>DroppedAndInventory</kbd>, <kbd>Held</kbd>, <kbd>DroppedAndHeld</kbd>, <kbd>Dropped</kbd>

All options that include a players inventory also teleport.


### **2. What are tickets in RA?**
That is the amount of chaos and mtf that can spawn for that round if tickets reach 0 that team can no longer spawn for that round.


### **3. How do I config the server?**

#### Windows 10

1. Open the Run prompt by clicking <kbd> <i class="fab fa-windows"></i> + R</kbd>
2. Type <kbd>%appdata%</kbd> in the Run prompt then press OK
3. That will open File Explorer and you should be inside of <kbd>C:\Users\[User]\AppData\Roaming</kbd>
4. Now you need to find the SCP Secret Laboratory folder, Inside it will have another folder called Config, Open that up and go to the folder called 7777 (Or whatever the port of your server is)
5. Inside the port folder will have all the configs, Make sure to not edit the templates, Just make new files called <kbd>config_gameplay.txt</kbd> & <kbd>config_remoteadmin.txt</kbd> then copy the stuff inside the template files and copy them over to their non-template file.

#### Linux


1. Go to <kbd>.config</kbd> folder inside the user that you installed the SCP:SL server on
2. Now you need to go to the SCP Secret Laboratory folder, Inside it will have another folder called Config, Open that up and go to the folder called 7777 (Or whatever the port of your server is)
3. Inside the port folder will have all the configs, Make sure to not edit the templates, Just make new files called <kbd>config_gameplay.txt</kbd> & <kbd>config_remoteadmin.txt</kbd> then copy the stuff inside the template files and copy them over to their non-template file.

***

### **Gameplay Config**

Latest Update - 10.03.2021

#### Server main settings
- <kbd>server_name:</kbd> The servers name, You can use [this](https://docs.unity3d.com/Manual/StyledText.html) Rich Text doc for cooler swagger stuff.
- <kbd>player_list_title:</kbd> The ingame server name on the players list. [Default: default]
- <kbd>player_list_title_rate:</kbd> [Default: default]
- <kbd>serverinfo_pastebin_id:</kbd> You're servers info works from a pastebin, You can use [this](http://digitalnativestudios.com/textmeshpro/docs/rich-text/) to make it look _fancy_.
- <kbd>server_ip:</kbd> The servers IP address. [Default: auto]
- <kbd>max_players:</kbd> Max amout of players to play on the server. [Default: 20]
- <kbd>server_tickrate:</kbd> How many times the server updates per second. [Default: 60]
- <kbd>use_reserved_slots:</kbd> If the server should use the <mark>UserIDReservedSlots.txt</mark>, this will allow the UserID's in the txt to join the server if it is full. [Default: true]
- <kbd>lobby_waiting_time:</kbd> How many seconds players will wait until a round begins. [Default: default]
- <kbd>ipv4_bind_ip:</kbd> Bind IP for IPv4. [Default: 0.0.0.0]
- <kbd>ipv6_bind_ip:</kbd> Bind IP for IPv6 [Default: <kbd>::</kbd>]
- <kbd>contact_email:</kbd> Your email address.

#### Spawn settings
- <kbd>minimum_MTF_time_to_spawn:</kbd> The minimum time (seconds) it should take for another wave of MTF to spawn when a respawn happens. [Default: 280]
- <kbd>maximum_MTF_time_to_spawn:</kbd> The maximum time (seconds) it can take from the last wave for a new one to spawn. [Default: 350]
- <kbd>maximum_MTF_respawn_amount:</kbd> The maximum amount of players that can spawn per MTF wave. [Default: 15]
- <kbd>maximum_CI_respawn_amount:</kbd> The maximum amount of players that can spawn per CI wave. [Default: 15]
- <kbd>priority_mtf_respawn:</kbd> Should MTF be a top priority for a respawn team? [Default: true]
- <kbd>use_crypto_rng:</kbd> Enables better randomness for generation by using cryptograhic random number generator (RNG). [Default: false]
! This will use more CPU to generate numbers, Default it is set to false.
- <kbd>team_respawn_queue:</kbd> Pattern in which the classes spawn at round start.
! 40143140314414041340 (Designed for 20 players)
- 0 = SCP
- 1 = MTF (Guard)
- 2 = Chaos
- 3 = Scientist
- 4 = Class-D
- 5 = Spectator
- 6 = Tutorial
- <kbd>smart_class_picker:</kbd> Should the Smart Class Picker be enabled? [Default: true]

## Player Info Range
- <kdb>player_info_range:</kdb> This controls the default range that the player information text appears on clients. [Default: 10]


#### Respawn ticket system settings
Enables the respawn tickets system.
Each NTF or CI player spawned in consumes one ticket.
We recommend keeping this on for game balance!
Warning: Even if you disable the system, the tickets ratio for MTF/CI will still determine their spawn chance. 
- <kbd>respawn_tickets_enable:</kbd> Should the respawn ticket system be enabled? [Default: true]

##### Ticket counts (initial)
The ratio of MTF-to-CI tickets directly determines which team has a higher chance of spawning.	
The initial settings (24:14) give around 36.8% chance for the CI to spawn instead of the MTF.	
The CI spawn chance can be calculated by this formula: <var>CI_TICKETS / (MTF_TICKETS + CI_TICKETS) * 100%</var>
- <kbd>respawn_tickets_mtf_initial_count:</kbd> [Default: 24]
- <kbd>respawn_tickets_ci_initial_count:</kbd> [Default: 14]

##### Ticket counts (events)
- <kbd>respawn_tickets_mtf_classd_cuffed_escape_count:</kbd> How many tickets should be given to MTF when a classd (cuffed) escapes. [Default: 1]
- <kbd>respawn_tickets_mtf_scientist_escape_count:</kbd> How many tickets should be given to MTF when a scientist escapes.[Default: 1]
- <kbd>respawn_tickets_mtf_scp_hurt_escape_count:</kbd> How many tickets should be given to MTF. [Default: 1]
- <kbd>respawn_tickets_ci_classd_escape_count:</kbd> How many tickets should be given to CI when a classd escapes. [Default: 1]
- <kbd>respawn_tickets_ci_scientist_cuffed_escape_count:</kbd> How many tickets should be given to CI when a scientist (cuffed) escapes. [Default: 2]
- <kbd>respawn_tickets_ci_scientist_died_count:</kbd> How many tickets should be given to CI when a scientist is killed. [Default: 1]
- <kbd>respawn_tickets_ci_scp_item_count:</kbd> [Default: 2]

Ticket misc settings

- <kbd>respawn_tickets_mtf_scp_hurt_interval:</kbd> The percentage of health an SCP must lose to trigger the 'scp_hurt' tickets. [Default: 0.25]

#### Stamina system settings

- <kbd>stamina_balance_use:</kbd> The percentage of stamina used per second while sprinting, 0.05 = 5%, 0.33 = 33%, etc. [Default: 0.05]

! NOTE: Stamina is currently only utilized on humans. 0 to disable, but this *will* cause weirdness with status effects and other mechanics, so we recommend keeping it on!

- <kbd>stamina_balance_immunity:</kbd> The time (in seconds) that newly-spawned players can sprint without consuming stamina. Used to reduce visual artifacts. [Default: 3]
- <kbd>stamina_balance_regen_cd:</kbd> The seconds that must pass before stamina starts regenerating after the player stops sprinting. [Default: 1]
- <kbd>stamina_balance_regen_speed:</kbd> How fast the stamina regenerates. [Default: 1]
- <kbd>stamina_balance_walk_speed:</kbd> Multiplier for human walk speed, Default speed before multiplier is 4.5 m/s. [Default: 1.2]
- <kbd>stamina_balance_sprint_speed:</kbd> Multiplier for human sprint speed, Default speed before multiplier is 7 m/s. [Default: 1.05]

#### Random-stuff settings

! <mark>-1</mark> = random.
- <kbd>server_forced_class:</kbd> Forced class on round start. [Default: -1]
- <kbd>map_seed:</kbd> Force single map seed for all rounds. [Default: -1]


#### Misc gameplay settings
- <kbd>auto_warhead_start:</kbd> Auto nuke in seconds.
- <kbd>auto_warhead_start_lock:</kbd> If the warhead lever should be locked so players cannot stop autonuke. [true/false]
- <kbd>intercom_cooldown:</kbd> Cooldown between intercom uses in seconds [Default: 120]
- <kbd>intercom_max_speech_time:</kbd> Maximum speech time on intercom in seconds [Default: 20]
- <kbd>auto_round_restart_time:</kbd> After how many rounds should the server automatically restart? [Default: 10]
- <kbd>friendly_fire:</kbd> Should Friendly Fire be enabled? [Default: false] 
- <kbd>friendly_fire_multiplier: 0.1-2</kbd> How big is friendly fire damage multiplier? [Default: 1]
- <kbd>warhead_tminus_start_duration:</kbd> How long does it take to detonate the Warhead in seconds? [Default: 90]
- <kbd>human_grenade_multiplier:</kbd> How much damage from the grenade is dealt to human classes? [Default: 0.7]
- <kbd>scp_grenade_multiplier:</kbd> How much damage from the grenade is dealt to SCP? [Default: 1]
- <kbd>lock_gates_on_countdown:</kbd> Should gates be locked (non-closable) while there's a Warhead countdown? [Default: true]
- <kbd>isolate_zones_on_countdown:</kbd> Should gates get closed while there's a Warhead countdown? [Default: false]
- <kbd>open_doors_on_countdown:</kbd> Should all inside-facility doors get opened when there's a Warhead countdown? Gates are overriden by parameter above [Default: true]
- <kbd>keep_items_after_escaping:</kbd> Should players keep their items after respawning as an addition to current loadout? [Default: true]
- <kbd>allow_playing_as_tutorial:</kbd> Should Tutorial be available using forceclass? [Default: true]
- <kbd>disable_decontamination:</kbd> Should decontamination get disabled? [Default: false]
- <kbd>096_destroy_locked_doors:</kbd> Give 096 access to destroy locked doors? [Default: true] 
- <kbd>no_holidays:</kbd> Should holiday specials be disabled? (Halloween, Christmas etc.) [Default: false]
- <kbd>allow_disarmed_interaction:</kbd> Should disarmed players be able to interact with doors? [Default: false]
- <kbd>914_mode:</kbd> Take a look at the top of the page for all available modes [Default: default]
- <kbd>sinkhole_slow_amount:</kbd> By how much units should 106 Sinkhole slow players down? [Default: 30]
- <kbd>sinkhole_spawn_chance:</kbd> What is the chance of sinkhole spawn in percent? [Default: 0]
- <kbd>disconnect_drop:</kbd> Should disconnected players automatically drop their items? [Default: true]
- <kbd>ragdoll_cleanup_time:</kbd>Time in seconds till ragdolls are removed. Set below 1 to disable. [Default: 0]
- <kbd>end_round_on_one_player:</kbd> Should round end when there's only one player on the server? [Default: false]
- <kbd>ci_on_start_percent:</kbd> Chance for CI to spawn at the beginning of a round. [Default: 10]
- <kbd>afk_time:</kbd> How many seconds someone is AFK sitting in their spawn location before they are kicked when a round started. Set to 0 to disable. [Default: 90]
- <kbd>constantly_check_afk:</kbd> Should the AFK system constantly check if someone is AFK during a round? [Default: false]

#### Pocket Dimension Settings

- <kbd>pd_exit_count:</kbd> How many valid exits appear in Pocket Dimension? [Default: 2]


#### Disarmer settings
- <kbd>mtf_can_cuff_researchers:</kbd> Can MTF cuff Researchers? [Default: true]
- <kbd>ci_can_cuff_class_d:</kbd> Can CI cuff Class D? [Default: true]
- <kbd>cuffed_escapee_change_team:</kbd> Should cuffed Class D that escapes become MTF? [Default: true]

#### Spawn Protect settings
- <kbd>spawn_protect_disable:</kbd> If spawn protection should be disabled. [Default: true]
- <kbd>spawn_protect_time:</kbd> How long spawn protection should last. [Default: 30]
- <kbd>spawn_protect_team:</kbd> [Default: [1, 2]]

!!! Team ID's
!!!
!!! * 0 = SCP
!!! * 1 = MTF
!!! * 2 = CHI (Chaos Insurgency)
!!! * 3 = RSC (Research)
!!! * 4 = CDP (Class-D Personnel)
!!! * 5 = RIP (Spectator)
!!! * 6 = TUT
- <kbd>spawn_protect_allow_dmg:</kbd> If players that are in spawn protection should be allowed todo damages. [Default: true]

#### Auto Event Broadcast settings
- <kbd>auto_warhead_broadcast_enabled:</kbd> Should a broadcast be sent when the auto warhead is engaged? [Default: false]
- <kbd>auto_warhead_broadcast_message:</kbd> [Default: "The Alpha Warhead is being detonated"]
- <kbd>auto_warhead_broadcast_time:</kbd> [Default: 10]
- <kbd>auto_warhead_detonate_broadcast:</kbd> [Default: "The Alpha Warhead has been detonated now"]
- <kbd>auto_warhead_detonate_broadcast_time:</kbd> [Default: 10]
- <kbd>auto_decon_broadcast_enabled:</kbd> Should a broadcast be sent when LCZ is decontaminated? [Default: false]
- <kbd>auto_decon_broadcast_message:</kbd> [Default: "Light Containment Zone is now decontaminated"]
- <kbd>auto_decon_broadcast_time:</kbd> [Default: 10]


#### Grenades chaining options
-1 to unlimited, 0 to disable chain reaction

- <kbd>grenade_chain_limit:</kbd> Maximum amount of grenades that can be activated by a single grenade [Default: 10]
- <kbd>grenade_chain_length_limit:</kbd> Maximum length of grenades chain [Default: 4]


#### Security & Anticheat (default settings are good enough in most cases)
Please type <mark>!private</mark> in your server console, if your server is verified, but you want to keep it hidden from the list. Type <mark>!public</mark> to make it public again.

- <kbd>online_mode:</kbd> [Default: true]
- <kbd>ip_banning:</kbd> [Default: true]
- <kbd>enable_whitelist:</kbd> [Default: false]
- <kbd>forward_ports:</kbd> [Default: true]
- <kbd>enable_query:</kbd> [Default: false]
- <kbd>query_port_shift:</kbd> [Default: 0]
- <kbd>query_use_IPv6:</kbd> [Default: true]
- <kbd>administrator_query_password:</kbd> [Default: none]
- <kbd>connections_delay_time:</kbd> [Default: 5]
- <kbd>enable_sync_command_binding:</kbd> [Default: false]
- <kbd>ratelimit_kick:</kbd> [Default: true]
- <kbd>same_account_joining:</kbd> [Default: false]
- <kbd>anticheat_console_output:</kbd> [Default: false]
- <kbd>enable_fast_round_restart:</kbd> [Default: true]
- <kbd>fast_round_restart_delay:</kbd> [Default: 3.2]

Enables challenge during preauthentication
- <kbd>preauth_challenge</kbd> [Default true]

Reply - prevents from flooding server with preauth requests from spoofed IP addresses
MD5 or SHA1 - prevents from flooding with preauth requests from legitimate IP addresses as well. Requires additional time to join the server.
- <kbd>preauth_challenge_mode:</kbd> [Default: reply]
- <kbd>preauth_challenge_base_length:</kbd> [Default: 10]
- <kbd>preauth_challenge_time_window:</kbd> [Default: 12]
- <kbd>preauth_challenge_clean_period:</kbd> [Default: 4]

Only for MD5 and SHA1 challenges (higher value = longer time required to join the server)
- <kbd>preauth_challenge_secret_length:</kbd> [Default 2]

This enforces the player to be using same IP address to connect to the game and authenticate.
Enabling this blocks proxies. Not enforced if player joined from IPv4 and authenticated from IPv6 or viceversa.
Situations with combinating IPv4 and IPv6 addresses are being checked on central servers after authentication (only for servers on public list).
- <kbd>enforce_same_ip:</kbd> [Default true]
- <kbd>no_enforcement_for_local_ip_addresses:</kbd> [Default true]

This enforces that the IP address used to connect to the game and authenticate must be assigned to the same Internet Service Provider (ISP).
Works only on servers on the public list. This is less restrictive that "enforce_same_ip" and blocks most of the proxies.
- <kbd>enforce_same_asn:</kbd>  [Default true]

Connections ratelimiting
Ratelimit time windows define how often user with the same IP/UserID can initialize new connection (once per X seconds).
- <kbd>enable_ip_ratelimit:</kbd> [Default true]
- <kbd>enable_userid_ratelimit:</kbd> [Default true]
- <kbd>ip_ratelimit_window:</kbd> [Default 3]
- <kbd>userid_ratelimit_window:</kbd> [Default 5]

!! Please refrain from changing any of these settings without enough knowledge.

#### Item limits
Ammo settings in this config are sorted as [X, Y, Z]
- X = 5.56mm (E-11-SR)
- Y = 7.62mm (Logicer, MP7)
- Z = 9mm (P90, COM-15)

##### Default ammo that each class gets on respawn
- <kbd>class_d_personnel_defaultammo:</kbd> Default: [0, 0, 0]
- <kbd>nine_tailed_fox_scientist_defaultammo:</kbd> Default: [120, 20, 20]
- <kbd>scientist_defaultammo:</kbd> Default: [0, 0, 0]
- <kbd>chaos_insurgency_defaultammo:</kbd> Default: [0, 100, 0]
- <kbd>nine_tailed_fox_lieutenant_defaultammo:</kbd> Default: [80, 0, 50]
- <kbd>nine_tailed_fox_commander_defaultammo:</kbd> Default: [120, 0, 100]
- <kbd>nine_tailed_fox_cadet_defaultammo:</kbd> Default: [40, 0, 100]
- <kbd>tutorial_defaultammo:</kbd> Default: [0, 0, 0]
- <kbd>facility_guard_defaultammo:</kbd> Default: [0, 35, 0]

##### Ammo limits, values from 0 to 65.5k, where 0 = unlimited.
- <kbd>class_d_personnel_ammolimit:</kbd> Default: [80, 70, 50]
- <kbd>nine_tailed_fox_scientist_ammolimit:</kbd> Default: [160, 100, 200]
- <kbd>scientist_ammolimit:</kbd> Default: [80, 70, 50]
- <kbd>chaos_insurgency_ammolimit:</kbd> Default: [80, 200, 100]
- <kbd>nine_tailed_fox_lieutenant_ammolimit:</kbd> [160, 100, 200]
- <kbd>nine_tailed_fox_commander_ammolimit:</kbd> [160, 100, 200]
- <kbd>nine_tailed_fox_cadet_ammolimit:</kbd> Default: [160, 100, 200]
- <kbd>tutorial_ammolimit:</kbd> Default: [160, 100, 200]
- <kbd>facility_guard_ammolimit:</kbd> Default: [160, 100, 200]

##### Item limits - values range from 0 to 8.
Values of 0 are NOT unlimited and will prevent item pickups of that type entirely!
The inventory can hold a max of 8 items,
so a limit of 8 is effectively unlimited.

- <kbd>itemlimit_keycard:</kbd> [Default: 3]
- <kbd>itemlimit_medical_item:</kbd> [Default: 3]
- <kbd>itemlimit_weapon:</kbd> [Default: 2]
- <kbd>itemlimit_grenade:</kbd> [Default: 3]
- <kbd>itemlimit_scp_item:</kbd> [Default: 3]


#### Friendly Fire Detector


!!! **How do I disable FF Detector?** [<u>Check the Server FAQ</u>!](/server-faq/faq)
!!!<br>If Friendly Fire is disabled, there is no need to disable the Detector too.
!!!
!!! Action is performed if someone either kills enough teammates OR deals enough damage to teammates.
!!! <br>Detectors priority: 
!!! <br>`Respawn (kill) -> Window (kill) -> Life (kill) -> Round (kill) -> Respawn (damage) -> Window (damage) -> Life (damage) -> Round (damage)`
!!! <br> Set kills or damage to 0 to disable that threshold.
!!!
!!! Actions:
!!! * kill
!!! * kick
!!! * ban
!!! * noop (no operation - do nothing, eg. to enable logging)
!!!
!!! Damage dealt AFTER round end is ignored.

- <kbd>ff_detector_global_broadcast_seconds:</kbd> For how long should the message be displayed on the Broadcast? [Default: 5]
- <kbd>ff_detector_global_adminchat_seconds:</kbd> For how long should the message be displayed on Admin Chat? [Default: 6]
- [Default: 6, Min: 4, Max: 25] 
- <kbd>ff_detector_classD_can_damage_classD:</kbd> If enabled Class D personnel can damage or kill other Class D personnel without being punished for it [Default: false]
- <kbd>ff_detector_webhook_url:</kbd> If set to "none" then the webhook for cheaters reporting will be used	[Default: none]

##### Per round
- <kbd>ff_detector_round_enabled:</kbd> Decides if Per Round FF detector should be enabled. [Default: true]
- <kbd>ff_detector_round_kills:</kbd> How much kills per round player has to make to trigger the detector. [Default: 6]
- <kbd>ff_detector_round_damage:</kbd> How much damage per round player has to deal to trigger the detector. [Default: 500]
- <kbd>ff_detector_round_action:</kbd> Action made after triggering the detector [Default: ban]
- <kbd>ff_detector_round_ban_time:</kbd> For how long should the player be banned. Used only if the action is set to ban 
- [Default: 24h,  Formats: s, m, h, d, M (months), y]
- <kbd>ff_detector_round_bankick_reason:</kbd> Message displayed to player after getting kicked/banned
- <kbd>ff_detector_round_kill_reason:</kbd> Message displayed to player after being killed for teamkilling
- <kbd>ff_detector_round_adminchat_enable:</kbd> Should admin chat messages be sent [Default: false]
- <kbd>ff_detector_round_adminchat_message:</kbd> Message sent to admin chat [Note: %nick - Player nickname]
- <kbd>ff_detector_round_broadcast_enable:</kbd> Should broadcast messages be sent [Default: true]
- <kbd>ff_detector_round_broadcast_message:</kbd> Broadcast message sent to players [Note: %nick - Player nickname]
- <kbd>ff_detector_round_webhook_report:</kbd> Should messages be sent using Discord Webhook? [Default: true]

##### Per life - Resets on respawn
- <kbd>ff_detector_life_enabled:</kbd> Decides if Per Life FF detector should be enabled. [Default: true]
- <kbd>ff_detector_life_kills:</kbd> How much kills per life player has to make to trigger the detector [Default: 4]
- <kbd>ff_detector_life_damage:</kbd> How much damage per life player has to deal to trigger the detector [Default: 300]
- <kbd>ff_detector_life_action:</kbd> Action made after triggering the detector [Default: ban]
- <kbd>ff_detector_life_ban_time:</kbd> For how long should the player be banned. Used only if the action is set to ban 
- [Default: 24h,  Formats: s, m, h, d, M (months), y]
- <kbd>ff_detector_life_bankick_reason:</kbd> Message displayed to player after getting kicked/banned
- <kbd>ff_detector_life_kill_reason:</kbd> Message displayed to player after being killed for teamkilling
- <kbd>ff_detector_life_adminchat_enable:</kbd> Should admin chat messages be sent [Default: false]
- <kbd>ff_detector_life_adminchat_message:</kbd> Message sent to admin chat [Note: %nick - Player nickname]
- <kbd>ff_detector_life_broadcast_enable:</kbd> Should broadcast messages be sent [Default: true]
- <kbd>ff_detector_life_broadcast_message:</kbd> Broadcast message sent to players [Note: %nick - Player nickname]
- <kbd>ff_detector_life_webhook_report:</kbd> Should messages be sent using Discord Webhook? [Default: true]

##### In a specified time window
- <kbd>ff_detector_window_enabled:</kbd> Decides if specified time window FF detector should be enabled. [Default: true]
- <kbd>ff_detector_window_seconds:</kbd> For how long is the window active [Default: 180]
- <kbd>ff_detector_window_kills:</kbd> How much kills in specified time window player has to make to trigger the detector [Default: 3]
- <kbd>ff_detector_window_damage:</kbd> How much damage per life player has to deal to trigger the detector [Default: 250]
- <kbd>ff_detector_window_action:</kbd> Action made after triggering the detector [Default: ban]
- <kbd>ff_detector_window_ban_time:</kbd> For how long should the player be banned. Used only if the action is set to ban 
- [Default: 16h,  Formats: s, m, h, d, M (months), y]
- <kbd>ff_detector_window_bankick_reason:</kbd> Message displayed to player after getting kicked/banned
- <kbd>ff_detector_window_kill_reason:</kbd> Message displayed to player after being killed for teamkilling
- <kbd>ff_detector_window_adminchat_enable:</kbd> Should admin chat messages be sent [Default: false]
- <kbd>ff_detector_window_adminchat_message:</kbd> Message sent to admin chat [Note: %nick - Player nickname]
- <kbd>ff_detector_window_broadcast_enable:</kbd> Should broadcast messages be sent [Default: true]
- <kbd>ff_detector_window_broadcast_message:</kbd> Broadcast message sent to players [Note: %nick - Player nickname]
- <kbd>ff_detector_window_webhook_report:</kbd> Should messages be sent using Discord Webhook? [Default: true]

##### In a specified time window AFTER RESPAWN
- <kbd>ff_detector_spawn_enabled:</kbd> Decides if specified time window after respawn FF detector should be enabled. [Default: true]
- <kbd>ff_detector_spawn_window_seconds:</kbd> For how long is the window active [Default: 120]
- <kbd>ff_detector_spawn_kills:</kbd> How much kills in specified time window player has to make to trigger the detector [Default: 2]
- <kbd>ff_detector_spawn_damage:</kbd> How much damage per life player has to deal to trigger the detector [Default: 180]
- <kbd>ff_detector_spawn_action:</kbd> Action made after triggering the detector [Default: ban]
- <kbd>ff_detector_spawn_ban_time:</kbd> For how long should the player be banned. Used only if the action is set to ban 
- [Default: 48h,  Formats: s, m, h, d, M (months), y]
- <kbd>ff_detector_spawn_bankick_reason:</kbd> Message displayed to player after getting kicked/banned
- <kbd>ff_detector_spawn_kill_reason:</kbd> Message displayed to player after being killed for teamkilling
- <kbd>ff_detector_spawn_adminchat_enable:</kbd> Should admin chat messages be sent [Default: false]
- <kbd>ff_detector_spawn_adminchat_message:</kbd> Message sent to admin chat [Note: %nick - Player nickname]
- <kbd>ff_detector_spawn_broadcast_enable:</kbd> Should broadcast messages be sent [Default: true]
- <kbd>ff_detector_spawn_broadcast_message:</kbd> Broadcast message sent to players [Note: %nick - Player nickname]
- <kbd>ff_detector_spawn_webhook_report:</kbd> Should messages be sent using Discord Webhook? [Default: true]


#### Custom Whitelist

Enable this ONLY if you use plugin or modification that provides custom whitelist.
This is only to mark the server on the public list as using a whitelist.
More information can be found in Verified Server Rules. If your server is not on the public list - ignore this.

- <kbd>custom_whitelist:</kbd> [Default: false]

Enable this ONLY if you use plugin or modification that restricts access to the server (other than whitelist, eg. password).
This is only to mark the server on the public list as using access restriction.
More information can be found in Verified Server Rules. If your server is not on the public list - ignore this.

- <kbd>server_access_restriction:</kbd> [Default: false]


#### Port Queue
**For nondedicated servers only**

> <code>port_queue:
> <br>- 7777
> <br>- 7778
> <br>- 7779
> <br>- 7780
> <br>- 7781
> <br>- 7782
> <br>- 7783
> <br>- 7784</code>


#### Enabling this will automatically ban IP of players on the server that receives a Global Ban by a Global Moderator. (Defaults to false)

- <kbd>gban_ban_ip:</kbd> [Default: default (true)]

- <kbd>ban_nickname_maxlength:</kbd> [Default: default]
- <kbd>ban_nickname_trimunicode:</kbd> [Default: default]

#### Nickname filtering, using regex
- <kbd>nickname_filter:</kbd> [Default: default]
- <kbd>nickname_filter_replacement:</kbd> [Default: default]


#### Administrative actions broadcast options

- <kbd>broadcast_kicks:</kbd> Should kick messages get announced to all players? [Default: false]
- <kbd>broadcast_kick_text:</kbd> Text of a kick message [Note: %nick% for player nickname]
- <kbd>broadcast_kick_duration:</kbd> How long is kick message visible in seconds? [Default: 5] 
- <kbd>broadcast_bans:</kbd> Should ban messages get announced to all players? [Default: true]
- <kbd>broadcast_ban_text:</kbd> Text of a ban message [Note: %nick% for player nickname]
- <kbd>broadcast_ban_duration:</kbd> How long is kick message visible in seconds? [Default: 5]

#### Server idle mode

- <kbd>idle_mode_enabled:</kbd> Is Idle mode enabled? [Default: true]
- <kbd>idle_mode_time:</kbd> How long should server be awake before going idle? [Default: 5000]
- <kbd>idle_mode_preauth_time:</kbd> [Default: 30000]
- <kbd>idle_mode_tickrate:</kbd> [Default: 1]

#### Player report

- <kbd>report_send_using_discord_webhook:</kbd> Should the report system be enabled? [Default: false]
- <kbd>report_discord_webhook_url:</kbd> Webhook URL to send the reports [Default: PleaseSetWebhookUrlHere]
- <kbd>report_username:</kbd> What should be the name of webhook? [Default: Cheater Report]
- <kbd>report_avatar_url:</kbd> [Default: default]
- <kbd>report_color:</kbd> Color of the report in decimal [Default: 14423100]
- <kbd>report_server_name:</kbd> Server name in the report [Default: My SCP:SL Server]
- <kbd>report_header:</kbd> Header of the report [Default: Player Report]
- <kbd>report_content:</kbd> Content of the report [Default: Player has just been reported.]

#### Restart options
##### Requires LocalAdmin or a fully compatible tool.

- <kbd>restart_after_rounds:</kbd> You can set autorestart of the server after a specified amount of rounds (0 - disabled). [Default: 0]
- <kbd>full_restart_rejoin_time</kbd> Amount of time after client should rejoin after a full server restart, Adjust depending on your server restart time. [Default: 25]


#### Geoblocking
If your server is on the public list, please refer to Verified Server Rules for more details.
<br>Modes: <kbd>none</kbd>, <kbd>whitelist</kbd>, <kbd>blacklist</kbd>

- <kbd>geoblocking_mode:</kbd> Which mode should geoblocking use? [Default: none]
- <kbd>geoblocking_ignore_whitelisted:</kbd> If enabled, players on the whitelist are able to ignore geoblocking. [Default: true]

Use ISO country codes, eg. PL, US, DE
> <code>geoblocking_whitelist:
> <br> - AA
> <br> - AB
> <br> - AC</code>

> <code>geoblocking_blacklist:
> <br> - AA
> <br> - AB
> <br> - AC</code>

***

### **Remote Admin Config**

#### Game Staff Access

- <kbd>enable_staff_access:</kbd> Should Secret Lab development staff be able to use the Remote Admin? [Default: true]
- <kbd>enable_manager_access:</kbd> Should Secret Lab CEO and managers be able to use Remote Admin? (We do not abuse our powers) [Default: true]
- <kbd>enable_banteam_access:</kbd> Allow remote admin access for the banning team, to allow them searching and fighting cheaters globally [Default: true]
- <kbd>enable_banteam_reserved_slots:</kbd> Enable reserved slots for the banning team (they are restricted by reserved slots limit set in the gameplay config) [Default: true]
- <kbd>enable_banteam_bypass_geoblocking:</kbd> Allow the banning team to bypass georestrictions on the server [Default: true]

#### Assigning Roles to Players

UserID format is `SteamId64Here@steam` or `DiscordUserIDHere@discord`.
You can get SteamID64 [here](https://steamid.io) and DiscordUserID [here](https://support.discord.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-).

> <code>Members:</code>
>  <br><code> - #################@steam: owner</code>
>  <br><code> - #################@steam: admin</code>
>  <br><code> - #################@discord: moderator</code>

**Remember to remove #################@ and other placeholders that are not used! You will encounter errors**

#### Creating Roles

- <kbd>badge</kbd> - Displayed name of the role
- <kbd>color</kbd> - Color of the Badge. Use <code>none</code> to disable badge. (List of Colors below)
- <kbd>cover</kbd> - This local badge is more important than a global badge and will cover it
- <kbd>hidden</kbd> - This local badge is hidden by default (Still can use "hidetag" and "showtag" commands in-game)
- <kbd>kick_power</kbd> - Power for kicking and banning that the member of this group has (0 to 255) 
- <kbd>required_kick_power</kbd> - Required kick power to kick or ban a member of this group (0 to 255)


Default Roles:
> <code>owner_badge: Owner
> <br>owner_color: red
> <br>owner_cover: true
> <br>owner_hidden: false
> <br>owner_kick_power: 255
> <br>owner_required_kick_power: 255</code>
>
> <code>admin_badge: Admin
> <br>admin_color: red
> <br>admin_cover: true
> <br>admin_hidden: false
> <br>admin_kick_power: 1
> <br>admin_required_kick_power: 2</code>
>
> <code>moderator_badge: Moderator
> <br>moderator_color: silver
> <br>moderator_cover: true
> <br>moderator_hidden: false
> <br>moderator_kick_power: 0
> <br>moderator_required_kick_power: 1</code>

##### Roles List
> <code>Roles:</code>
>  <br><code>- owner</code>
>  <br><code>- admin</code>
>  <br><code>- moderator</code>
  
##### List of Colors

| Color                        | Sample                        | Restricted 
| :-------------------------- | :---------------------------: | -------------------: |
| gold                          | <span style="color:#EFC01A">█████</span> | Yes
| teal                           | <span style="color:#008080">█████</span> | Yes
| blue                          | <span style="color:#005EBC">█████</span> | Yes
| purple                       | <span style="color:#8137CE">█████</span> | Yes
| light_red                   | <span style="color:#FD8272">█████</span> | Yes
| silver_blue              | <span style="color:#666699">█████</span> | Yes
| police_blue             | <span style="color:#002DB3">█████</span> | Yes
| pink                          | <span style="color:#FF96DE">█████</span> | 
| red                           | <span style="color:#C50000">█████</span> | 
| brown                      | <span style="color:#944710">█████</span> | 
| silver                       | <span style="color:#A0A0A0">█████</span> | 
| light_green              | <span style="color:#32CD32">█████</span> | 
| crimson                   | <span style="color:#DC143C">█████</span> | 
| cyan                        | <span style="color:#00B7EB">█████</span> | 
| aqua                       | <span style="color:#00FFFF">█████</span> | 
| deep_pink              | <span style="color:#FF1493">█████</span> | 
| tomato                    | <span style="color:#FF6448">█████</span> | 
| yellow                     | <span style="color:#FAFF86">█████</span> | 
| magenta                 | <span style="color:#FF0090">█████</span> | 
| blue_green             | <span style="color:#4DFFB8">█████</span> | 
| orange                    | <span style="color:#FF9966">█████</span> | 
| lime                        | <span style="color:#BFFF00">█████</span> | 
| green                      | <span style="color:#228B22">█████</span> | 
| emerald                  | <span style="color:#50C878">█████</span> | 
| carmine                  | <span style="color:#960018">█████</span> | 
| nickel                      | <span style="color:#727472">█████</span> | 
| mint                        | <span style="color:#98FB98">█████</span> | 
| army_green            | <span style="color:#4B5320">█████</span> | 
| pumpkin                 | <span style="color:#EE7600">█████</span> | 

**What are restricted colors?** _They are used in Game Staff badges, if you try to use them on your own server - they will not be visible._

##### Permissions

Default Permissions as on 10/14/2021.
> <code>Permissions:
> <br>- KickingAndShortTermBanning: [owner, admin, moderator]
> <br>- BanningUpToDay: [owner, admin, moderator]
> <br>- LongTermBanning: [owner, admin]
> <br>- ForceclassSelf: [owner, admin, moderator]
> <br>- ForceclassToSpectator: [owner, admin, moderator]
> <br>- ForceclassWithoutRestrictions: [owner, admin]
> <br>- GivingItems: [owner, admin]
> <br>- WarheadEvents: [owner, admin, moderator]
> <br>- RespawnEvents: [owner, admin]
> <br>- RoundEvents: [owner, admin, moderator]
> <br>- SetGroup: [owner]
> <br>- GameplayData: [owner, admin]
> <br>- Overwatch: [owner, admin, moderator]
> <br>- FacilityManagement: [owner, admin, moderator]
> <br>- PlayersManagement: [owner, admin]
> <br>- PermissionsManagement: [owner]
> <br>- ServerConsoleCommands: []
> <br>- ViewHiddenBadges: [owner, admin, moderator]
> <br>- ServerConfigs: [owner]
> <br>- Broadcasting: [owner, admin, moderator]
> <br>- PlayerSensitiveDataAccess: [owner, admin, moderator]
> <br>- Noclip: [owner, admin]
> <br>- AFKImmunity: [owner, admin]
> <br>- AdminChat: [owner, admin, moderator]
> <br>- ViewHiddenGlobalBadges: [owner, admin, moderator]
> <br>- Announcer: [owner, admin]
> <br>- Effects: [owner, admin]
> <br>- FriendlyFireDetectorImmunity: [owner, admin, moderator]
> <br>- FriendlyFireDetectorTempDisable: [owner, admin]</code>

#### Allows running central server commands (they are prefixed with "!") using "sudo"/"cron" command in RA (requires ServerConsoleCommands permission).
Don't turn on unless you fully trust all people with this permission, they needs to run that commands from RA and you know what are you doing

- <kbd>allow_central_server_commands_as_ServerConsoleCommands:</kbd> [Default: false]

#### Should the GUI-Based RA use the predefined ban templates below?

- <kbd>enable_predefined_ban_templates:</kbd> [Default: true]

Here you can define ban templates for your staff members to use in-game. This can always be overridden by choosing the "Custom" ban tab

FORMAT: - [Duration in seconds, Reason]

**Note** The reason cannot contain any commas or it will break the parsing!

!!! PredefinedBanTemplates:
!!!
!!!  - [0, Consider this a warning!]
!!!  - [3600, Mic Spamming]
!!!  - [86400, Team Killing (Minor Offence)]
!!!  - [604800, Team Killing (Major Offence)]
!!!  - [1577000000, Abusing Exploits]


!> [h3] Detailed info about permission nodes (Click me)
> <code>KickingAndShortTermBanning</code>Allows staff to kick players and do short term banning.

> <code>BanningUpToDay</code> Allows staff to ban players up to a day.

> <code>LongTermBanning</code> Allows staff to ban players for any time.

> <code>ForceclassSelf</code> Allows staff to force-class themself.

> <code>ForceclassToSpectator</code> Allows staff to force-class players into spectator.

> <code>ForceclassWithoutRestrictions</code> Allows staff to force-class anyone without restrictions.

> <code>GivingItems</code> Allows staff to give items to themself/players.

> <code>WarheadEvents</code> Allows staff to active warhead events.

> <code>RespawnEvents</code> Allows staff to use respawn events for CI & MTF.

> <code>RoundEvents</code> Allows staff to use round events such as lockround, Lobbylock, etc.

> <code>SetGroup</code> Allows staff to use the setgroup command, Do **not** give this to everyone. The setgroup command can set players rank and give them staff rank.

> <code>GameplayData</code> Allows staff to see players gameplay data in the "Player spec. info" part of RA.

> <code>Overwatch</code> Allows staff to set themself to overwatch mode, Usefully for watching sus players that may be breaking the rules.

> <code>FacilityManagement</code> Allows staff to ~~break the server~~ use the Door management part of the RA panel.

> <code>PlayersManagement</code> Allows staff to use the Player mgmt part of RA panel.

> <code>PermissionsManagement</code> Type "PM" into RA console to read about it.

> <code>ServerConsoleCommands</code> Allows staff to execute commands in LocalAdmin console, Do **NOT** give this permission to everyone.

> <code>ViewHiddenBadges</code> Allows staff to see hidden badges of other players/staff, Not studio staff.

> <code>ServerConfigs</code> Allows staff to use the Server configs section of RA panel.

> <code>Broadcasting</code> Allows staff to make broadcasts.

> <code>PlayerSensitiveDataAccess</code> Allows staff to see players IP/auth's.

> <code>Noclip</code> Allows staff to give themself/players noclip, Use noclip with left alt.

> <code>AFKImmunity</code> Allows staff to be immune to auto-afk.

> <code>AdminChat</code> Allows staff to use adminchat. [Type @ in RA console or debug console.]

> <code>ViewHiddenGlobalBadges</code> Allows staff to view hidden g-badges.

> <code>Announcer</code> Allows staff to use the cassie command.

> <code>Effects</code> Allows staff to use effects.

> <code>FriendlyFireDetectorImmunity</code> Allows staff to be immune to FF detector.

> <code>FriendlyFireDetectorTempDisable</code> Allows staff to temporally disable FF detector.
!@

#### RA PASSWORD REMOVED
##### RA Password section is removed from this FAQ due to it being forcefully disabled for a good reason, You cannot enable it nor should you.

!!!! Some stuff here was pulled from the [SCP:SL Wiki](https://en.scpslgame.com/index.php?title=Docs:Server_Config), If you have any questions or concerns or find a typo you can either join our discord server [here](https://discord.gg/qZ97fZjJeq) or send a email at scpsl.faq@gmail.com
