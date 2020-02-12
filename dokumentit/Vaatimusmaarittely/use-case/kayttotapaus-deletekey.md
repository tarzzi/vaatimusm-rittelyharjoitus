# Poista avain:
## Use Case 


```plantuml
Admin -- (Delete key)
```

__Tsekkaa video ja poista linkki, jos homma selvä__
* Laatija: Tarmo
* Päiväys 19.1.2020 / Versio 1.0 
* Avaintenhallinta
	
**Käyttäjäroolit**	

1. Ylläpitäjä

**Esitiedot/ehdot**	

1. Ylläpitäjällä on avaimen tiedot 
2. Ylläpitäjällä on syy avaimen poistoon

**Käyttötapauksen kuvaus**

1. Ylläpitäjä kirjautuu käyttöliittymään
2. Ylläpitäjä painaa poista avain-painiketta
3. Avainlista avautuu
4. Ylläpitäjä valitsee poistettavan avaimen
5. Ylläpitäjä hyväksyy avaimen poiston
6. Järjestelmä päivittyy

**Poikkeukset**
 
* Ylläpitäjä valitsee väärän avaimen poistoon -- peruuttaa avaimen poiston järjestelmästä	

	
**Lopputulos**	

* Avain on poistettu järjestelmästä

**Käyttötiheys** 

* Aina kun on tarve poistaa avain järjestelmästä.

**Muuta**	


**Lähteet**

Tämä wiki-dokumentin runko pohjautuu [Julkisenhallinnon suosituksiin](http://www.jhs-suositukset.fi/web/guest/jhs/recommendations/173)

Kiitokset alkuperäisen tekijöille!

