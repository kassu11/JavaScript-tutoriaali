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

<br>

<details open>
<summary>Tehtävä 0 | Opastus</summary>

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