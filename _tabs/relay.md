---
title: Csomópontok
icon: fas fa-server
order: 3
---

A Nostr hálózatában a csomópontok azok a szerverek, amik a bejegyzéseket, profil adatokat, és egyéb szöveges infókat tárolják.

![nostr architektura](/assets/img/nostr.webp)

Minden felhasználó saját maga dönti el, hogy mely csomópontokra tölti fel a posztjait. A követők pedig tudják, hogy hol keressék a posztokat.

<!-- markdownlint-disable-next-line -->
>  Be kell magadnak állítanod néhány csomópontot. A cikk végén ajánlunk egy alap beállítást, amivel elindulhatsz.
{: .prompt-info }

## A csomópont az innováció

1. A csomópont működése egyszerű, néhány oldalon elfér a [leírás](https://nips.nostr.com/1), hogy mit kell egy csomópontnak tudnia. Fogadnia kell a posztokat (és egyéb eseményeket), és az olvasónak vissza kell adni azokat úgy, ahogy ő épp kíváncsi rájuk.

2. A csomópont nem tudja egymagában megakadályozni, hogy egy szerző írásai eljussanak a követőihez. Ha a szerző 5 csomópontot adott meg, ahova ő posztol, akkor az 5-ből 4-et akár le is lőhetnek, az 5. csomóponton keresztül a követők továbbra is olvashatják amire kíváncsiak. **Ez biztosítja a szólásszabadságot a Nostr-en**.

3. A csomópontnál nincs meg a felhasználók titkos kulcsa, így nem tudja meghamisítani a posztokat. A poszt hitelességét mindig az olvasó által használt kliensprogram ellenőrzi automatikusan.

## Milyen csomópontok vannak?

Az, hogy egy csomópont milyen szabályok szerint fogad el üzeneteket, függ a használat módjától (Írt / olvasott / üzenő), és attól, hogy ki és miért üzemelteti. Léteznek közösségi csomópontok, melyek egy közösség számára vannak, fizetett csomópontok, ahol ára van annak, hogy tárolják a posztjainkat, de tarthatunk csomópontot saját használatra is, ha nem szeretjük a meglepetéseket.

A rendszer életképességét és decentralizáltságát (központ nélküliség) az adja, hogy mindenki saját maga dönti el, milyen csomópontokat használ.

#### Írt és olvasott csomópontok

Az írt csomópontjaid azok a szerverek, ahova a kliensed feltölti a posztjaidat miután megírtad őket. Ez általában 2-4 csomópont praktikusan. Ha ezekből valamelyik épp nem megy a posztod megírásakor, a többi relay eltárolja és odaadja a követőidnek. Ugyanígy, ha valamelyik csomópont törli a posztodat, a többin még megvan és bárki számára elérhető.

Az olvasott csomópontok azok, ahova a válaszok érkeznek. Ha valaki megemlít téged egy bejegyzésben, az értesítést ezekre a csomópontokra fogja feltölteni, mivel tudja, hogy a te kliensed ezeket a csomópontokat olvassa. Ha reakció érkezik egy posztodra, szintén ide fogják az értesítéseket feltölteni. Itt a csomópontok szoktak némi spam-szűrést végezni.

Gyakran az írt és az olvasott csomópont ugyanaz. Ezeket a csomópontokat majdnem minden kliensben be tudod állítani, például [itt is](https://jumble.nostr.hu/settings/relays) az "írt és olvasott csomópontok"-ra klikkelve.

A `wss://relay.nostr.hu` egy olyan csomópont, ami a magyar Nostr közösségnek van fenntartva.

#### DM, vagyis üzenet csomópontok

Ezek a csomópontok azt vállalják, hogy tárolják a felhasználóknak küldött privát üzeneteket ([nip17](https://nips.nostr.com/17)).



