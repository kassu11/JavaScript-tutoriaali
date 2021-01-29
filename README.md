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

## Tehtävä 0 | Opastus

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

---

<br>

## Tehtävä 1 | Hei maailma

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

---

<br>

## Tehtävä 2 | Toistoa ja pituutta

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

---

<br>

## Tehtävä 3 | Teksti boxi

- Tee konsoliin tekstiboxi `#` merkistä joka `ympäröi tekstiä`
- Teksti tallennetaan `olioon`, jotta sitä voi helposti muuttaa
- Tekstin `päällä` ja `alla` on `rivin vaihto`
- Tekstin `oikealla` ja `vasemmalla` on `2 väliä`
- Teksti on `ympäröity #` merkeillä
- Saat käyttää tähän tehtävään vaan yhtä `console.log()` komentoa

<br>

3 Esimerkki tulosta

```js
######################              |           ###########
#                    #              |           #         #
#  Moro olen teksti  #              |           #  lyhyt  #
#                    #              |           #         #
######################              |           ###########
                                    |
------------------------------------+----------------------

###########################################################
#                                                         #
#  tosi pitkä teksti joka venyy ja laatikko tulee mukana  #
#                                                         #
###########################################################
```

<details>
<summary>Vinkki 1</summary>

- Voit tehdä rivin vaihdon `"\n"` tekstillä

```js
console.log("Rivi1\nRivi2\nRivi3");
```

```js
Rivi1
Rivi2
Rivi3
```

</details>

<details>
<summary>Vastaus</summary>

```js
const teksti = "Moro olen teksti"
const tyhja = " ".repeat(teksti.length + 2);
const viiva = "#".repeat(teksti.length + 6) + "\n";

console.log(viiva + "#", tyhja, "#\n# ", teksti, " #\n#", tyhja, "#\n" + viiva);
```

</details>

---

<br>

## Tehtävä 4 | Neliö konsoliin

- Tee konsoliin `neliö` käyttämällä `#` merkkiä
- Neliö on `ontto sisältä` ja sen suhteet on `1/2`
  - Eli neliö voisi olla `20 pitkä` ja `10 korkea`
- Neliön `koko` määritetään `numerolla oliossa`
  - Käytät `kokoon yhtä oliota`, joka tallentaa `pituuden`
- Neliön `ei` tarvitse `toimia alle 10` olevilla numeroilla
- Tehtävässä saa käytetään yhtä `console.log()` komentoa

<br>

Esimerkki tulos

```js
##############################
#                            #
#                            #
#                            #
#                            #
#                            #
#                            #
#                            #
#                            #
#                            #
#                            #
#                            #
#                            #
#                            #
##############################

##########
#        #
#        #
#        #
##########

####################
#                  #
#                  #
#                  #
#                  #
#                  #
#                  #
#                  #
#                  #
####################
```

<details>
<summary>Vastaus</summary>

```js
const nelionKoko = 20;
const rivi = "#".repeat(nelionKoko) + "\n";
const tyhjaRivi = "#" + " ".repeat(nelionKoko - 2) + "#\n";

console.log(rivi + tyhjaRivi.repeat(nelionKoko / 2 - 2) + rivi);
```

</details>

---

<br>

## Tehtävä 5 | Logiikka operaattorit

Tietoa `if`, `>`, `<`, `&&`, `||`, `==` ja `!=` operaattoreista

```js
let luku = 5;

// Testaa onko olio "luku" pienempi kun 10
if(luku < 10) { // jos on, suorita kaikki koodi sen sisällä
  console.log(luku, "on pienempi kun 10");
  console.log("#".repeat(30));
}

luku = 32;

if(luku < 10) {
  console.log(luku, "on pienempi kun 10");
} 
else { // suorita tämä jos if lause ei suoritu
  console.log(luku, "ei suorittanut testiä");
}


if(luku > 50) { // tarkistaa ehdon
  console.log(luku, "on isompi kun 50");
}
else if(luku > 30) { // jos ei suoritu tarkistaa tämän
  console.log(luku, "on isompi kun 30");
}
else {  // jos mikään ei mennyt läpi suorittaa tämän
  console.log(luku, "ei ollut isompi kun 50 tai 30");
}

console.log("#".repeat(30));

console.log(10 > 5); // voit myös suorittaa logiikka operaattoreita näin
console.log(10 < 5); // palauttaa joko "true" tai "false"
// "false" on epätosi, "true" on tosi

console.log(luku == 32) // Voit myös testata, onko joku tasan tietty arvo
console.log(luku != 32) // Tämä on päinastoin, onko se jokin muu kun 32, jos on 32 palauttaa "false"



if(luku != 2) {
  if("c" > "b") {
    if(luku == 32) {
      console.log("Suoritettu");
    }
  }
}

// Voit laittaa monia ehtoja yhteen if lauseeseen
            // tämä on "ja" merkki
if(luku != 2 && "c" > "b" && luku == 32) { // jos kaikki ehdot on "true" se suorittaa if lauseen
  console.log("&& merkit on käytännöllisiä");
}

// || on tämä ehto, jos jompikumpi ehdoista tulee toteen, suorittuu if lause
if(4 < 100 || 10 + 50 == 60) {
  console.log("Suorittaa koska 10 + 50 on 60");
}
```

<br>

Odotettu lopputulos

```js
5 "on pienempi kun 10"
##############################
32 "ei suorittanut testiä"
32 "on isompi kun 30"
##############################
true
false
true
false
Suoritettu
&& merkit on käytännöllisiä
Suorittaa koska 10 + 50 on 60
```

<br>

- Tee sovellus joka palauttaa konsoliin `tietoa numerosta`
- Sovellus kertoo onko numero `positiivinen` vai `negatiivinen`
- Jos numero on nolla se sanoo `"Lukusi on 0"`
- Jos et laittamasi arvo `ei ole numero`, sanoo konsoli siitä jotain

<br>

Esimkerkki vastauksia

```js

######################## 
3 on positiivinen

######################## 
-2 on negatiivinin

######################## 
> 0
Lukusi on 0

######################## 
"dfgqw" ei ole numero!

######################## 
519 on positiivinen

######################## 
-345 on negatiivinin

######################## 
> -0
Lukusi on 0
```

<details>
<summary>Vinkki 1</summary>

- Voit testata `if` tauleessa onko luku jokin arvo

```js
if(luku == 5) {
  /* Jos luku on "5" kaikki sulkujen 
  sisällä olevat komennot suoritetaan */
  console.log("Luku on 5");
}
```

<details>
<summary>Vinkki 2</summary>

- Voit laittaa `if` lauseen jälkeen `else` tai `else if` lauseen
- `else` suorittuu jos `if` ei suoritu
- `else if` on niikun `if`, mutta suorittuu vaan, jos `if` ei suoritu ja `else if` logiikka on tosi

```js
const luku = 6;
if(luku == 5) {
  /* Jos luku on "5" kaikki sulkujen 
  sisällä olevat komennot suoritetaan */
  console.log("Luku on 5");
} else if(luku == 6) {
  /* suorittuu, jos luku ei ole "5" 
    ja luku on "6" */
  console.log("Luku on 6");
} else {
  /* =================================================
  # Jos if tai else if ei suorittunu, tämä suorittuu #
  ================================================= */
  console.log("Luku ei ollut 5 tai 6);
}
```

<details>
<summary>Vinkki 3</summary>

- `<` ja `>` taskistaa onko luku pienempi/suurempi kun joku

```js
if(luku < -5) console.log("Pienempi kun -5");
else if(luku > 5) console.log("Isompi kun 5");
```

</details>

</details>

</details>

<details>
<summary>Vastaus</summary>

```js
const luku = 0;

if(luku == 0) console.log("Lukusi on 0");
else if(luku > 0) console.log(`${luku} on positiivinen`);
else if(luku < 0) console.log(`${luku} on negatiivinin`);
else console.log(`"${luku}" ei ole numero!`)
```

</details>