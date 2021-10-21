---
title: 'Tunnetut Ongelmat'
metadata:
    'og:url': 'https://scpsl-faq.com/fi/user-faq/known-issues'
    'og:type': website
    'og:title': 'Tunnetut Ongelmat | SCP:SL FAQ'
    'og:author': 'SCP: Secret Laboratory Unofficial FAQ'
    'twitter:card': summary_large_image
    'twitter:title': 'Tunnetut Ongelmat | SCP:SL FAQ'
    'article:published_time': '2020-08-06T10:27:21-04:00'
    'article:modified_time': '2020-08-06T10:27:21-04:00'
    'article:author': 'SCP: Secret Laboratory Unofficial FAQ'
    description: 'Unofficial SCP:SL FAQ'
    'og:site_name': scpsl-faq.com
---

# **Käyttäjä | Tunnetut Ongelmat**


### **1. Palvelinluettelon vastaus on vanhentunut! Aseta oikea aika ja aikavyöhyke tietokoneellesi.**

DST (Kesäaika) aiheuttaa tämän ongelman, korjaa aikavyöhyke 1llä tunnilla eteenpäin.

### **2. Minulla on -1 hp tai muita ongelmia pelatessani nondedicatedissa palvelimessa!**

Älä käytä sitä, toiminto on rikki stabiilissa ja beetaversiossa.

### **3. Jotkut asetukset eivät tallennu tai eivät toimi kunnolla.**

Se on tunnettu ongelma, siihen ei voi vaikuttaa mitenkään. Ohita ongelma, ja odota päivitys.

### **4. Olen jumissa vanhassa menuussa!**

Ratkaisu 1. Paina <kbd>Windows + R</kbd>, ja sitten kirjoita <kbd>%AppData%\SCP Secret Laboratory</kbd>, avaa <mark>Registry.txt</mark> ja vaihda <kbd>07menumode</kbd> => <kbd>1</kbd>

Ratkaisu 2. Lataa [tämän](https://cdn.discordapp.com/attachments/403321276153987072/716675004258844703/MenuReset.exe) ohjelman ja käynnistä .exen, sen pitäis automaattisesti korjata <mark>Registry.txt</mark> tiedoston.

!!! **<center>Tämän ohjelman on tehnyt Virallinen Northwood Studios Henkilöstö.</center>** <br> Jos et ole varma lataamasta sitä verkkosivustoltamme, tarkista Tech Support kanava virallisesta [<u>SCP:SL Discordista</u>](https://discord.com/invite/scpsl).

### **5. Palvelin ei käynnisty uudelleen/lataudu ja se jäi jumiin 0%ssa**

Ratkaisu 1. (Jos olet palvelin omistaja) Sinun config_gameplayin tiedoston sisällä löytyy <kbd>idle_mode_enabled</kbd>, vaihda se <mark>False</mark>ks.

Ratkaisu 2. (Jos et ole palvelin omistaja) Joko etsi toinen pelattava palvelin tai pyydä palvelimen omistajaa korjaamaan ongelman.
