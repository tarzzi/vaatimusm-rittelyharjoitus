# Muokkaa käyttäjää:

## Use Case 


```plantuml
Admin -- (Edit user info)
User-- (Edit user info)
```

* Laatija: Tarmo
* Päiväys 19.1.2020 / Versio 1.0 
* Käyttäjänhallinta
	
**Käyttäjäroolit**	

1. Ylläpitäjä
2. Käyttäjä

**Esitiedot/ehdot**	

1. Käyttäjä on lisätty järjestelmään 
2. Käyttötapausta toimittava henkilö on kirjautuneena järjestelmään

**Käyttötapauksen kuvaus**

1. Käyttäjä painaa muokkaa käyttäjätietoja-painiketta
2. Käyttöliittymä näyttää käyttäjän tiedot
3. Käyttäjä voi halutessaan muokata tietoja/tietojaan
4. Käyttäjä tallentaa tiedot muutosten jälkeen  
5. Käyttöliittymä pyytää varmistusta tallentamiseen
6. Järjestelmä päivittyy

**Poikkeukset**
 
* Käyttäjä ei tallennakkaan tietoja -- Ei muutoksia tietoihin


	
**Lopputulos**	

* Käyttäjä näkee ja voi muokata käyttäjän tietoja sekä tallentaa ne.

**Käyttötiheys** 

* Käytetään aina käyttäjän tietoihin tulleiden muutosten tarpeen mukaisesti.

**Muuta**	



**Lähteet**

Tämä wiki-dokumentin runko pohjautuu [Julkisenhallinnon suosituksiin](http://www.jhs-suositukset.fi/web/guest/jhs/recommendations/173)

Kiitokset alkuperäisen tekijöille!

