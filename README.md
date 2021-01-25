# JavaScript ympäristön asettaminen
**JavaScript** on koodikieli joka kulkee käsi kädessä kahden muun koodikielen kanssa 
<span style = "color: #ffb76b">**html**</span> ja 
<span style = "color: #6bbaff">**css**</span>, mutta aluksi opetan 
<span style = "color: #eb3434">**JavaScriptiä**</span>


<span style = "color: #ffb76b">**html**</span> on koodikioli, missä tullaan suunnittelemaan käyttöliittymää ja tulee olemaan se ikkuna missä näet visuaalisesti kaiken, toisin sanottuna <span style = "color: #ffb76b">**html**</span> on nettisivu. Jos käyt googlessa, youtubessa tai muualla netissä se mitä näet on <span style = "color: #ffb76b">**html**</span> netti sivu.

<span style = "color: #6bbaff">**css**</span> on tyylittely kieli, jolla päätetään miten sivua tyylitellään ja minkä kokoisia vaikka ikkunat ovat, minkä värisiä otsikot on, missä kaikki sijaitsee sivulla ja muuta. Ilman <span style = "color: #6bbaff">**css**</span> nettisivut näyttävät yleensä hyvin mustavalkoiselta ja on tylsiä elottomia sivuja jotka eivät näytä visuaalisesti parhaimmalta. Esim tältä näyttää youtube ilman <span style = "color: #6bbaff">**css**</span>:  
<img src = "https://i.imgur.com/1oSbAU9.png" height = "200px">

<span style = "color: #eb3434">**JavaScript**</span> on vastuussa kaikesta logiikasta mitä tapahtuu nettisivulla, kun esim lajittelet taulua, hae musiikkia nimellä, painat nappia joka avaa jotain, se kaikki on tehty <span style = "color: #eb3434">**javascriptin**</span> avulla. Ilman <span style = "color: #eb3434">**javascriptiä**</span> nettisivut näyttäisivät hienoilta, mutta niissä ei olisi juuri mitään toimintaa, tai tekemistä.

<hr>

## Näin asetat oppimisympäristön missä koodata.
* Ensiksi luo johonkin kansio missä haluat aloittaa koodaamaan
* Sitten luo tiedosto kansioon nimeltä <span style = "color: #ffb76b">**index.html**</span>
  * Kirjoita tiedoston sisälle tämä: 
  ```html
  <script src = "code.js"></script>
  ```
* Sen jälkeen lisää kansioon toinen tiedosto nimeltä <span style = "color: #eb3434">**code.js**</span>
  * Tämä on se tiedosto jossa koodaaminen tullaan tekemään ja <span style = "color: #ffb76b">**index.html**</span> on se mistä sen voi avata
* Aloita avaamalla <span style = "color: #ffb76b">**index.html**</span> tiedosto selaimeen. Voit avata **Chromella, Firefoxilla, Edgellä** jne, millä vaan haluut
* Jos painat **F12** tai **ctrl** + **shift** + **i** saat auki konsoolin. Tänä näyttää erillaiselta riippuen mitä selainta käytät, mutta siitä pitäisi päästä konsooli näkymään *(saattaa olla jo valmiina siinä)*
  <img src = "https://i.imgur.com/rBTE6Xp.png">
* Tämä konsooli tulee olemaan se mistä näet sinut suoritetun koodin alussa koska emme tee mitään visuaalista.

# JavaScript perusteet

Aloita kirjoittamalla <span style = "color: #eb3434">**code.js**</span> tiedostoon:
```js 
console.log("moro kaikki");
```
Ulostulo: 
```js
moro kaikki
```
Jos avaat selaimen, missä on auki <span style = "color: #ffb76b">**index.html**</span> ja katsot konsoliin näet siellä tekstiä. Aina kun muutat <span style = "color: #eb3434">**code.js**</span> tiedostoa pitää sinun päivittää selain ikkuna joko **F5**, **ctrl** + **r**, **ctrl** + **shift** + **r**, tai sitten painamalla `lataa sivu uudelleen` nappia, jotta uusi teksti tulisi näkyviin.

<hr>

Voit luoda objektin johon voit tallentaa tiedon ja sitten kertoa sen konsooliin:
```js
let teksti = "moro kaikki";
console.log("moro kaikki");
console.log("###########");
console.log(teksti);
```
Ulostulo: 

```js
moro kaikki
###########
moro kaikki
```

<hr>

Esimerkkejä mitä voit tehdä konsoolissa

```js
console.log(1 + 1);
console.log(5 + 6);
console.log(4 / 2);
console.log(2 * 6);
console.log(15 - 10);
console.log("##################");

let numero1 = 50;
let numero2 = 150;
console.log(numero1 + numero2);
```
Ulostulo: 
```js
2
11
2
12
5
##################
200
```

<hr>
Tässä eri tapoja yhdistellä tekstiä ja objekteja. Ei ole mitään väärää tapaa, mutta itse olen aika tottunut käyttämään tota alinta vaihtoehtoa.

```js
let nimi = "Pekka";
let sukunimi = "Puuro";
let ikä = 25;

console.log(nimi, sukunimi, 'on', ikä, 'vuotta vanha');
console.log(nimi, sukunimi, "on", ikä, "vuotta vanha");
console.log(nimi + sukunimi + "on" + ikä + "vuotta vanha");
console.log(`${nimi} ${sukunimi} on ${ikä} vuotta vanha`);
```

```js
Pekka Puuro on 25 vuotta vanha
6 PekkaPuuroon25vuotta vanha
7 Pekka Puuro on 25 vuotta vanha
```

<hr>

```js
// okei käydään perusteita läpi.
// Jos laitat kaksi sivu viivaa, se tekee koodiin kommentin, jota koodi ei suorita, joten näin voit
// seolittää mitä koodi tekee, jotta se olisi selkeämpää

console.log(50); // Yleensä javascriptissä laitetaan ; jokaisen rivin loppuun, mutta se ei hajoa yleensä jos sen jättää laittamalla
console.log(50) // Toimii ilman ;

console.log("########################################")

let tuote = "Juusto"
console.log(tuote)
tuote = "Maito" // Voit vaihtaa jo luodun objektin arvoa näin. Älä laita let alkuun, tai tulee Error
console.log(tuote)

console.log("########################################")

let nimi = "Pekka" // On myös tapauksia missä on pakko laittaa ; tai koodi hajoaa, joten suosittelen vaan laittamaan niitä joka rivin päätteeksi, jos et ole varma tarvitseeko semmoista vai ei
(() => {
  console.log("moi");
})();
```

```js
50
50
########################################
Juusto
Maito
########################################
> Uncaught TypeError: "Pekka" is not a function
    at code.js:18
```

<hr>

```js
console.log("Eka rivi\nToka rivi\nKolmas rivi") // \n vaihtaa riviä
console.log("moi \t olen \t iso \t väli") // \t heittää tabulaattorin
console.log("Eka rivi\n\tToka rivi\n\t\tKolmas rivi") // Voit yhdistää näitä

// Voit myös tehdä noin monta riviä
console.log(`
  ##################
  #                #
  #      Text      #
  #                #
  ##################
`)
```

```js
Eka rivi
Toka rivi
Kolmas rivi
moi 	 olen 	 iso 	 väli
Eka rivi
	Toka rivi
		Kolmas rivi
  ##################
  #                #
  #      Text      #
  #                #
  ##################
```


<hr>

```js
let nimi = "Joosef"
console.log(nimi)
console.log(nimi[0]) // Tämä ottaa ensimmäisen kirjaimen
console.log(nimi.length) // Kertoo miten pitkä objekti on

console.log("#".repeat(40)) // toistaa asiaa 40 kertaa
console.log(nimi[nimi.length - 1]) // Ottaa nimi objektin viimeisen kirjaimen. Koska lasku alkaa nollasta, pitää vähentää yksi
console.log(nimi[nimi.length]) // Muutan tulee määrittämätön
```
```js
Joosef
J
6
########################################
f
undefined
```
<hr>

```js
let num1 = 5;
let num2 = 10;

if(num1 < num2) { // jos num1 on pienempi kuin num2 suorittuu if lauseen sisällä olevat komennot
  console.log(num1 + " on pienempi kuin " + num2)
} else { // jos ei tämä suorittuu
  console.log(num1 + " on isompi kuin " + num2)
}
```
```js
5 on pienempi kuin 10
```

# JavaScript Tehtävät
Vastaukset ja vinkit tehtäviin löytyvät alempaa. Vastauksia on monia erillaisia, joten kunhan lopputuloksesi on sama kuin tehtävän annossa, se on kelvollinen tapa.

## JavaScript Tehtävä #1
```js
// Kerro miten paljon on numero1 jaettuna numero2

let numero1 = 40;
let numero2 = 10;

console.log()
```
```js
// Odotettava tulos:
40 jaettuna 10 on 4
```
## JavaScript Tehtävä #1 vinkit
```js
console.log(10 / 5) // Näin käytät jakolaskua

let numero = 5;
console.log("tiesitkö että " + numero / 2 + " on numero") // Näin sekoitat objekteja tekstiin
```
## JavaScript Tehtävä #1 vastaus

```js
// Kerro miten paljon on numero1 jaettuna numero2

let numero1 = 40;
let numero2 = 10;

console.log(`${numero1} jaettuna ${numero2} on ${numero1 / numero2}`);
```

<hr>

## JavaScript Tehtävä #2

```js
// Anna tekstin ensimmäinen ja viimeinen kirjain
// kerro onko teksti pidempi kuin 7 merkkiä

let teksti = "Mansikkakakku"
```
```js
// Odotettava tulos pitkä sana:
Tekstin "Mansikkakakku" ensimmäinen kirjain on "M"
Tekstin "Mansikkakakku" viimeinen kirjain on "u"
"Mansikkakakku" on pidempi kuin 7 kirjainta
```
```js
// Odotettava tulos lyhyt sana:
Tekstin "kakku" ensimmäinen kirjain on "k"
Tekstin "kakku" viimeinen kirjain on "u"
"kakku" ei ole pidempi kuin 7 kirjainta
```





## JavaScript Tehtävä #2 vinkit
```js
console.log("tekstiä"[3]) // Ottaa neljännen kirjaimen, koska 0 on eka
console.log("tekstiä"[0])

let num1 = 3
let num2 = 5
if(num1 < num2) {
  console.log("Tosi")
} else { // jos ei tule toteen suorittuu tämä
  console.log("Epätosi")
}
```

## JavaScript Tehtävä #2 vastaus
```js
// Anna tekstin ensimmäinen ja viimeinen kirjain
// kerro onko teksti pidempi kuin 7 merkkiä

let teksti = "Mansikkakakku"

console.log(`Tekstin "${teksti}" ensimmäinen kirjain on "${teksti[0]}"`)
console.log(`Tekstin "${teksti}" viimeinen kirjain on "${teksti[teksti.length - 1]}"`)
if(teksti.length > 7) console.log(`"${teksti}" on pidempi kuin 7 kirjainta`);
else console.log(`"${teksti}" ei ole pidempi kuin 7 kirjainta`);
```
