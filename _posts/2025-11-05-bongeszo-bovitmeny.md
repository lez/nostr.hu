---
title: Aláírók
description: >-
  A privát kulcsot titokban kell tartani, erre valók az aláírók. Ezek appok, vagy böngésző bővítmények,
  melyek alá tudják írni az eseményeket, úgy hogy közben a titkos kulcsra vigyáznak, hogy ne kerülhessen más kezébe.
author: lezkoma
date: 2025-11-05 11:01:00 +0100
categories: [Tutorial]
tags: []
permalink: /alairok
icon: fas fa-pen-nib
order: 1
---

## Böngésző bővítmények

### Chrome

Ha Chrome alapú böngészőt használunk, telepítsük fel a [keys.band](https://chromewebstore.google.com/detail/keysband/jdencabhccnfhedpfoojbbdlgmecnlkm) bővítményt, majd menjünk végig a beállításokon. Ha a végére értünk, készen állunk arra, hogy belevessük magunkat a Nostr világába.

![pin it](/assets/img/keys-pin.png)
*Telepítés után pinneljük a keys.band bővítményt*

![step 1](/assets/img/keys-1.png)
*Nyissuk le a profil választó menüt*

![step 2](/assets/img/keys-2.png)
*Adjunk hozzá új profilt (Add Account)*

![step 3](/assets/img/keys-3.png)
*Generáljunk egy titkos kulcsot. Ha már korábban elmentettünk egy titkos kulcsot, másoljuk be ide.*

![step 4](/assets/img/keys-4.png)
*Írjuk be a nevet, klikkeljünk az "Add Account"-ra*

![step 5](/assets/img/keys-5.png)
*Válasszuk ki az új profilt*

Gratulálunk, kész az új profilod, amire a böngésződ emlékezni fog. Ne felejts el biztonsági mentést készíteni a titkos kulcsról.

Innentől kezdve ha be akarunk lépni Nostr-rel egy weboldalra, pl. a [Köztérre](https://kozter.nostr.hu), a következő ablakot fogja feldobni a bővítmény:

![step 6](/assets/img/keys-6.png)
*Csak okézzuk le, és élvezzük a Nostr-t*

Ha több profilt szeretnénk használni, csak ugyanezt a folyamatot kell többször végigjátszani. Később a keys.band bővítményben tudjuk kiválasztani a használni kívánt profilt.

### Firefox

Hasonló folyamatot kell végigcsinálni a [nos2x-fox](https://addons.mozilla.org/en-US/firefox/addon/nos2x-fox/) bővítménnyel.

### Safari

A [nostash](https://apps.apple.com/us/app/nostash/id6744309333) programot telepítsük, és a fentiekhez hasonló módon állítsuk be.

### Android

Androidon a titkos kulcs kezelését az Amber nevű alkalmazásra célszerű bízni. Legtöbb Androidos Nostr app tudja kezelni, így a titkos kulcsunk védve lesz, ha kliensek hibásan működnek.

### Egyéb lehetőségek

Ha IPhone-on Nostr-ezünk, vagy a fenti aláírókat valami miatt nem akarjuk vagy nem tudjuk feltelepíteni, két választásunk van:

* Használjuk a titkos kulcsot közvetlenül az alkalmazásban. Ha ezt választjuk, előbb-utóbb vagy mi, vagy az app fejlesztői elkövetnek egy hibát, és a titkos kulcs kompromittálódik, egy ismeretlen személynél köt ki. Például fáradtan véletlenül a böngésző címsorába másoljuk be az nsec1-gyel kezdődő titkos kulcsot, és az már fenn is van a Google szerverein, anélkül hogy akár entert nyomnánk.

Ilyenkor bölcs dolog lecserélni a kulcsot, és értesíteni a régi követőket, hogy mi az új publikus kulcsod.

#### Bunker login

![bunker](/assets/img/bunker.png)

Haladó felhasználók megcsinálhatják, hogy egy szerveren vagy egy mini-pc-n (Raspberry Pi-n) üzemeltetnek egy aláírószoftvert, amit bunkernek vagy nsecBunkernek neveznek. Ezt, főleg ha ez az egy dolog fut a gépen, gyakorlatilag lehetetlen feltörni, a hiba lehetősége meglehetősen alacsony. Egyelőre még technikai tudás szükséges ahhoz, hogy ilyet üzemeltessünk, de ahogy egyre népszerűbb lesz a Nostr, számíthatunk rá, hogy megjelennek a fogyasztói bunker kütyük.

<a href="https://www.flaticon.com/free-icons/bunkers" title="bunkers icons">Bunkers icons created by Sergei Kokota - Flaticon</a>
