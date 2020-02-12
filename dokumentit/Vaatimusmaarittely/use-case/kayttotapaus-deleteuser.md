# Poista käyttäjä:
## Use Case 


```plantuml
Admin -- (Delete user)
```

__Tsekkaa video ja poista linkki, jos homma selvä__
* Laatija: Tarmo
* Päiväys 19.1.2020 / Versio 1.0 
* Käyttäjänhallinta
	
**Käyttäjäroolit**	

1. Ylläpitäjä

**Esitiedot/ehdot**	

1. Ylläpitäjällä on käyttäjän tiedot 
2. Ylläpitäjällä syy käyttäjän poistoon

**Käyttötapauksen kuvaus**

1. Ylläpitäjä kirjautuu käyttöliittymään
2. Ylläpitäjä painaa poista-käyttäjä painiketta
3. Ylläpitäjä valitsee poistettavan käyttäjän listalta
4. Ylläpitäjä vahvistaa poiston olevan oikea
5. Käyttäjä poistetaan
6. Järjestelmä päivittyy

**Poikkeukset**
 
* Ylläpitäjä poistaa väärän käyttäjän -- peruuttaa poiston	

	
**Lopputulos**	

* Käyttäjä on poistettu järjestelmästä

**Käyttötiheys** 

* Aina kun on tarve poistaa käyttäjä järjestelmästä.

**Muuta**	


**Lähteet**

Tämä wiki-dokumentin runko pohjautuu [Julkisenhallinnon suosituksiin](http://www.jhs-suositukset.fi/web/guest/jhs/recommendations/173)

Kiitokset alkuperäisen tekijöille!

