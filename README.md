# JavaScript opettelu tehtäviä

## Tehtävien rakenne ja kuvaus

- Tehtävät menevät suunnilleen `vaikeus` järjestyksessä
- Tehtävien ohessa opetetaan tarpeelliset koodit, joilla tehtävän voi suorittaa
- Aikaisemmin neuvottuja koodeja ei neuvota uudelleen
- Jokaisessa tehtävässä on lopussa `vastaus`, miten tehtävän voi suorittaa
  - Tehtäviin voi olla `useita oikeita vastauksia`
  - Kunhan lopputulos on sama, kun mitä kysyttiin, tehtävä on suoritettu
  - Kannattaa silti katsoa `"malli" vastausta`, jos siitä oppisi jotain
- Tehtävien lopussa on myös `vinkkejä` jos, olet jumissa

---

<br>

<details open>
<summary style="font-size: 1.5em">Tehtävä 0 | Opastus</summary>

Tässä on vähän aloitus koodia jotta pääset alkuun, ja näet miten asiat toimii

```js
// Tämä on kommentti
// Voin kirjoittaa mitä vaan tänne, eikä se vaikuta koodiin

/*
  Voin myös kommentoida
  paljon asiaa näillä merkeillä
*/

// Tässä on tapoja luoda olioita
var lukuA = 2;  // "var" on vanha tapa tehdä olioita, eikä sitä kannata käyttää enää, mutta sitä näkee koodissa joka on ennen 2015 tehty
let lukuB = 6;  // "let" ja "const" on uusia tapoja tehdä olioita, ja niitä kannattaa käyttää var tilalla
const lukuC = 10; // "let" tallentaa olin tiedon, mutta sitä voi muuttaa myöhemmin, "const" ei anna sitä muuttaa

console.log(lukuA + lukuB); // Näyttää konsolissa paljon on 2 + 6, eli 8
console.log("Voit myös laittaa teksti tänne"); // Tämä tulee myös konsoliin

lukuA = 15; // Voit muuttaa oliolle annettua vastausta näin
lukuB = 3;

console.log("lukuA on nyt", lukuA) // Voit yhdistää tekstiä ja olioita
console.log("lukuB on nyt" + lukuA) // "+" toimii myös, mutta ei luo väliä

lukuC = 4;  // Jos yrität muuttaa "lukuC", tulee error, koska olio luotiin "const" termillä, joka estää muutoksen
```

<br>

Odotettu lopputulos

```js
8
Voit myös laittaa teksti tänne
lukuA on nyt 15
lukuB on nyt15
> Uncaught TypeError: Assignment to constant variable.
    at code.js:23
```

</details>

---

<br>

<details open>
<summary style="font-size: 1.5em">Tehtävä 1 | Hei maailma</summary>

- Tee `2` oliota, tallenna toiseen `nimesi` ja toiseen `ikäsi`
- Näytä konsoolissa paljon `ikä olio` ja `54` on yhteensä
- Kirjoita konsooliin lause, käyttäen `2` edellistä oliota
  - Hei, olen `ikä` vuotta vanha ja nimeni on `nimi`!

<br>

Odotettu lopputulos

```js
72
Hei, olen 18 vuotta vanha ja nimeni on Kassu!
```

<details>
<summary>Vinkki 1</summary>

- Voit tehdä olion `const` tai `let` komennolla

```js
const uusiOlio = "olen tekstiä";
let muutettavaOlio = "olen myös tekstiä";

console.log(uusiOlio);
console.log(muutettavaOlio);
```

<br>

Odotettu lopputulos

```js
olen tekstiä
olen myös tekstiä
```

<details>
<summary>Vinkki 2</summary>

- Voit yhdistää olitoita `+` tai `,` merkillä

```js
const olioA = "yksi";
const olioB = "kaksi";
const olioC = "kolme";

console.log(olioA, olioB + olioC);
```

<br>

Odotettu lopputulos

```js
yksi kaksikolme
```

</details>

</details>

<details>
<summary>Vastaus</summary>

```js
const nimi = "Kassu";
const ika = 18;

console.log(ika + 54);
console.log("Hei, olen", ika, "vuotta vanha ja nimeni on", nimi + "!");
console.log(`Hei, olen ${ika} vuotta vanha ja nimeni on ${nimi}!`); // tää on myös tapa sekottaa tekstiä olioitten kanssa
```

</details>

</details>

---

<br>

<details open>
<summary style="font-size: 1.5em">Tehtävä 2 | Toistoa ja pituutta</summary>

Uutta tietoa `.repeat()`, `.length` ja matikka `operaattoreista`

```js
const viiva = "#".repeat(15); // toistaa merkin "#" 15 kertaa

console.log(viiva);
console.log("tämä viiva on", viiva.length, "merkkiä pitkä");
console.log(viiva.repeat(2));

console.log("\n") // Tämä tekee rivin vaihdon

console.log("5 + 5 on", 5 + 5);
console.log("8 - 3 on", 8 - 3);
console.log("10 jaettuna 2 on", 10 / 2);
console.log("5 kertaa 5 on", 5 * 5);
console.log("2 potenssiin 3 on", 2 ** 3);
console.log("42 jakojäännys on", 42 % 10, "jos se jaetaan 10");
console.log("16 neliöjuuri on", Math.sqrt(16));

console.log(viiva.repeat(2));
// "\t" tekee tabulaattorin consoliin
console.log("\t\ttekstii\n".repeat(5));
```

<br>

Odotettu lopputulos

```js
###############
tämä viiva on 15 merkkiä pitkä
##############################

5 + 5 on 10
8 - 3 on 5
10 jaettuna 2 on 5
5 kertaa 5 on 25
2 potenssiin 3 on 8
42 jakojäännys on 2 jos se jaetaan 10
16 neliöjuuri on 4
##############################
		tekstii
		tekstii
		tekstii
		tekstii
		tekstii
```

<br>

- Tee `olio` johon voi tallennetaan `tekstiä`
- Olion teksti kirjoitetaan konsooliin ja se saa alleviivauksen
- Alleviivaus on tehty vaikka `#` merkistä
  - Viiva on aina yhtäpitkä kun olio teksti

<br>

Odotettu lopputulos

```js
tää on teksti
#############

olen vielä pidempi teksti
#########################

olen vielä pidempi teksti !!!!!!!!!!!!!!!!!!!!!!!!!!!!!
#######################################################

u
#
```

<details>
<summary>Vinkki 1</summary>

- Voit käyttää `.length` komentoa jos haluat tietää tekstin pituuden

<details>
<summary>Vinkki 2</summary>

- Käytä `.repeat()` komentoa, joka toistaa tekstin monta kertaa haluat

```js
console.log("e".repeat(5)) // Tekee 5 "e" kirjainta
console.log("ha".repeat(8));
```

<br>

Odotettu lopputulos

```js
eeeee
hahahahahahahaha
```

</details>

</details>

<details>
<summary>Vastaus</summary>

```js
const teksti = "teksti tulee tähän";

console.log(teksti);
console.log("#".repeat(teksti.length));
```

</details>

</details>

---

<br>