---
title: "Sitemap.xml i robots.txt – šta rade i zašto postoje?"
description: "Sitemap.xml i robots.txt su važni delovi tehničkog SEO-a. Saznajte čemu služe, kako funkcionišu i kako pomažu Google-u da pronađe i razume vaš web sajt."

image: "/assets/images/sitemap-robots.txt.webp"

categories: 
  - seo
---

Ako ste ikada radili na SEO optimizaciji web sajta, gotovo sigurno ste naišli na dva fajla: **sitemap.xml** i **robots.txt**.

Na prvi pogled deluju kao obični tekstualni fajlovi koji se nalaze u korenu sajta. Ipak, imaju veoma važnu ulogu u komunikaciji između vašeg sajta i pretraživača.

Ali šta zapravo rade?

## Šta je sitemap.xml?

**Sitemap.xml** je XML fajl koji sadrži listu URL adresa koje želimo da pretraživači pronađu i indeksiraju.

Na primer, jedan jednostavan sitemap može sadržati:

početnu stranicu

stranicu „O meni“

kontakt stranicu

blog

pojedinačne blog postove

kategorije

Možemo ga zamisliti kao **mapu sajta za pretraživače**.

Kada Google ili drugi pretraživač pronađe sitemap, lakše može da otkrije stranice koje postoje na sajtu.

Važno je napomenuti da sitemap sam po sebi **ne garantuje bolje rangiranje**. Njegova glavna svrha je da pomogne pretraživačima da otkriju i razumeju strukturu sadržaja.

Posebno može biti koristan kod većih sajtova, novih sajtova ili sajtova čije stranice nisu dobro povezane internim linkovima.

## Šta je robots.txt?

**robots.txt** je potpuno drugačiji fajl.

Dok sitemap govori pretraživačima **šta postoji na sajtu**, robots.txt daje instrukcije crawlerima **koje delove sajta mogu ili ne mogu da obilaze**.

Primer:

```text
User-agent: *
Disallow: /admin/
```

Ovo znači da se instrukcija odnosi na sve crawlers, dok se `/admin/` navodi kao deo sajta koji ne treba obilaziti.

Robots.txt se nalazi na adresi:

```text
https://vas-sajt.rs/robots.txt
```

i treba da bude dostupan direktno iz glavnog domena.

## Sitemap nije isto što i robots.txt

Ovo je jedna od najčešćih zabuna.

**Sitemap.xml = mapa stranica**

**Robots.txt = pravila za crawlers**

Mogu da rade zajedno, a često se sitemap navodi direktno u robots.txt fajlu:

```text
User-agent: *
Allow: /

Sitemap: https://vas-sajt.rs/sitemap.xml
```

Na ovaj način crawler može lako da pronađe adresu sitemap-a.

## Da li robots.txt blokira indeksiranje?

Ne baš.

Ovo je veoma važna stvar za SEO.

Robots.txt prvenstveno kontroliše **crawling**, odnosno pristup crawlera određenim URL adresama. Ne treba ga koristiti kao glavni način za uklanjanje stranice iz Google indeksa.

Ako želite da određena stranica ne bude indeksirana, u zavisnosti od situacije koriste se druge metode, kao što je `noindex` direktiva.

Zato treba biti oprezan sa pravilima u robots.txt fajlu. Jedna pogrešna `Disallow` direktiva može sprečiti crawler da dođe do važnog dela sajta.

## Da li svaki sajt mora da ima oba fajla?

Ne mora.

Mali sajt može funkcionisati i bez sitemap-a ili robots.txt fajla. Međutim, njihovo pravilno korišćenje može olakšati pretraživačima razumevanje i obilazak sajta.

Za SEO optimizovan sajt preporučljivo je imati **dobro podešen sitemap.xml i pravilno konfigurisan robots.txt**.

Posebno ako radite na većem projektu ili želite ozbiljnije da pratite indeksiranje stranica.

## A gde je tu Google Search Console?

Tu dolazimo do još jednog korisnog alata – **Google Search Console**.

U njemu možete pratiti kako Google vidi vaš sajt, koje stranice su indeksirane, da li postoje problemi i, između ostalog, poslati adresu sitemap-a.

To je odličan način da proverite da li Google zaista može da pronađe stranice koje želite da budu vidljive u pretrazi.

## Ukratko

Ako tek počinjete da se bavite SEO-om, zapamtite jednostavno pravilo:

**Sitemap govori pretraživaču gde su stranice.**

**Robots.txt govori crawleru gde sme da ide.**

Ova dva mala fajla nisu magično SEO rešenje, ali su važan deo tehničke optimizacije web sajta.

A kada ih pravilno kombinujete sa kvalitetnim sadržajem, dobrim internim linkovima i tehnički ispravnim sajtom, pretraživačima znatno olakšavate posao.

I upravo to je jedna od osnovnih ideja dobrog SEO-a – **ne pokušavati da prevarimo pretraživač, već mu pomoći da razume naš sajt.**
