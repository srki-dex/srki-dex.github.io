---
title: "AJAX objašnjen jednostavno."
description: "AJAX objašnjen jednostavno: saznajte kako JavaScript komunicira sa serverom, kako radi fetch() i kako učitati podatke bez ponovnog učitavanja stranice."

image: "/assets/images/ajax.webp"

categories: 
  - web-dizajn
---

Ako si ikada koristio web sajt na kojem se deo sadržaja promeni bez ponovnog učitavanja cele stranice, vrlo je moguće da si koristio **AJAX**.

AJAX je skraćenica od **Asynchronous JavaScript and XML**. Iako se u nazivu nalazi XML, danas se najčešće koriste **JavaScript i JSON** za komunikaciju sa serverom.

## Šta je AJAX?

Najjednostavnije rečeno, AJAX omogućava JavaScript-u da pošalje zahtev serveru i dobije podatke **bez reloadovanja cele web stranice**.

Bez AJAX-a, scenario može izgledati ovako:

```text
Korisnik klikne dugme
        ↓
Browser šalje zahtev
        ↓
Server vraća celu stranicu
        ↓
Browser ponovo učitava stranicu
```

Sa AJAX-om:

```text
Korisnik klikne dugme
        ↓
JavaScript šalje zahtev
        ↓
Server vraća podatke
        ↓
JavaScript menja samo deo stranice
```

Zbog toga aplikacija može delovati mnogo brže i interaktivnije.

## Jednostavan primer

Recimo da imamo dugme:

```html
<button id="loadData">Učitaj podatke</button>

<div id="result"></div>
```

JavaScript može poslati zahtev serveru pomoću `fetch()` funkcije:

```javascript
document.getElementById("loadData").addEventListener("click", async () => {

    const response = await fetch("/api/data.php");

    const data = await response.json();

    document.getElementById("result").textContent = data.message;

});
```

Server može vratiti JSON:

```json
{
    "message": "Pozdrav sa servera!"
}
```

JavaScript zatim ubacuje poruku u `<div>` bez osvežavanja stranice.

## AJAX i PHP

AJAX se često koristi zajedno sa PHP-om.

Na primer:

```text
JavaScript
    ↓
fetch()
    ↓
PHP
    ↓
Baza podataka
    ↓
PHP vraća JSON
    ↓
JavaScript
    ↓
HTML stranica
```

Ovakav sistem možeš koristiti za kontakt forme, pretragu, filtriranje proizvoda, login sisteme, komentare i različite web aplikacije.

## Da li je AJAX tehnologija?

AJAX nije poseban programski jezik niti biblioteka.

To je način komunikacije između browsera i servera pomoću JavaScript-a i web API-ja.

Nekada se za AJAX koristio `XMLHttpRequest`:

```javascript
const xhr = new XMLHttpRequest();

xhr.open("GET", "/api/data.php");

xhr.onload = function () {
    console.log(xhr.responseText);
};

xhr.send();
```

Danas je `fetch()` uglavnom jednostavniji i moderniji način:

```javascript
fetch("/api/data.php")
    .then(response => response.json())
    .then(data => console.log(data));
```

## AJAX nije samo za velike sajtove

Ne moraš praviti kompleksnu aplikaciju da bi koristio AJAX.

Možeš ga koristiti za jednostavne stvari kao što su:

učitavanje dodatnih blog postova, filtriranje sadržaja, live search, kontakt forme, validacija podataka, učitavanje komentara, prikaz podataka iz baze, automatsko osvežavanje određenog dela stranice

## Zaključak

AJAX omogućava web stranici da komunicira sa serverom **bez potrebe da se cela stranica ponovo učita**.

Danas se AJAX najčešće realizuje pomoću JavaScript `fetch()` API-ja i JSON podataka. Kada razumeš osnovni princip:

```text
JavaScript → Server → JSON → JavaScript → HTML
```

otvara ti se mogućnost da praviš mnogo interaktivnije web sajtove i aplikacije.

Ako učiš HTML, CSS i JavaScript, razumevanje AJAX-a je odličan sledeći korak ka ozbiljnijem web developmentu.
