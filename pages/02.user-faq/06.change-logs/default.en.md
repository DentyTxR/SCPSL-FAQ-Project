---
title: 'Change Logs'
published: true
metadata:
    'og:url': 'https://scpsl-faq.com/en/user-faq/Change Logs'
    'og:type': website
    'og:title': 'Change Logs | SCP:SL FAQ'
    'og:author': 'SCP: Secret Laboratory Unofficial FAQ'
    'og:image': 'https://scpsl-faq.com/user/themes/quarklight/images/favicon.png'
    'twitter:card': summary_large_image
    'twitter:title': 'Change Logs | SCP:SL FAQ'
    'article:author': 'SCP: Secret Laboratory Unofficial FAQ'
    description: 'Unofficial SCP:SL FAQ'
    'og:site_name': scpsl-faq.com
    theme-color: '#3BB9FF'
visible: false
---

# **User FAQ | Official SCP:SL Change Logs**


!> [h3] Version 11.1 | December 1st, 2021
[From Here](https://store.steampowered.com/news/app/700330/view/3102412650211108576)

## SCP-330, ”Take Only Two”
While it may not have had as many explosions as last year, 2021’s version of SCP-330 was an instant hit. Between the practical effects and the spectacular ones, the candy bowl helped define both the identity, and in-game experience of Halloween.

As promised, the object has been refined and is now a permanent addition to the game — awaiting visitors with a sweet tooth.

You can find SCP-330 in Test Chamber 01, or TC01 for short. TC01 has replaced the old SCP-012 room from SCP: Containment Breach
. SCP-330 itself is located behind an airlock, which can only be operated from a keycard-locked control room. Try not to lock yourself in... unless you have something to break the glass with, overindulging in SCP-330 might be the only way to free yourself.

The permanent version of SCP-330 is much less theatrical than that experienced in October. Each of its candies now have a much gentler effect. While they still provide a lot of helpful gameplay applications, they no longer have the round-defining abilities that they had during the Halloween event. Even so, we’re very happy with the outcome, and we hope that you enjoy it.




## SCP-2176, ”Ghostlight™”
This haunted light bulb was the second SCP object introduced in the Halloween update. It may not have been as spectacular as its sister feature, SCP-330, but still had plenty of tricks up its sleeve. Whether it was saving players from risky situations, or making those situations much worse, it bent the rules and shaped the round in unexpected ways — characteristics which we love to see in an SCP object.

As opposed to SCP-330, the Ghostlight hasn’t received many changes compared to its Halloween version. In fact, it’s mostly been buffed across the board, featuring a longer effect duration, SCP-914 interactions, and a generous helping of stability improvements.

You can find SCP-2176 in pedestals placed throughout the map, although there may be other ways to obtain it as well. Have fun, and be sure to bring your smudge sticks!

As a side note, we saw a lot of success in introducing these features as limited-time content, then taking the time to review them for permanent implementation. We’ll likely be doing this again, so make sure to keep your eyes open.

## Balance Changes
11.1 is our first real opportunity to do a balance pass on the mechanics introduced in Parabellum; as we’ve now had a chance to observe the new content, and see how it plays out within the game. With that in mind, we’ve drafted a small collection of adjustments:
SCP-173

- Blink cooldown no longer increases by 0.6s for each observer. Its cooldown is now always 3.6s.
- Blink distance decreased to 12.5m, from 15.0m. Blink distance during Breakneck Speeds remains unchanged, at 22.5m.

### Weapons

- Slightly buffed all suppressors; they now weigh less, and improve the firearm’s bullet accuracy.
- Removing the buttstock from your AK will no longer prevent aiming down the sights, however doing so is very inaccurate and does not reduce the recoil.



### Other Changes

- SCP-268 can no longer be obtained through SCP-914. (This was an accidental addition committed during testing of SCP-914’s systems)
- Dropped body armor is now less likely to block small items. Items below a certain weight will be teleported on top of the dropped armour to improve visibility.
- The shotgun can now be unloaded and dry-fired like other firearms, and its performance is no longer compromised when playing on high-latency servers.
- The damage multiplier for friendly fire is now 40% by default. Existing configs remain unchanged.
- Fast round restart is now disabled by default. Existing configs remain unchanged.
- The default team assignment queue now repeats the sequence from the beginning if the number of players at the beginning of the round exceeds the amount of entries, instead of automatically spawning all excess players as Class-D personnel. The default sequence has also been modified to compensate for this effect.
- Ragdolls may now have force applied to them depending on cause of death. Being shot in the face might cause your character to tumble backwards, while SCP-096's charge sends people flying.
- The spawntarget Remote Admin command has been replaced by the spawntoy command, which supports several new additions; including light sources and primitive objects for use with plugins.
- Added a destroytoy
- Remote Admin command for removing spawned toys.
- Doors spawned at runtime are properly added to the culling system.
- The Surface Zone now culls based on the player’s height in the game world. This fixes a bug where a player could get lost if they moved far enough away while in noclip, due to the entire zone being culled.
- The volume of SCP-173’s audio cues is now correctly tied to sound effect volume, which should prevent them from being much louder than other sounds.
- Added more invisible colliders to prevent people from jumping on some spots that are unreachable to SCPs.
- SCP-173’s Blink will no longer attempt to place them in the HCZ armory’s pit, which used to result in an instant death.
- Grenades no longer move at 500x the speed of sound when thrown in a moving elevator, or by an escaping player. This would cause the server to softlock until the physics engine caught up. (We referred to this bug as a “lore-accurate 018”.)
- Fixed a bug where the friendly-fire damage multiplier was being squared before use.
- Fixed the Logicer’s third-person model missing holes in its heat shield material.
- Fixed an exploit that allowed players to gain infinite ammo.
- Ammo boxes in the SCP-079 armoury should no longer spawn misplaced.
- Fixed camera movement animation playing when moving your mouse while picking up items.
- Fixed Micro H.I.D. sound that kept playing when a dead player gets quickly respawned.
- Fixed MTF-E11-SR often spawning misplaced in its rack.
- Fixed voice chat loudness indicators not having animated background.
- 173's sound effects now properly respect the audio settings.
- The warning about body being expired for 049's revival works again.
    
!@
