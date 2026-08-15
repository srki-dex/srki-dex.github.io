---
title: "Canonical URL – šta je i kada se koristi?"
description: "Saznajte šta je canonical URL, kada se koristi, kako se postavlja i koja je razlika između canonical taga i 301 redirecta u tehničkom SEO-u."

image: "/assets/images/canonical-url.webp"

categories: 
  - seo
---

Kada isti ili veoma sličan sadržaj postoji na više različitih URL adresa, pretraživači mogu imati problem da odrede koju verziju stranice treba da prikažu u rezultatima pretrage. Tu na scenu stupa **canonical URL**.

Canonical URL predstavlja URL koji smatramo glavnom, odnosno preferiranom verzijom određene stranice. Google ga koristi kao signal za određivanje reprezentativne URL adrese među dupliranim ili veoma sličnim stranicama.

## Kako izgleda canonical tag?

Canonical se postavlja unutar `<head>` sekcije HTML dokumenta:

```html
<link rel="canonical" href="https://example.com/blog/seo/canonical-url/" />
```

Na primer, ako je ovo glavna verzija mog članka:

```text
https://srki-dex.github.io/blog/seo/canonical-url/
```

onda upravo taj URL treba navesti kao canonical.

Google preporučuje da canonical bude **apsolutni URL**, odnosno da sadrži kompletan `https://` URL. Takođe je preporučljivo da glavna stranica ima takozvani **self-referencing canonical**, odnosno canonical koji pokazuje na samu sebe.

## Kada se koristi?

Canonical je posebno koristan kada isti sadržaj može biti dostupan preko više URL-ova.

Na primer:

```text
https://example.com/proizvod
https://example.com/proizvod?ref=instagram
https://example.com/proizvod?utm_source=facebook
```

Ako sve ove adrese prikazuju isti sadržaj, možemo Google-u signalizirati da je `/proizvod` glavna verzija.

Canonical se može koristiti i kod različitih URL varijanti nastalih zbog filtera, sortiranja ili drugih parametara. Međutim, nije zamena za pravilnu strukturu sajta ili redirect.

## Canonical nije isto što i redirect

Ovo je veoma važno.

**301 redirect** korisnika automatski šalje sa stare URL adrese na novu. Canonical, sa druge strane, ostavlja stranicu dostupnom, ali pretraživaču daje signal koja verzija je preferirana.

Google navodi da su redirecti jači signal za canonicalizaciju, dok je `rel="canonical"` takođe snažan signal, a sitemap predstavlja slabiji signal.

## Da li canonical garantuje rezultat?

Ne. Canonical je **signal, a ne naredba**.

Google može izabrati drugačiji canonical ako proceni da je druga URL verzija korisnija ili bolje odgovara sadržaju. Zbog toga je najbolje kombinovati canonical sa konzistentnim internim linkovima, sitemapom i pravilnom URL strukturom.

## Zaključak

Canonical URL je mali, ali veoma važan deo tehničkog SEO-a. Njegova osnovna svrha je da pretraživačima pomogne da razumeju **koja URL adresa predstavlja glavnu verziju sadržaja**.

Ako praviš Jekyll sajt, WordPress sajt ili potpuno custom web projekat, pravilno postavljen canonical može pomoći da izbegneš nepotrebnu konfuziju oko dupliranih URL-ova i konsoliduješ SEO signale na željenu stranicu.
