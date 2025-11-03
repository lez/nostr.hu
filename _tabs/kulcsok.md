---
title: Kulcsok
icon: fas fa-key
order: 2
---

A szólásszabadság érdekében egyetlen dolgot kell mindenképpen megtennünk.
Ahol nem kell, ott a közösségi oldal tulajdonosa kedvére cenzúrázhatnak vagy shadow-bannolhatnak minket, kontrollálhatják hogy kihez jutnak el a posztjaink.
Vigyázni kell egy **titkos kulcsra**, nem szabad elveszíteni és nem szabad, hogy más megtudja. Sajnos ez van, ez a belépő a szuverenitáshoz.

## A titkos kulcs (nsec...)

![keys](/assets/img/keys.png){: .right }

Így néz ki: <kbd>nsec1vdfhcle6h7uup2z9g6qherdulg4ghjnuzd8pn9389vqexq56y8qqjfy3pa</kbd>

A titkos kulcsot úgy kell elképzelni, mint egy kocsikulcsot. Akinél a kulcs van, az tudja a kocsit használni. Csinálhatunk belőle másolatokat, és elrejthetjük őket, az egyiket a párna alá, a másikat a nyaralóba. Ha valaki megtalálja a kulcsot a nyaralóban, akkor azzal tudja használni az autódat, amit jobb elkerülni. Ha elveszíted az összes kulcsot, a kocsi is használhatatlanná válik.

Tehát a Nostr-en a titkos kulcs arra szolgál, hogy digitálisan aláírjunk vele posztokat és más eseményeket. A kulcs nélkül nem tudunk aláírni.

A titkos kulcs biztonságos tárolására szolgálnak a böngésző bővítmények, illetve androidon az Amber applikáció. Ezek olyan aláíró (signer) programok, amik nem adják ki a titkos kulcsot, de engedik a weboldalnak vagy alkalmazásnak, hogy aláírjanak vele posztokat, eseményeket. Így egy gonosz honlap vagy mobilalkalmazás nem tudja ellopni a titkos kulcsot.

## A publikus kulcs (npub...)

Így néz ki: <kbd>npub158nrfx7jwmfry9stu9d0ujrz6zqz9lmvad9pyrulrsvhhpm40ngst6pjyx</kbd>

A publikus kulcs, vagy "*npub* " a profil nyilvános, egyedi azonosítója. A publikus kulcsot ismerve bárki leelenőrizheti, hogy egy posztot valóban az az ember írta, akinek megvan a hozzátartozó privát kulcs.

A publikus és a titkos kulcs együtt egy kulcspárt alkot.

## Böngésző Bővítmények

Ha **Chrome** alapú böngészőt használsz, a [keys.band](https://chromewebstore.google.com/detail/keysband/jdencabhccnfhedpfoojbbdlgmecnlkm) bővítménnyel kezelheted a kulcsaidat.

**Firefox** alapú böngészőkhöz a [nos2x-fox](https://addons.mozilla.org/en-US/firefox/addon/nos2x-fox/) bővítményt javasoljuk.

**Safari** böngésző esetén a [nostash](https://apps.apple.com/us/app/nostash/id6744309333) használható.

## Mobil

**Androidon** pedig az [Amber](https://github.com/greenart7c3/Amber) a javasolt alkalmazás, mely a titkos kulcsaidat kezeli.

**Iphoneon** sajnos nincs külön aláíró alkalmazás, de a Damus nevű kliensprogrammal tudod használni a Nostr-t.
