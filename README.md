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

### Tehtävänanto

- Tässä on vähän aloitus koodia jotta pääset alkuun, ja näet miten asiat toimii
- Kopio koodi itsellesi ja leiki sillä vähän, kunnes tajuut miten se toimii

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
const lukuC = 10; // "let" tallentaa olion tiedon, mutta sitä voi muuttaa myöhemmin, "const" ei anna sitä muuttaa

console.log(lukuA + lukuB); // Näyttää konsolissa paljon on 2 + 6, eli 8
console.log("Voit myös laittaa teksti tänne"); // Tämä tulee myös konsoliin

lukuA = 15; // Voit muuttaa oliolle annettua vastausta näin
lukuB = 3;

console.log("lukuA on nyt", lukuA) // Voit yhdistää tekstiä ja olioita
console.log("lukuB on nyt" + lukuA) // "+" toimii myös, mutta ei luo väliä

lukuA = lukuA + 50; // Voit myös tehdä näin, joka ei olisi mahdollista normaalissa matikassa
console.log(lukuA);

lukuC = 4;  // Jos yrität muuttaa "lukuC", tulee error, koska olio luotiin "const" termillä, joka estää muutoksen
```

<br>

### Odotettu lopputulos

```js
8
Voit myös laittaa teksti tänne
lukuA on nyt 15
lukuB on nyt15
65
> Uncaught TypeError: Assignment to constant variable.
    at code.js:26
```

---

<br>

## Tehtävä 1 | Hei maailma

### Tehtävänanto

- Tee `2` oliota, tallenna toiseen `nimesi` ja toiseen `ikäsi`
- Näytä konsoolissa paljon `ikä olio` ja `54` on yhteensä
- Kirjoita konsooliin lause, käyttäen `2` edellistä oliota
  - Hei, olen `ikä` vuotta vanha ja nimeni on `nimi`!

<br>

### Odotettu lopputulos

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

## Uutta tietoa `.repeat()`, `.length` ja matikka `operaattoreista`

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

### Odotettu lopputulos

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

---

<br>

## Tehtävä 2 | Tekstin alleviivausta

### Tehtävänanto

- Tee `olio` johon voi tallentaa `tekstiä`
- Olion teksti kirjoitetaan konsooliin ja se saa alleviivauksen
- Alleviivaus on tehty vaikka `#` merkistä
  - Viiva on aina yhtäpitkä kun olio teksti

<br>

### Tässä 3 esimerkki tulosta

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

### Tehtävänanto

- Tee konsoliin tekstiboxi `#` merkistä joka `ympäröi tekstiä`
- Teksti tallennetaan `olioon`, jotta sitä voi helposti muuttaa
- Tekstin `päällä` ja `alla` on `rivin vaihto`
- Tekstin `oikealla` ja `vasemmalla` on `2 väliä`
- Teksti on `ympäröity #` merkeillä
- Saat käyttää tähän tehtävään vaan yhtä `console.log()` komentoa

<br>

### 3 Esimerkki tulosta

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

### Tehtävänanto

- Tee konsoliin `neliö` käyttämällä `#` merkkiä
- Neliö on `ontto sisältä` ja sen suhteet on `1/2`
  - Eli neliö voisi olla `20 pitkä` ja `10 korkea`
- Neliön `koko` määritetään `numerolla oliossa`
  - Käytät `kokoon yhtä oliota`, joka tallentaa `pituuden`
- Neliön `ei` tarvitse `toimia alle 10` olevilla numeroilla
- Tehtävässä saa käyttää yhtä `console.log()` komentoa

<br>

### 3 Esimerkki tulosta

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

## Tietoa `if`, `>`, `<`, `&&`, `||`, `==` ja `!=` operaattoreista

```js
let luku = 5; // Jos muutat tätä lukua, huomaat että vastaus vaihtuu

if(luku < 10) { // Testaa onko luku alle 10
  // Jos on, se suorittaa kaiken aalkosulkeitten sisällä
  console.log(luku, "on pienempi kun 10");
} 
else if(luku < 20) { // Jos eka tarkistus ei onnistu, tarkistaa tämän
  console.log(luku, "on pienempi kun 20");
}
else if(luku < 30) { // Sitten tarkistaa tämän
  console.log(luku, "on pienempi kun 30");
}
else { // Jos kaikki aikaisemmat tarkistukset eivät olleet tosia, suorittaa tämän
  console.log(luku, "ei suorittanut mitään testiä");
}

luku = 32;
if(luku > 50) { // tarkistaa ehdon
  console.log(luku, "on isompi kun 50");
}
else {  // Voit suoraan laittaa if, lauseen perään else
  console.log(luku, "ei ollut isompi kun 50");
}

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

// || on tai ehto, jos jompikumpi ehdoista tulee toteen, suorittuu if lause
if(4 > 100 || 10 + 50 == 60) {
  console.log("Suorittaa koska 10 + 50 on 60");
}

// Jokainen aaltosulje avaa uuden "ikkunan, jossa voi luoda omia olioita, joita ei voi käsitellä sen ulkopuolella"

if(2 < 5) {
  let testi = "tekstiä";
  console.log("suorittuu ekasta if lauseesta", testi) // Voin käsitellä oliota normaalisti täällä
  if(3 < 5) {
    console.log("suorittuu tokasta if lauseesta", testi); // voin myös käyttää sitä muissa if, lauseissa tämän sisällä
    let testi2 = "lisää tekstiä";
    console.log(testi2);
  }

  // En voi käyttää testi2 täällä, koska se luotiin toisessa "ikkunassa"
  // console.log(testi2) /* Tämä tekisi errorin*/
}

console.log("Tämä tekee errorin, koska olio luotiin if lauseen sisällä, eikä siihen ole oikeutta täältä");
console.log(testi);
```

<br>

### Odotettu lopputulos

```js
5 "on pienempi kun 10"
32 "ei ollut isompi kun 50"
true
false
true
false
Suoritettu
&& merkit on käytännöllisiä
Suorittaa koska 10 + 50 on 60
suorittuu ekasta if lauseesta tekstiä
suorittuu tokasta if lauseesta tekstiä
lisää tekstiä
Tämä tekee errorin, koska olio luotiin if lauseen sisällä, eikä siihen ole oikeutta täältä
> Uncaught ReferenceError: testi is not defined
    at code.js:67
```

---

<br>

## Tehtävä 5 | Positiivinen ja negatiivinen

### Tehtävänanto

- Tee sovellus joka palauttaa konsoliin `tietoa numerosta`
- Sovellus kertoo onko numero `positiivinen` vai `negatiivinen`
- Jos numero on nolla se sanoo `"Lukusi on 0"`
- Jos laittamasi arvo `ei ole numero`, sanoo konsoli siitä jotain

<br>

### Esimkerkki vastauksia

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

---

<br>

## Materiaalia `for` loopista

```js
let luku = 5;
console.log(luku);
luku += 10; // Lisää lukuun 10
console.log(luku);
luku += 20; // Lisää lukuun 20
console.log(luku);
luku -= 30; // Vähentää luvusta 30
console.log(luku);

console.log("ennen for looppia");
// For loop koostuu 3 osasta
  // 1. Luo olio
  // 2. If ehto, ja niin kauan kun se tulee toteen, for loop pysyy päällä
  // 3. Toiminto, mitä looppi tekee joka toistokerran jälkeen
for(let numero = 0; numero < 5; numero += 1) {
  console.log("for loop", numero);
}

console.log("for loopin jälkeen");

// ++ nostaa numeroa yhdellä
for(let eka = 0; eka < 3; eka++) {
  console.log("Ensimmäinen loop", eka);

  for(let toka = 2; toka > 0; toka--) {
    console.log("Toinen loop", `Eka: ${eka} Toka: ${toka}`);
  }
  // console.log(toka); /* Aiheuttaisi errorin */
}

// Vähän niikun if lauseissa, koska oliot "eka" ja "toka" luotiin for loopissa
// Niitä ei voi käyttää täällä

// console.log(eka); /* Aiheuttaisi errorin */

const teksti = "kauppa";
for(let num = 0; num < teksti.length; num++) {
  console.log(`tekstin "${teksti}" kirjain "${num}" on: ${teksti[num]}`);
}
```

<br>

### Esimerkin lopputulos

```js
5
15
35
5
ennen for looppia
for loop 0
for loop 1
for loop 2
for loop 3
for loop 4
for loopin jälkeen
Ensimmäinen loop 0
Toinen loop Eka: 0 Toka: 2
Toinen loop Eka: 0 Toka: 1
Ensimmäinen loop 1
Toinen loop Eka: 1 Toka: 2
Toinen loop Eka: 1 Toka: 1
Ensimmäinen loop 2
Toinen loop Eka: 2 Toka: 2
Toinen loop Eka: 2 Toka: 1
tekstin "kauppa" kirjain "0" on: k
tekstin "kauppa" kirjain "1" on: a
tekstin "kauppa" kirjain "2" on: u
tekstin "kauppa" kirjain "3" on: p
tekstin "kauppa" kirjain "4" on: p
tekstin "kauppa" kirjain "5" on: a
```

---

<br>

## Tehtävä 6 | Suorakulmion teko for loopilla

### Tehtävänanto

- Tee `10` korkea ja `35` leveä suorakolmio käyttäen `#` merkkiä
- Tehtässä saat käyttää vaan yhtä `console.log()` komentoa
- Et saa käyttää `.repeat()` koodia
- Joudut hyödyntämään `for` looppeja jotta saat tehtävän tehtyä

<br>

### Odotettu lopputulos

```js
###################################
###################################
###################################
###################################
###################################
###################################
###################################
###################################
###################################
###################################
```

<details>
<summary>Vinkki 1</summary>

```js
const luku1 = 5;
const luku2 = 3;

for(let i = 0; i < luku1; i++) {

  // Voit laittaa for looppeja sisäkkäin O_o
  for(let i2 = 0; i2 < luku2; i2++) {
    console.log("luku1:", i, "luku2:", i2);
  }

  if(i < luku1 - 1) console.log("#".repeat(17));
}
```

Esimerkin lopputulos

```js
luku1: 0 luku2: 0
luku1: 0 luku2: 1
luku1: 0 luku2: 2
#################
luku1: 1 luku2: 0
luku1: 1 luku2: 1
luku1: 1 luku2: 2
#################
luku1: 2 luku2: 0
luku1: 2 luku2: 1
luku1: 2 luku2: 2
#################
luku1: 3 luku2: 0
luku1: 3 luku2: 1
luku1: 3 luku2: 2
#################
luku1: 4 luku2: 0
luku1: 4 luku2: 1
luku1: 4 luku2: 2
```

</details>

<details>
<summary>Vastaus</summary>

```js
let text = "";
const leveys = 35;
const korkeus = 10;

for(let y = 0; y < korkeus; y++) {
  let rivi = "";
  for(let x = 0; x < leveys; x++) {
    rivi += "#";
  } text += rivi + "\n";
}

console.log(text);
```

</details>

---

<br>

## Tehtävä 7 | Alleviivaus väleillä

### Tehtävänanto

- Tee `tehtävä 2`, mutta alleviivaus ei mene `väleihin`
- Jos tekstissä `ei ole välejä` se tekee samanlailla kun tehtävä 2

<br>

### Odotettu lopputulos

```js
olen teksti jossa on välejä
#### ###### ##### ## ######
```

<details>
<summary>Vinkki 1</summary>

- Voit käydä tekstin läpi `for` loopilla

```js
const text = "wow";

for(let i = 0; i < text; i++) {
  console.log(text[i]);
}
```

</details>

<details>
<summary>Vastaus</summary>

```js
const teksti = "olen teksti jossa on välejä";
let viiva = "";

for(let i = 0; i < teksti.length; i++) {
  if(teksti[i] == " ") viiva += " ";
  else viiva += "#";
}

console.log(teksti + "\n" + viiva);
```

</details>

---

<br>

## Tehtävä 8 | Kertoma laskuri

### Tehtävänanto

- Tee `laskuri` joka laskee `annetun luvun kertoman`
- Luvun `kertoma` eli `factorial` lasketaan näin
  - Esim luvun `3` kertoma on `3 * 2 * 1 = 6`
  - Luvun `6` kertoma on `6 * 5 * 4 * 3 * 2 * 1 = 120`
- Tannennat haluamasi `kertoman luvun` olioon
- Tulosta konsoliin `lasku yhtälö` ja `vastaus`

<br>

### 5 Esimerkki tapausta

```js
"7" kertoma on: 7 * 6 * 5 * 4 * 3 * 2 * 1 = 5040

"1" kertoma on 1

Laskuri ei tue negatiivisia numeroita

"0" kertoma on 0

"4" kertoma on: 4 * 3 * 2 * 1 = 24
```

<details>
<summary>Vastaus</summary>

```js
const kertoma = 8;
let vastaus = kertoma;
let yhtälö = `${kertoma}`;

for(let uusiLuku = kertoma - 1; uusiLuku > 0; uusiLuku--) {
  vastaus *= uusiLuku;
  yhtälö += " * " + uusiLuku;
}

if(kertoma < 0) console.log("Laskuri ei tue negatiivisia numeroita");
else if(kertoma < 2) console.log(`"${kertoma}" kertoma on ${kertoma}`);
else console.log(`"${kertoma}" kertoma on: ${yhtälö} = ${vastaus}`);
```

</details>

---

<br>

## Tehtävä 9 | Tekstistä etsimistä

### Tehtävänanto

- Tee `olio` johon `tallennat tektiä`
- Tee toinen `olio` johon `tallennat tekstijonon` jota haluat `etsiä` edellisestä oliosta
- Sovellus palauttaa konsoliin
  - Tekstin `josta` etsitään
  - Tekstin `mitä` etsitään
  - `Monta kertaa` etsittävä teksti `löydettiin`

<br>

### Esimerkki tapauksia

```js
tekstistä "kauppa sulkeutuu viideltä" löytyi 1 kertaa teksti "ppa"

tekstistä "kauppa sulkeutuu viideltä" löytyi 5 kertaa teksti "u"

tekstistä "kauppa sulkeutuu viideltä" löytyi 1 kertaa teksti "sulkeutuu viideltä"

tekstistä "yksi kaksi kolme neljä viisi" löytyi 4 kertaa teksti " "

tekstistä "yksi kaksi kolme neljä viisi" löytyi 3 kertaa teksti "si"
```

<details>
<summary>Vastaus</summary>

```js
const etsittavaTeksti = "asd";
const teksti = "miten menee olen teksti";

let etsiNumero = 0;
let montaLoytynyt = 0;

for(let kirjain of teksti) {
  if(kirjain == etsittavaTeksti[etsiNumero]) {
    etsiNumero++;
    if(etsiNumero == etsittavaTeksti.length) {
      montaLoytynyt++;
      etsiNumero = 0;
    }
  } else etsiNumero = 0;
}

console.log(`tekstistä "${teksti}" löytyi ${montaLoytynyt} kertaa teksti "${etsittavaTeksti}"`);
```

</details>

---

<br>

## Tehtävä 10 | Kolmion piirtäminen

### Tehtävänanto

- Piirrä konsoliin `kolmio`
- Kolmion `pohjan koko` määritellään `oliossa` numerolla
- Kolmio on piirretty konsoliin `*` merkillä

<br>

### Esimerkki tuloksia

```js
    *
   **
  ***
 ****
*****

       *
      **
     ***
    ****
   *****
  ******
 *******
********

              *
             **
            ***
           ****
          *****
         ******
        *******
       ********
      *********
     **********
    ***********
   ************
  *************
 **************
***************
```

<details>
<summary>Vastaus</summary>

```js
const koko = 100;

for(let i = 1; i <= koko; i++) {
  console.log(" ".repeat(koko - i) + "*".repeat(i));
}
```

</details>

---

<br>

## Opetus materiaalia `.indexOf()`, `.toUpperCase()`, `.toLowerCase()` ja `pyöristys` operaattoreista

```js
// Etsii tekstistä tietyn kirjain arvon, ja palauttaa sen index numeron
console.log("abcdefghijklmnop".indexOf("g"));
console.log("abcdefghijklmnop".indexOf("lmn"));
// Jos arvoa ei löydy tekstistä palauttaa -1
console.log("kauppa".indexOf("o"));

// muuttaa jokaisen kirjaimen isoksi
console.log("Kaikki On Isolla".toUpperCase());
// muuttaa jokaisen kirjaimen pieneksi
console.log("KAIKKI ON PIENELLÄ".toLowerCase());

for(let i = 0; i < 10; i++) {
  console.log("Aloittaa", i);

  // "%" on joka jäännös
  // se testaa montakertaa joku on jaollinen, ja paljon siitä jää yli
    // Esim 3 % 2 == 1
    // Esim 6 % 2 == 0
  if(i > 6) break;  // Jos luku on yli 6 se poistuu loopista
  if(i % 2 == 0) continue; // Jos luku on parillinen, se alottaa seuraavaan kierroksen loopista
  console.log("\tLopettaa", i);
}

let luku = 5;
while(2 < 100) {
  luku += 5;
  console.log("while loop on toinen loop, joka ei vaadi kun vaan yhden ehdon", luku);
  if(luku > 20) break;
}

console.log(Math.ceil(8.9), Math.ceil(3.1)); // Pyöristää ylöspäin
console.log(Math.floor(8.9), Math.floor(3.1)); // Pyöristää alaspäin
console.log(Math.round(8.9), Math.round(3.1), Math.round(7.5)); // Pyöristää normaalisti
```

---

<br>

## Tehtävä 11 | Tuplakirjainten löytäminen

### Tehtävänanto

- Tallenna etsittävä `teksti olioon`
- Sovellus etsii `onko` tekstissä yhtään `kirjainta keksi kertaa`
  - `Ensimmäinen` kirjain jota löytyy `2 kertaa kirjoitetaan konsoliin`
  - Jos samoja kirjaimia ei tekstissä `ole yli 1`, `sanotaan siitä konsoliin`

<br>

### Esimerkki tuloksia

```js
ensimmäinen tuplakirjain tekstissä "koiran ruoka on lopussa" on "r"

tekstissä "kirja" ei ollut yhtään tuplakirjainta

ensimmäinen tuplakirjain tekstissä "erkin omena" on "e"

ensimmäinen tuplakirjain tekstissä "kissa kehrää" on "s"
```

</details>

<details>
<summary>Vinkki 1</summary>

- Voit käyttää `indexOf()` functiota löytämään onko tekstissä mitä etsit

```js
console.log("abcd".indexOf("g")) // palauttaa -1 koska ei löytynyt

console.log("terve".indexOf("t")) // palauttaa 0, koska "t" oli ensimmäinen kirjain

const nimi = "Pertti";

if(nimi.indexOf("ö") == -1) {
  console.log(`nimestäsi ei löytynyt "ö" kirjainta`);
}
```

<details>
<summary>Vinkki 2</summary>

- Voit käyttää `break` komentoa jos haluat poistua `for` loopista

```js
for(let i = 0; i < 100; i++) {
  console.log(i);
  if(i > 10) break; // Lopettaa loopin, jos "i" menee yli 10
}
```

</details>

</details>

<details>
<summary>Vastaus</summary>

```js
const teksti = "koiran ruoka on lopussa";
const tarkistetutKirjaimet = [];
let tuplakirjain = "";

for(const kirjain of teksti) {
  if(tarkistetutKirjaimet.indexOf(kirjain) !== -1) {
    tuplakirjain = kirjain;
    break;
  } else tarkistetutKirjaimet.push(kirjain);
}

if(tuplakirjain) {
  console.log(`ensimmäinen tuplakirjain tekstissä "${teksti}" on "${tuplakirjain}"`);
} else {
  console.log(`tekstissä "${teksti}" ei ollut yhtään tuplakirjainta"`);
}
```

</details>

---

<br>

## Tehtävä 12 | Pyramiidin teko

### Tehtävänanto

- Tee konsoliin pyramiidi `*` merkeistä
- Tehtävässä `saa käyttää vaan yhtä console.log()` lausetta
- Pyramiidin `koko` määritetään `oliolla`
  - `Olio` kertoo pyramiidin `pohjan leveyden`
  - Leveys `pyöristetään alaspäin`, esim `4 leveys olis 3`

<br>

### Esimerkki tuloksia

```js
> 15
       *
      ***
     *****
    *******
   *********
  ***********
 *************
***************

> 4
 *
***

> 6
  *
 ***
*****
```

<details>
<summary>Vinkki 1</summary>

- Voit käyttää `%` matikka operaattoria laskemaan `jakojäännöksen`
- Jakojäännöksellä voit helposti tarkistaa onko luku `parinninen` vai ei

```js
if(120 % 2 == 0) console.log("luku 120 on parinninen");
if(132 % 3 == 0) console.log("luku 132 on jaollinen 3");

console.log(11 % 5) // "11" menee lukuun "5" kaksi kertaa, ja siitä jää 1 yli
```

</details>



<details>
<summary>Vastaus</summary>

```js
const koko = 15;
let pyramiidi = "";
let valit = koko / 2;
// tarkistaa onko luku jaollinen 2, jos on pyöristää alaspäin
if(koko % 2 == 0) valit = (koko - 1) / 2;


for(let i = 1; i <= koko; i += 2) {
  pyramiidi += " ".repeat(valit--) + "*".repeat(i) + "\n";
} if(koko > 0) console.log(pyramiidi);
```

</details>