# Sisällysluettelo

- [JavaScript opettelu tehtäviä](#javascript-opettelu-tehtäviä)
  - [Tehtävä 1.0 | Oliot ja konsoliin kirjoittaminen](#tehtävä-10--oliot-ja-konsoliin-kirjoittaminen)
    - [Tehtävä 1.1 | Hei maailma](#tehtävä-11--hei-maailma)
    - [Tehtävä 1.2 | Olion muokkaamista](#tehtävä-12--olion-muokkaamista)
  - [Tehtävä 2.0 | .repeat(), .length ja matikka operaattorit](#tehtävä-20--repeat-length-ja-matikka-operaattorit)
    - [Tehtävä 2.1 | Täydellinen neliö](#tehtävä-21--täydellinen-neliö)
    - [Tehtävä 2.2 | Tekstin alleviivausta](#tehtävä-22--tekstin-alleviivausta)
    - [Tehtävä 2.3 | Teksti boxi](#tehtävä-23--teksti-boxi)
    - [Tehtävä 2.4 | Neliö konsoliin](#tehtävä-24--neliö-konsoliin)
  - [Tehtävä 3.0 | Tietoa if, >, <, &&, ||, == ja != operaattoreista](#tehtävä-30--tietoa-if------ja--operaattoreista)
    - [Tehtävä 3.1 | Positiivinen ja negatiivinen](#tehtävä-31--positiivinen-ja-negatiivinen)
    - [Tehtävä 3.2 | Digitaaliset numerot](#tehtävä-32--digitaaliset-numerot)
    - [Tehtävä 3.3 | Salasanan tarkistus](#tehtävä-33--salasanan-tarkistus)
    - [Tehtävä 3.4 | Jaolliset numerot](#tehtävä-34--jaolliset-numerot)
    - [Tehtävä 3.5 | Tekstin keskitys](#tehtävä-35--tekstin-keskitys)
  - [Tehtävä 4.0 | Materiaalia for loopista, += ja -= operaattoreista](#tehtävä-40--materiaalia-for-loopista--ja---operaattoreista)
    - [Tehtävä 4.1 | Ensimmäinen ja viimeinen kirjain](#tehtävä-41--ensimmäinen-ja-viimeinen-kirjain)
    - [Tehtävä 4.2 | Portaitten teko](#tehtävä-42--portaitten-teko)
    - [Tehtävä 4.3 | Kolmion piirtäminen](#tehtävä-43--kolmion-piirtäminen)
    - [Tehtävä 4.4 | Suorakulmion teko for loopilla](#tehtävä-44--suorakulmion-teko-for-loopilla)
    - [Tehtävä 4.5 | Alleviivaus väleillä](#tehtävä-45--alleviivaus-väleillä)
    - [Tehtävä 4.6 | Kertoma laskuri](#tehtävä-46--kertoma-laskuri)
    - [Tehtävä 4.7 | Tekstistä etsimistä](#tehtävä-47--tekstistä-etsimistä)
    - [Tehtävä 4.8 | Pyramidin teko](#tehtävä-48--pyramidin-teko)
    - [Tehtävä 4.9 | Onton pyramidin teko](#tehtävä-49--onton-pyramidin-teko)
  - [Tehtävä 5.0 | Opetus materiaalia .indexOf(), .toUpperCase(), .toLowerCase() ja pyöristys operaattoreista](#tehtävä-50--opetus-materiaalia-indexOf-toUpperCase-toLowerCase-ja-pyöristys-operaattoreista)
    - [Tehtävä 5.1 | Tuplakirjainten löytäminen](#tehtävä-51--tuplakirjainten-löytäminen)
    - [Tehtävä 5.2 | Palindromin tunnistus](#tehtävä-52--palindromin-tunnistus)
    - [Tehtävä 5.3 | Isot alkukirjaimet](#tehtävä-53--isot-alkukirjaimet)
  - [Tehtävä 6.0 | Taulut, objectit ja random numerot](#tehtävä-60--taulut-objectit-ja-random-numerot)

<br>

# JavaScript opettelu tehtäviä

## Tehtävien rakenne ja kuvaus

- Tehtävät menevät suunnilleen `vaikeus` järjestyksessä
  - Jokainen `.0` tehtävä, neuvoo jotain uutta
  - Jos olet omasta mielestä oppinut .0 asiat, voit mennä seuraavaan numeroon
- Tehtävien ohessa opetetaan tarpeelliset koodit, joilla tehtävän voi suorittaa
- Aikaisemmin neuvottuja koodeja ei neuvota uudelleen
- Jokaisessa tehtävässä on lopussa `vastaus`, miten tehtävän voi suorittaa
  - Tehtäviin voi olla `useita oikeita vastauksia`
  - Kunhan lopputulos on sama, kun mitä kysyttiin, tehtävä on suoritettu
  - Kannattaa silti katsoa `"malli" vastausta`, jos siitä oppisi jotain
  - Jos tehtävää ei millään, saa läpi, vastauksen voi ajatuksella käydä läpi
- Tehtävien lopussa on myös `vinkkejä` jos, olet jumissa

---

<br>

## Tehtävä 1.0 | `Oliot` ja `konsoliin kirjoittaminen`

### Opetus materiaali

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

let tekstiA = "miten menee";
console.log(tekstiA);

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
miten menee
> Uncaught TypeError: Assignment to constant variable.
    at code.js:26
```

---

<br>

## Tehtävä 1.1 | Hei maailma

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

## Tehtävä 1.2 | Olion muokkaamista

### Tehtävänanto

- Tee `yksi olio` johon tallennat aloitus arvon `5`
- `Olion nimi` on `muuttuja`
- Tee uusi rivi ja `lisää` olion arvoon `5`
- Uudella rivillä `lisää` olion arvoon teksti `on numero` perään
- Tehtävässä pitää tulostaa vastas `console.log(muuttuja)` komennolla

<br>

### Odotettu lopputulos

```js
10 on numero
```

<details>
<summary>Vinkki 1</summary>

```js
let teksti = "oho";
teksti = teksti + ", onpa kaunis päivä";
console.log(teksti);
```

</details>

<details>
<summary>Vastaus</summary>

```js
let muuttuja = 5;
muuttuja = muuttuja + 5;
muuttuja = muuttuja + " on numero";
console.log(muuttuja);
```

</details>

---

<br>

## Tehtävä 2.0 | `.repeat()`, `.length` ja matikka `operaattorit`

### Selitykset

- `.length` kertoo tekstin pituuden
- `.repeat()` toistaa tietyn tekstijanan annetus numeron verran
  - Jos laittaa `0`, se ei palauta tekstiä ollenkaan
- `\n` tämä on rivin vaihto koodikielenä
  - Jos haluat laittaa montarivisiä tekstejä konsooliin, käytä `\n`
- `\t` on tabulaattori, eli vähän isompi väli perjaattessa

### Opetus materiaali

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
console.log("42 jakojäännös 10 on", 42 % 10);
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
42 jakojäännös 10 on 2
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

## Tehtävä 2.1 | Täydellinen neliö

### Tehtävänanto

- Tee konsoliin neliö `#` merkeistä
- Neliön `koko` määritetään `oliolla`
  - Jos `olion arvo` on esim `5`, tulee neliön olla `5x5 kokoinen`

<br>

### 3 Esimerkki tulosta

```js
##
##

#####
#####
#####
#####
#####

##########
##########
##########
##########
##########
##########
##########
##########
##########
##########
```

<details>
<summary>Vinkki 1</summary>

- Käytä `.repeat()` komentoa, joka toistaa tekstin monta kertaa haluat

```js
console.log("e".repeat(5)) // Tekee 5 "e" kirjainta
console.log("ha".repeat(8));
```

```js
eeeee
hahahahahahahaha
```

<details>
<summary>Vinkki 2</summary>

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

</details>

<details>
<summary>Vastaus</summary>

```js
const koko = 5;
const rivi = "#".repeat(koko) + "\n";

console.log(rivi.repeat(koko));
```

</details>

---

<br>

## Tehtävä 2.2 | Tekstin alleviivausta

### Tehtävänanto

- Tee `olio` johon voi tallentaa `tekstiä`
- Olion `teksti` kirjoitetaan konsooliin ja se saa `alleviivauksen`
- `Alleviivaus` on tehty vaikka `#` merkistä
  - Viiva on `aina yhtäpitkä kun olio teksti`
- Tehtävässä `saa käyttää` vain yhtä `console.log()` komentoa 

<br>

### Tässä 4 esimerkki tulosta

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

## Tehtävä 2.3 | Teksti boxi

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

## Tehtävä 2.4 | Neliö konsoliin

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
<summary>Vinkit 1</summary>

```js
const rahat = 100;
console.log("Puolet", rahat + "€ on", rahat/2 + "€");
```

```js
Puolet 100€ on 50€
```

</details>

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

## Tehtävä 3.0 | Tietoa `if`, `>`, `<`, `&&`, `||`, `==` ja `!=` operaattoreista

### Selitykset

- Koodaamisen tärkein komento on `if` ja `else` lauseet
- Voit käyttää `if` lauseita `monimutkaisiin` tai `yksinkertaisiin` kyselyihin
  - Ilman näitä ei voitaisi tehdä mitään `valinta kysymyksia` tai muita `logiikka` asioita
  - `if` lause `testaaa` palauttaako ehto `true` vai `false` arvon
  - `if` lauseen `suoritettava koodi`, laitetaan `{}` aaltosulkeisiin
    - Kaikki `oliot` jotka on `luotu aaltosulkeiden sisällä`, pysyy siellä, eikä niitä voi `käsitellä` niitten `ulkoupuolella`
  - `if` lauseen `ehto` laitetaan `()` sulkeisiin
    - Jos `arvo` on `true`
      - Suorittaa `if` lause kaiken `koodin mikä sen sisälle on` laitettu suorittumaan
    - Jos `arvo` on `false`
      - Ohittaa `if` kaiken sen `sisällä olevan koodin`
      - Jos `if` lauseen `jälkeen` on `else` tai `else if`, suorittaa koodi sen
        - `else if` lauseen ehto tarkistetaan myös vastaavasti, ja jatketaan samaan malliin
        - `else` lauseessa ei ole `ehtoa`, ja `suorittuu` aina jos edeltävä `if` tai `else if` lause `ei suoritu`

### Opetus materiaali

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
console.log(luku != 32) // Tämä on päinvastoin, onko se jokin muu kun 32, jos on 32 palauttaa "false"

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

## Tehtävä 3.1 | Positiivinen ja negatiivinen

### Tehtävänanto

- Tee sovellus joka palauttaa konsoliin `tietoa numerosta`
- Sovellus kertoo onko numero `positiivinen` vai `negatiivinen`
- Jos numero on `nolla` se sanoo `"Lukusi on 0"`
- Jos laittamasi arvo `ei ole numero`, sanoo konsoli siitä jotain

<br>

### 7 Esimerkki tulosta

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

## Tehtävä 3.2 | Digitaaliset numerot

### Tehtävänanto

- Luo `olio` johon `tallennetaan` luku `arvo 0-9 väliltä`
- `Arvosta` tulostetaan konsooliin digitaalinen numero `#` merkkejä käyttäen
- Mikäli olion arvo ei ole `0-9` välillä, tulee siitä `viesti konsoliin`
- Esimerkki numerot alhaalla
  - Voit tyylitellä itse, jos haluat
    ```js
    ###   #   ###  ###  # #  ###  ###  ###  ###  ###
    # #  ##     #    #  # #  #    #      #  # #  # #
    # #   #   ###  ###  ###  ###  ###    #  ###  ###
    # #   #   #      #    #    #  # #   #   # #    #
    ###  ###  ###  ###    #  ###  ###   #   ###  ###
    ```

<br>

### 4 Esimerkki tulosta

```js
###
  #
###
  #
###

###
  #
  #
 # 
 # 

Antamasi arvo ei ollut numero 0-9 väliltä

###
# #
###
  #
###
```

<details>
<summary>Vastaus</summary>

```js
const numero = 5;

if(numero == 0) {
  console.log("###\n# #\n# #\n# #\n###\n");
} else if(numero == 1) {
  console.log(" # \n## \n # \n # \n###\n");
} else if(numero == 2) {
  console.log("###\n  #\n###\n#  \n###\n");
} else if(numero == 3) {
  console.log("###\n  #\n###\n  #\n###\n");
} else if(numero == 4) {
  console.log("# #\n# #\n###\n  #\n  #\n");
} else if(numero == 5) {
  console.log("###\n#  \n###\n  #\n###\n");
} else if(numero == 6) {
  console.log("###\n#  \n###\n# #\n###\n");
} else if(numero == 7) {
  console.log("###\n  #\n  #\n # \n # \n");
} else if(numero == 8) {
  console.log("###\n# #\n###\n# #\n###\n");
} else if(numero == 9) {
  console.log("###\n# #\n###\n  #\n###\n");
} else {
  console.log("Antamasi arvo ei ollut numero 0-9 väliltä");
}
```

</details>

---

<br>

## Tehtävä 3.3 | Salasanan tarkistus

- Tee sovellus joka tarkistaa miten `turvallinen salasanasi on`
  - Jos salasana on `alle 5 merkkiä`, se on `liian lyhyt`
  - Jos salasanassa on `alle 9 merkkiä`, se on `keskiverto`
  - Jos salasana on `alle 20 merkkiä` se on `pitkä`
  - Jos salasana on `yli 20 merkkiä` se on `liian pitkä`
  - Mikäli käyttäjä `ei laita salasanaa` sanotaan siitä konsooliin
- Salasanan `turvallisuus kerrotaan konsooliin`, ja `salansana näkyy` siinä `salattuna`

<br>

### Esimerkki tuloksia

```js
salasanasi ******* on keskiverto

salasanasi *** on liian lyhyt

salasanasi ********* on pitkä

salasanasi ************** on liian pitkä

laita salasana
```

<details>
<summary>Vastaus</summary>

```js
const salasana = "";

if(salasana.length == 0) {
  console.log("laita salasana");
} else if(salasana.length < 5) {
  console.log("salasanasi", "*".repeat(salasana.length), "on liian lyhyt");
} else if(salasana.length < 9) {
  console.log("salasanasi", "*".repeat(salasana.length), "on keskiverto");
} else if(salasana.length < 20) {
  console.log("salasanasi", "*".repeat(salasana.length), "on pitkä");
} else {
  console.log("salasanasi", "*".repeat(salasana.length), "on liian pitkä");
}
```

</details>

---

<br>

## Tehtävä 3.4 | Jaolliset numerot

### Tehtävänanto

- Tee sovellus joka `testaa` onko luku `jaollinen` `3`, `4` tai `7`
- `Tarkistettava` luku tallennetaan `olioon`
- `Millä` luku `on jaollinen` kerrotaan konsoliin
- Jos luku `ei ole jaollinen` millään `sanotaan siitä`
- Mikäli luku on jaollinen `monella luvulla`, sanotaan `kaikki niistä millä sen voi jakaa` tasan

<br>

### 7 Esimerkki tulosta

```js
"12" on jaollinen numeroilla "3" ja "4"

"5" ei olle jaollinen "3", "4" tai "7"

"84" on jaollinen "3", "4" sekä "7"!

"28" on jaollinen numeroilla "4" ja "7"

"14" on jaollinen numerolla "7"

"8" on jaollinen numerolla "4"

"abc" ei olle jaollinen "3", "4" tai "7"
```

<details>
<summary>Vinkki 1</summary>

- jakojäännöksen voi laskea `%` merkillä
- Jakojäännöstä voi ajatella niikun jakaisi karkkia
  - Jos yrität jakaa `5` karkkia `6` ihmiselle eli `5 % 6`
    - jää yli `5` karkkia, koska niitä ei voi jakaa tasaisesti
  - `7 % 6` jää yli `1` karkki
  - `6 % 6` jää yli `0`, koska kaikki karkit jaettiin tasan 

```js
console.log(13 % 6);
console.log(12 % 6);
console.log(17 % 6);
console.log(5 % 6);

if(12 % 6 == 0) console.log("on jaollinen kuudella");
```

```js
1
0
5
5
on jaollinen kuudella
```

</details>

<details>
<summary>Vastaus</summary>

```js
const numero = 56;
let jaolliset = "";

if(numero % 3 == 0 && numero % 4 == 0 && numero % 7 == 0) {
  console.log(`"${numero}" on jaollinen "3", "4" sekä "7"!`);
} else {
  if(numero % 3 == 0) {
    if(jaolliset.length > 0) jaolliset = jaolliset + ` ja "3"`;
    else jaolliset = `"3"`;
  } if(numero % 4 == 0) {
    if(jaolliset.length > 0) jaolliset = jaolliset + ` ja "4"`;
    else jaolliset = `"4"`;
  } if(numero % 7 == 0) {
    if(jaolliset.length > 0) jaolliset = jaolliset + ` ja "7"`;
    else jaolliset = `"7"`;
  }

  if(jaolliset.length > 3) {
    console.log(`"${numero}" on jaollinen numeroilla ${jaolliset}`);
  } else if(jaolliset.length > 0) {
    console.log(`"${numero}" on jaollinen numerolla ${jaolliset}`);
  } else {
    console.log(`"${numero}" ei olle jaollinen "3", "4" tai "7"`);
  } 
}
```

</details>

---

<br>

## Tehtävä 3.5 | Tekstin keskitys

### Tehtävänanto

- Luo `olio` johon laitat boxin `minimi leveys`
- Tee `tekstille olio`, johon laitetaan `boxiin ilmestyvä teksti`
- `Teksti` tulee piirtää konsoliin, ja sen `ympärillä` on reunat `#` merkeistä
  - `Teksti` on `keskitetty` `vasemmalta` ja `oikealta` päin
  - Jos tekstiä `ei voi keskittää tasaisesti`, tulee reunoista `yksi isompi`
- Jos `teksti on isompi kun minimi` laatikon koko, tulee se `venymään tekstin mukana`
  - `Reinoissa pitää aina olla` vähintään `yksi väli`, `oikeilla` ja `vasemmalla`

<br>

### 7 Esimerkki tulosta

```js
################
#  <-- 16 -->  #
################

#################
#  <-- 16! -->  #
#################

#################
#      -_-      #
#################

###################
# saippuakauppias #
###################

##########################################
# saippuakauppias menee myymään saippuaa #
##########################################

########################
#      <-- 23 -->      #
########################

#######################
#     <-- 23! -->     #
#######################
```

<details>
<summary>Vastaus</summary>

```js
const teksti = "tekstiä";
const maxPituus = 23;

if(teksti.length < maxPituus - 2) {
  if((maxPituus - teksti.length) % 2 == 0) { // Luku on parillinen
    const valienMaara = (maxPituus - teksti.length) / 2 - 1;
    const valit = " ".repeat(valienMaara);
    console.log("#".repeat(maxPituus) + "\n#" + valit + teksti + valit + "#\n" + "#".repeat(maxPituus));
  } else { // Luku ei ole parillinen
    const valienMaara = (maxPituus + 1 - teksti.length) / 2 - 1;
    const valit = " ".repeat(valienMaara);
    console.log("#".repeat(maxPituus + 1) + "\n#" + valit + teksti + valit + "#\n" + "#".repeat(maxPituus + 1));
  }
} else {
  const pituus = teksti.length + 4;
  console.log("#".repeat(pituus) + "\n#", teksti, "#\n" + "#".repeat(pituus));
}
```

</details>

---

<br>

## Tehtävä 4.0 | Materiaalia `for` loopista, `+=` ja `-=` operaattoreista

### Selitykset

- Jos haluat `nostaa` tai `laskea` `yhdellä olion arvoa` voit käyttää `++` tai `--`
  - Jos meillä on luotu tämmöinen olio `let lukuA = 2`
    - Sitten laitetaan `lukuA++` niin olion arvo muuttui `3`
    - Jos sitten laitetaan `lukuA--`, se vähentää olion arvoa yhdellä, eli tulee `2`
- `+=` `lisää` olion arvoon `laittamasi arvon`
  - Jos meillä on tämmöinen olio `let testA = 5`
    - `testA += 10` muuttaisi `testA` olion arvon `15`, koska `5 + 10` on `15`
    - `testA += "text"` muuttaa arvoksi `"5text"`
- `-=` `vähentää` olion arvosta `laittamasi arvon`
  - Toisin kuin `+=` niin `-=` toimii vain numeroilla, ja muuten se palauttaa `NaN`
    - `NaN` on JavaScript arvo jos luku `ei ole numero`
  - Jos meillä on tämmöinen olio `let testB = 5`
    - `testB -= 10` muuttaisi `testB` olion arvon `-5`, koska `5 - 10` on `-5`
    - `testB -= "text"` muuttaa arvoksi `NaN`
- `for` looppi koostuu `3 osasta`, jotka käydään läpi eri osassi looppia
  - `Ensimmäinen osa` on `aloitus koodi`, eli tämä suoritetaan `aina kun loop suorittuu ekan kerran`
  - `Toinen osa` on `if ehto`, joka kertoo miten kauan `loop on käynnissä`
    - `Niin kauan` kun ehto palauttaa `true`, pysyy `loop päällä`
    - Tämä ehto `tarkistetaan` joka `loopin jälkeen`, `ja ennen kun loop aloitetaan`
  - `Viimeinen osa` on koodi, joka suorittuu aina `joka loopin jälkeen`
    - `Tätä koodia ei suoriteta ensimmäisellä loopilla`, mutta sen `jälkeen` se `suorittuu joka looppi`
    - Tämä suorittuu myös `aina ennen toisen osaa`, jonka jälkeen `toinen osa tarkistetaan`
  - Loopin virallinen osien `suoritus järjestys` on
    - `1` > `2` > `suorittaa koodin sisällä` > `3` > `2` > `koodi säsällä` > `3` > `2` > ...

### Oppimis materiaali

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

## Tehtävä 4.1 | Ensimmäinen ja viimeinen kirjain

### Tehtävänanto

- Tee sovellus joka `etsii` tekstistä `ensimmäisen` ja `viimeisen kirjaimen`
  - `Kirjaimet` kerrotaan `konsooliin` `tekstin kanssa`
- Tarkistettava `teksti` `tallennetaan olioon`
- Jos tekstiä `ei anneta` `sanotaan siitä konsoliin`

<br>

### 5 Esimerkki tulosta

```js
tekstin "alumiini" ensimmäinen kirjain on "a" ja vika kirjain on "i"

tekstin "t" ensimmäinen kirjain on "t" ja vika kirjain on "t"

tekstin "olio" ensimmäinen kirjain on "o" ja vika kirjain on "o"

kirjoita jokin teksti tutkittavaksi

tekstin "tosi pitkä sana jossa on välejä" ensimmäinen kirjain on "t" ja vika kirjain on "ä"
```

<details>
<summary>Vinkki 1</summary>

- Voit käyttää `[]` kulmasulkeita `tektiis`, jos haluat valita `tietyn kirjaimen`

```js
const teksti = "ABCDEFG";
console.log(teksti[2]);
```

</details>

<details>
<summary>Vastaus</summary>

```js
const teksti = "kirja";
const eka = teksti[0];
const vika = teksti[teksti.length - 1];

if(teksti.length > 0) {
  console.log(`tekstin "${teksti}" ensimmäinen kirjain on "${eka}" ja vika kirjain on "${vika}"`);
} else {
  console.log("kirjoita jokin teksti tutkittavaksi");
}
```

</details>

---

<br>

## Tehtävä 4.2 | Portaitten teko

### Tehtävänanto

- Tee sovellus joka piirtää konsoliin portaat `#` merkeistä
- `Yksi` porras `koostuu 4` `#` merkistä
- jokainen `askelma` menee `2 merkkiä oikealle`
- Portaitten `lukumäärä` määritellään `oliolla`, johon laitetaan `numero arvo`

<br>

### 3 Esimerkki tulosta

```js
> 3
####
  ####
    ####

> 5
####
  ####
    ####
      ####
        ####

> 8
####
  ####
    ####
      ####
        ####
          ####
            ####
              ####
```

<details>
<summary>Vinkki 1</summary>

- Perus `for` loop pohja
- Ekana luodaan `olio` nimeltä `i`, arvolla `0`
- Sitten `tarkistetaan` onko `i` `pienempi` kun `10`
  - Jos on suorittuu looppi
  - `Aina` loopin suorittamisen jälkeen `i` olioon lisätään `1`
- Kun `i` menee `yli 10`, loop loppuu, koska ehto palauttaa `false`

```js
for(let i = 0; i < 10; i++) {
  console.log("Loop suoritettu", i);
}
```

</details>

<details>
<summary>Vastaus</summary>

```js
const rappuset = 10;

for(let rappunen = 0; rappunen < rappuset; rappunen++) {
  console.log(" ".repeat(rappunen * 2) + "####");
}
```

</details>

---

<br>

## Tehtävä 4.3 | Kolmion piirtäminen

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

## Tehtävä 4.4 | Suorakulmion teko for loopilla

### Tehtävänanto

- Tee `10` korkea ja `35` leveä suorakolmio käyttäen `#` merkkiä
- Tehtässä saat käyttää vaan yhtä `console.log()` komentoa
- Koko `suorakulmio` pitää olla tallennettu `olioon`, joka tulostetaan konsoliin `for loopin ulkona`
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

## Tehtävä 4.5 | Alleviivaus väleillä

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

for(let i = 0; i < text.length; i++) {
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

## Tehtävä 4.6 | Kertoma laskuri

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

## Tehtävä 4.7 | Tekstistä etsimistä

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

## Tehtävä 4.8 | Pyramidin teko

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

---

<br>

## Tehtävä 4.9 | Onton pyramidin teko

### Tehtävänanto

- Tee konsoliin pyramiidi `*` merkeistä
- Tehtävässä `saa käyttää vaan yhtä console.log()` lausetta
- Pyramiidin `koko` määritetään `oliolla`
  - `Olio` kertoo pyramiidin `pohjan leveyden`
  - Leveys `pyöristetään alaspäin`, esim `4 leveys olis 3`
- Pyramiidi tulee olla `ontto sisältä`

<br>

### 4 Esimerkki tulosta

```js
> 15
       *
      * *
     *   *
    *     *
   *       *
  *         *
 *           *
***************

> 4
 *
***

> 6
  *
 * *
*****

> 11
     *
    * *
   *   *
  *     *
 *       *
***********
```

<details>
<summary>Vastaus</summary>

```js
const leveys = 10;
let pyramiidi = "";
let valit = leveys / 2;
if(leveys % 2 == 0) valit = (leveys - 1) / 2;

for(let i = 1; i <= leveys; i += 2) {
  if(i > 2 && i + 1 < leveys) {
    pyramiidi += " ".repeat(valit--) + "*" + " ".repeat(i - 2) + "*" + "\n";
  } else pyramiidi += " ".repeat(valit--) + "*".repeat(i) + "\n";
} if(leveys > 0) console.log(pyramiidi);
```

</details>

---

<br>

## Tehtävä 5.0 | Opetus materiaalia `.indexOf()`, `.toUpperCase()`, `.toLowerCase()` ja `pyöristys` operaattoreista

### Selitykset

- `.indexOf()` palauttaa numero `indexin` josta tietty `merkkijono löytyi` ekana `vasemmalta oikealle`
  - Jos merkkijonoa `ei löydy` palauttaa se `-1`
- `.toUpperCase()` muuttaa tekstissä jokaisen kirjaimen `isoksi` kirjaimeksi
- `.toLowerCase()` muuttaa tekstissä jokaisen kirjaimen `pieneksi` kirjaimeksi
- `break` lopettaa `for` tai `while` loopin
  - `break` käytetään esim, jos halutaan loopata kunnes tietty asia tapahtuu, jolloin loop voidan lopettaa
- `continue` lopettaa kyseisen `kierroksen loopissa`
  - Jos laitat heti loopin koodin alkuun `continue`, se ei suorita `loppuja koodeja`
  - `continue` laittaa loopin seuraavalle loopille, ja `for` loopissa suorittaa `3 vaiheen`
- `Math.ceil()` pyötistää desimaaliluvut `ylös` päin
  - `Math.ceil(0.9)`, tulisi pyöristymään `1`
  - `Math.ceil(0.0001)`, tulisi pyöristymään `1`
  - `Math.ceil(0)`, pyöristyy `0`
- `Math.floor()` pyöristää `alaspäin`
  - `Math.floor(0.999)` pyöristyy `0`
  - `Math.floor(0.2)` pyöristyy `0`
  - `Math.floor(1.2)` pyöristyy `1`
- `Math.round()` pyöristää luvun `oikeaoppisesti`, eli `alle .5 alas`, ja` .5 tai enemmän ylös`
  - `Math.round(5.5)` pyöristyy `6`
  - `Math.round(5.49999)` pyöristyy `5`
  - `Math.round(5.8)` pyöristyy `6`

### Opetus materiaali

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

<br>

### Odotettu lopputulos

```js
6
11
-1
KAIKKI ON ISOLLA
kaikki on pienellä
Aloittaa 0
Aloittaa 1
	Lopettaa 1
Aloittaa 2
Aloittaa 3
	Lopettaa 3
Aloittaa 4
Aloittaa 5
	Lopettaa 5
Aloittaa 6
Aloittaa 7
while loop on toinen loop, joka ei vaadi kun vaan yhden ehdon 10
while loop on toinen loop, joka ei vaadi kun vaan yhden ehdon 15
while loop on toinen loop, joka ei vaadi kun vaan yhden ehdon 20
while loop on toinen loop, joka ei vaadi kun vaan yhden ehdon 25
9 4
8 3
9 3 8
```


---

<br>


## Tehtävä 5.1 | Tuplakirjainten löytäminen

### Tehtävänanto

- Tallenna etsittävä `teksti olioon`
- Sovellus etsii `onko` tekstissä yhtään `kirjainta kaksi kertaa`
  - `Ensimmäinen` kirjain jota löytyy `2 kertaa kirjoitetaan konsoliin`
  - Jos samoja kirjaimia ei tekstissä `ole yli 1`, `sanotaan siitä konsoliin`

<br>

### Esimerkki tuloksia

```js
ensimmäinen tuplakirjain tekstissä "koiran ruoka on lopussa" on "r"

tekstissä "kirja" ei ollut yhtään tuplakirjainta

tekstissä "Aa" ei ollut yhtään tuplakirjainta

ensimmäinen tuplakirjain tekstissä "erkin omena" on "e"

ensimmäinen tuplakirjain tekstissä "kissa kehrää" on "s"

ensimmäinen tuplakirjain tekstissä "A B C D" on " "
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
let tarkistetutKirjaimet = "";
let tuplakirjain = "";

for(const kirjain of teksti) {
  if(tarkistetutKirjaimet.indexOf(kirjain) !== -1) {
    tuplakirjain = kirjain;
    break;
  } else tarkistetutKirjaimet += kirjain;
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

## Tehtävä 5.2 | Palindromin tunnistus

### Tehtävänanto

- Tee sovellus joka tunnistaa `palindromin`
  - `Palindromi` on `teksti/numero/merkki jono`, joka on `taka ja etuperin sama`
  - Esim `saippuakauppias`
  - Esim `5005`
- Sovellus `ei välitä` onko `kirjaimet isolla vai pienellä`

<br>

### Esimerkki tuloksia

```js
teksti "saippuakauppias" on palindromi

teksti "teksti" on takaperin "itsket", se ei ole palindromi

teksti "12321" on palindromi

teksti "loL" on palindromi
```

<details>
<summary>Vinkki 1</summary>

- Voit käyttää `toLowerCase()` functiota
- Nytten testi ei välitä kirjain koko erosta

```js
console.log("TÄMÄ ON ISO".toLowerCase());
```

</details>

<details>
<summary>Vastaus</summary>

```js
const teksti = "saippuakauppias";
let takaperin = "";

for(const kirjain of teksti) {
  takaperin = kirjain + takaperin;
}

if(teksti.toLowerCase() == takaperin.toLowerCase()) {
  console.log(`teksti "${teksti}" on palindromi`);
} else {
  console.log(`teksti "${teksti}" on takaperin "${takaperin}", se ei ole palindromi`);
}
```

</details>

---

<br>

## Tehtävä 5.3 | Isot alkukirjaimet

### Tehtävänanto

- Tallenna teksti `olioon`, ja muuta siitä jokainen `alkukirjain isoksi`
- Jos tekstissä on jo `isoja kirjaimia` tulee ne `muuttaa pieneksi`
- Jokainen kirjain `välin jälkeen` tulee olla `isolla`
- Myös `ensimmäinen` kirjain tekstissä tulisi olla `isolla`

<br>

### Esimerkki tuloksia

```js
> "olen teksti joSsa on isOJa kirjaimia"
Olen Teksti Jossa On Isoja Kirjaimia

> "KAIKKI ON ISOLLA      MUHAHAHAH"
Kaikki On Isolla      Muhahahah

> "yksipitkäsana"
Yksipitkäsana
```

<details>
<summary>Vastaus</summary>

```js
const teksti = "olen teksti joSsa on isOJa kirjaimia";
let uusiTeksti = "";

for(let i = 0; i < teksti.length; i++) {
  if(teksti[i - 1] == " " || i == 0) uusiTeksti += teksti[i].toUpperCase();
  else uusiTeksti += teksti[i].toLowerCase();
}

console.log(uusiTeksti);
```

</details>

---

<br>

## Tehtävä 6.0 | `Taulut`, `objectit` ja `random` numerot

### Selitykset

- `Taulut` ovat koodaamisessa hyvin `tärkeä` tapa `säilöä` ja `käyttää dataa`
  - On `pari` eri tapaa `tehdä tauluja`, mutta nytten käydään `objectit` ja `index taulut`
  - `index taulu` tehdään `[]` `kulmasulkeilla` ja siitä voi nimensä mukaan `hakea dataa` `index numerolla`
    - `Numerot alkaa 0`, ja voit `.length` komennolla, nähdä miten paljon `dataa taulussa on`
      - Voit `hakea dataa` näin `taulu[0]` nytten tuo palauttaisi `0` indexin `tiedot`
      - Jos `haet` dataa numerolla `jota ei ole`, palauttaa se `undefined`
      - Voit `muuttaa dataa` laittamalla `taulu[0] = "uusi arvo"` jolloin `edellinen arvo` muuttuu `uudeksi`
        - Vaikka `indexissä` ei olisi ollut tietoa, siihen tulee `uusi tieto`
        - Voit laittaa tietoa `indexiin`, joka on paljon pidemmällä kun taulu on
  - `Objecti` on taulu, josta haetaan `avain` sanalla eikä `index numerolla`
  - Voit laittaa `avain` sanaksi toki `index numeron`, jos haluat
  - `Objectin` voit luoda `{}` `aalkosulkeilla`
    - Sulkeitten sisälle tulee ensin `avain sana`, sitten `:` ja `arvo`
    - Jos haet `avaimella jota ei ole`, palauttaa se `undefined`
  - `Tauluihin` ja `objecteihin` voi tallentaa `mitä arvoja vaan`
- `.split("")` muuttaa `tekstin` `tauluksi`
  - Jos et määritä `merkkiä` `splitin` sisälle, se ajaa `jokaisen` merkin tekstissä `omaksi taulun indexiksi`
  - Jos määrität `merkin`, se jakaa kyseisen merken kohdalla tiedon kahteen `taulun soluun`
    - Esim `"eeeteetetee".split("t")` tulisi `["eee", "ee", "e", "ee"]`, huomaa että `"t"` kirjaimet on `poistettu`
- `.join("")` liittää taulun `yhteen tekstiksi`
  - Jos laitat `merkin` `join("")` lauseen `sisälle`, se liittää taulun `datan yhteen sillä merkillä`
  - Muuten kaikki `data` menee vaan `yhteen normaalisti`
- Voit yhdistää `.split("")` ja `.join("")` lauseen ja `korvata` tiettyjä kirjaimia
  - Esim `"etana".split("a").join("r")`, muutta jokaisen `"a"` kirjaimen `"r"` kirjaimeksi
- `Math.random()` palauttaa numeron joka on `0 - 0.999999...` välillä

### Opetus materiaali

```js
const isotaulu = {
  "nimiA": 5,
  "nimiB": "arvo", // Arvona voi olla mikä vaan, vaikka numero, taulu, objecti tai teksti
  "nimiC": {
    "nimiA": 100
  }
}

console.log(isotaulu); // Tulostaa koko objectin
console.log(isotaulu.nimiA); // Hakee objectista nimiA avain sanan
console.log(isotaulu["nimiB"]); // Voit myös käyttää kulma sulkeita
console.log(isotaulu.nimiC);
console.log(isotaulu.tuntematon) // Tätä nimeä ei löydy, joten palauttaa "undefined"
console.log(isotaulu.nimiC.nimiA)

const indexTaulu = [ // Voit tehdä index taulun, josta haetaan vaan index numerolla
  "abcd", 14234, "5/5 arvo",
  { "nimiA": "arvo" },
  [ 10, 20, 30 ]
];

console.log(indexTaulu[0]);
console.log(indexTaulu[2]);
console.log(indexTaulu[3]);
  console.log(indexTaulu[3].nimiA);
console.log(indexTaulu[4]);
  console.log(indexTaulu[4][1]);
console.log(indexTaulu[75]);

console.log(indexTaulu.indexOf(14234)) // Voit käyttää index of, myös index tauluihin

indexTaulu.push("uusi data"); // Voit lisätä push komennolla uutta dataa tauluun
console.log(indexTaulu[5]);

indexTaulu[1] = "muutettu data"; // Voit myös muuttaa taulun dataa näin
console.log(indexTaulu[1])

console.log("tämä on teksti".split("")) // Voit myös muuttaa "split" komennolla tekstistä taulun
console.log("aaaiaaaiaiaaa".split("i")) // Nytten se jakaa sen tauluihin aina "i" kohdalla

console.log(["a", "b", "c"].join("")) // Voit myös yhdistää taulun tekstiksi
console.log("kello".split("ll").join("45")) // Voit myös korvata näin tiettyjä kirjaimia

console.log(Math.floor(Math.random() * 10)) // Antaa random numeron 0 - 9 välillä
console.log(Math.ceil(Math.random() * 30)) // Antaa random numeron 1 - 30 välillä
console.log(Math.round(Math.random() * 40)) // Antaa random numeron 0 - 40 välillä
```

<br>

### Odotettu lopputulos

```js
► {nimiA: 5, nimiB: "arvo", nimiC: {…}}
5
arvo
► {nimiA: 100}
undefined
100
abcd
5/5 arvo
► {nimiA: "arvo"}
arvo
► (3) [10, 20, 30]
20
undefined
1
uusi data
muutettu data
► (14) ["t", "ä", "m", "ä", " ", "o", "n", " ", "t", "e", "k", "s", "t", "i"]
► (4) ["aaa", "aaa", "a", "aaa"]
abc
ke45o
2
9
30
```