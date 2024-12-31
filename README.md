# HarryPotter
Frontend perusteet 2024 lopputyö

## Yleistiedot
Tekijä: Jenni Hapuli
Lopputyön nimi: Harry Potter -hahmohaku

## Idea lyhyesti:
Sovellus on tarkoitettu kaikille Harry Potter -elokuvien hahmoista
kiinnostuneille. Sovelluksella voi hakea hahmoja nimen, sukupuolen ja Tylypahkan koulun tupien perusteella. Sovellus näyttää hahmon kuvan, nimen ja tuvan korttina.

## Toiminnallisuus:
### Hahmodatan lataaminen: 
Kun sovellus käynnistetään, se hakee heti kaikki hahmot API:sta ja näyttää ne korttilistana.

### Hahmojen haku ja suodatus: 
Käyttäjä voi etsiä hahmoja nimellä hakukentän avulla. Syötteeseen riittää jo muutama nimen ensimmäinen kirjain,  eikä kirjainkoolla ole väliä. Hakukenttä toimii ilman “hakupainiketta”.
Hakutulosta voi suodattaa sukupuolen mukaan (nainen, mies tai kaikki).
Hahmoja voi etsiä myös Tylypahkaan kuuluvien tupien perusteella (Gryffindor, Hufflepuff, Ravenclaw, Slytherin tai kaikki). Haku ja suodatus päivittävät automaattisesti näytettävät hahmot.

Testaa: Esimerkiksi syöttämällä nimen "Weasley", sovellus hakee välittömästi kaikki Weasleyn suvun jäsenet. Valitsemalla "Naiset" tulos näyttää neljä Weasleyn suvun naista. Jos hakuehtoon lisää vielä tuvan "Gryffindor", niin hakutuloksesta suodattuu pois Victoire Weasley, joka ei kuulu mihinkään tupaan.

### Hahmojen esittäminen: 
Suodatetut hahmot näytetään kortteina, jotka sisältävät hahmon kuvan, nimen ja tuvan (tai ilmoituksen, jos hahmo ei kuulu mihinkään tupaan, eli kyseessä on Tylypahkan kouluun kuulumaton hahmo).

Sovellus sisältää latausanimaation, joka näkyy, kun dataa haetaan.


## Harjoitustyön tekeminen
Harry Potter API:
https://www.freepublicapis.com/harry-potter-api
https://hp-api.onrender.com/api/characters

## Tekoälyn hyödyntäminen lopputyössä:
Käytin ChatGpt:tä hakutoimintoihin liittyvien funktioiden luomisessa siinä vaiheessa, kun en saanut yhdistettyä itse input-kenttään annettua syötettä sekä radio-buttoneilla annettuja hakuehtoja toisiinsa. Koodi ei toiminut oikein, jos valitsi ensin esim. Sukupuolen ja sen jälkeen vasta kirjoitti hahmon nimen. Syötin ChatGpt:lle viallisen koodini, ja se antoi korjausehdotuksia ja koodipätkiä, joilla sain sovelluksen toimimaan. ChatGpt:n kirjoittamat koodit on merkitty selkeästi koodiin.

Tekoälyn osuus lopputyöstä on valitettavan suuri, sillä hakutoiminto on sovelluksen ydin. Lisäksi käytin tekoälyä monen CSS-määreen selittämiseen, sillä en osaa niistä kovinkaan montaa vielä ulkoa. Käytin ChatGpt:tä apuna myös ideoinnissa. Esim. latausanimaation tekeminen omaksi komponentikseen oli sen idea.
Tekoäly auttoi siis noin 30% koodista.


