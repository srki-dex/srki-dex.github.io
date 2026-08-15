---
title: "Kako funkcioniše domen i hosting? Objašnjenje za početnike"
description: "Saznajte šta su domen i hosting, kako funkcionišu zajedno i kako DNS povezuje domen sa serverom. Jednostavno objašnjenje za početnike u web dizajnu."

image: "/assets/images/domen-hosting.webp"

categories: 
  - web-dizajn
---

Kada napravimo web sajt, potrebno je da ga postavimo na internet kako bi drugi ljudi mogli da ga posete. Tu se najčešće susrećemo sa dva pojma: **domen** i **hosting**.

Ako tek ulazite u svet web dizajna, ova dva pojma mogu delovati komplikovano. Međutim, njihova uloga je prilično jednostavna.

## Šta je domen?

Domen je **adresa vašeg sajta na internetu**.

Na primer:

`srki-dex.github.io`

ili:

`example.com`

Kada korisnik ukuca domen u browser, on zapravo govori browseru koju web adresu želi da poseti.

Domen se sastoji iz nekoliko delova. Kod adrese `example.com`, `example` je naziv domena, dok je `.com` domen najvišeg nivoa, odnosno TLD.

Postoje različiti nastavci, kao što su:

`.com`
`.rs`
`.org`
`.net`

Izbor domena zavisi od projekta. Za firmu koja posluje u Srbiji, na primer, `.rs` može biti logičan izbor.

## Šta je hosting?

Hosting je mesto na serveru na kojem se nalaze fajlovi vašeg web sajta.

HTML, CSS, JavaScript, slike, fontovi i ostali potrebni fajlovi moraju biti dostupni serveru kako bi browser mogao da ih preuzme.

Možemo napraviti jednostavno poređenje:

**Domen = adresa kuće**
**Hosting = sama kuća**

Domen govori gde se sajt nalazi, dok hosting obezbeđuje prostor na kojem se sajt nalazi.

## Kako domen i hosting rade zajedno?

Kada korisnik ukuca domen u browser, događa se nekoliko stvari.

Prvo browser mora da pronađe server na kojem se nalazi sajt. Za to se koristi **DNS (Domain Name System)**.

DNS povezuje naziv domena sa IP adresom servera.

Na primer, korisnik ukuca:

`example.com`

DNS pronalazi odgovarajući server, a browser zatim šalje zahtev tom serveru.

Server pronalazi potrebne fajlove i šalje ih browseru, koji ih prikazuje kao web stranicu.

Pojednostavljeno:

**Domen → DNS → server → fajlovi sajta → browser → web stranica**

## Da li su domen i hosting ista stvar?

Ne.

Domen i hosting su dve različite usluge, iako ih mnogi hosting provajderi nude zajedno.

Možete kupiti domen kod jedne kompanije, a hosting koristiti kod druge.

Postoje i platforme koje omogućavaju hosting bez klasičnog plaćenog servera. Na primer, **GitHub Pages** može hostovati statičke sajtove direktno iz GitHub repozitorijuma.

Zbog toga je moguće imati sajt bez tradicionalnog hosting paketa, u zavisnosti od potreba projekta.

## Šta je HTTPS?

Kada posetite sajt koji počinje sa:

`https://`

komunikacija između browsera i servera je zaštićena HTTPS protokolom.

Za HTTPS se koristi SSL/TLS sertifikat. Browser tada može da prikaže ikonicu katanca pored adrese.

HTTPS je danas standard za web sajtove i važan je za bezbednost, privatnost i poverenje korisnika.

## Šta zapravo plaćamo?

Kod klasičnog web sajta najčešće plaćamo **registraciju domena** i **hosting**.

Cena zavisi od domena, provajdera, prostora, performansi, email naloga, baze podataka i drugih funkcija.

Za jednostavan statički sajt mogu biti dovoljna vrlo jednostavna ili čak besplatna hosting rešenja. Za veće aplikacije, online prodavnice ili sajtove sa bazama podataka potrebna je ozbiljnija serverska infrastruktura.

### Zaključak

Domen i hosting nisu ista stvar, ali zajedno omogućavaju da web sajt bude dostupan na internetu.

**Domen je adresa, hosting je prostor na serveru, a DNS ih povezuje.**

Kada razumete ovu osnovu, mnogo je lakše razumeti kako funkcionišu web sajtovi, serveri i internet.

Iza jednostavnog klika na link zapravo se dešava čitav niz procesa – od DNS-a i servera do HTTP/HTTPS zahteva i prikazivanja HTML-a u browseru.
