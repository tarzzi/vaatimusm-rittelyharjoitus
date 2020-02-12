# Muokkaa avainta:

## Use Case 


```plantuml
Admin -- (Edit key info)
User-- (Edit key info)
```

* Laatija: Tarmo
* Päiväys 19.1.2020 / Versio 1.0 
* Avaintenhallinta
	
**Käyttäjäroolit**	

1. Ylläpitäjä
2. Käyttäjä

**Esitiedot/ehdot**	

1. Avain on lisätty järjestelmään 
2. Käyttötapausta toimittava henkilö on kirjautuneena järjestelmään

**Käyttötapauksen kuvaus**

1. Käyttäjä painaa muokkaa avainoikeuksia-painiketta
2. Käyttöliittymä näyttää avaimen oikeudet
3. Käyttäjä voi halutessaan lisätä tai poistaa avaimen käyttöoikeuksia
4. Käyttäjä tallentaa tiedot muutosten jälkeen  
5. Käyttöliittymä pyytää varmistusta tallentamiseen
6. Järjestelmä päivittyy

**Poikkeukset**
 
* Käyttäjä ei tallennakkaan avaimen tietoja -- Ei muutoksia avaimen tietoihin


	
**Lopputulos**	

* Käyttäjä näkee ja voi muokata avaimen oikeuksia sekä tallentaa ne.

**Käyttötiheys** 

* Käytetään aina avaimen tietoihin tulleiden muutosten tarpeen mukaisesti.

**Muuta**	



**Lähteet**

Tämä wiki-dokumentin runko pohjautuu [Julkisenhallinnon suosituksiin](http://www.jhs-suositukset.fi/web/guest/jhs/recommendations/173)

Kiitokset alkuperäisen tekijöille!

