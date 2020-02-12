# Palvelun vaatimukset listana

[![](http://img.youtube.com/vi/rp3DkiZ-Mkk/0.jpg)](http://www.youtube.com/watch?v=rp3DkiZ-Mkk "")


Tämä malli on varsin käyttökelpoinen, jos lista ei veny kovin pitkäksi. Sama lista voidaan aika kätevästi tehdä Excelillä, mutta se johtaa varsin pian dokumentoinnin monimutkaisuuteen.
Kun käytetään yhtä ympäristöä keräämään oleellinen tieto on niiden linkittäminen helpompaa ja tieto pysyy ajantasalla paremmin.


# Liiketoiminta/Asiakkaat/Rajoitteet

**Asiakasvaatimukset**

| VaatimusID | Tyyppi | Kuvaus | 							
|:-:|:-:|:-:|
| CUSTOMER-REQ-0001 | Customer Requirement | Käyttäjänä haluan oven avauksen tapahtuvan vaivattomasti | 
| CUSTOMER-REQ-0002 | Customer Requirement | Käyttäjänä haluan ettei minun tarvitse päivittää ovenavaus-oikeuksia jatkuvasti |
| CUSTOMER-REQ-0003 | Customer Requirement | Käyttäjänä haluan että järjestelmän käyttö on helpompaa kuin tavallisen avaimen käyttö |
| CUSTOMER-REQ-0004 | Customer Requirement | Käyttäjänä haluan että voin lisätä avainoikeuksia niitä tarvittaessa
| CUSTOMER-REQ-0005 | Customer Requirement | Käyttäjänä haluan että voin tarkastella oikeuksiani
| CUSTOMER-REQ-0006 | Customer Requirement | Ylläpitäjänä haluan että voin hallinnoida oikeuksia käyttöliittymästä |
| CUSTOMER-REQ-0007 | Customer Requirement | Ylläpitäjänä haluan että oikeuksien hallinnointi onnistuu suurelle käyttäjäryhmälle |
| CUSTOMER-REQ-0008 | Customer Requirement | Ylläpitäjänä haluan että voin muokata ja lisätä käyttäjiä ja avaimia |
| CUSTOMER-REQ-0009 | Customer Requirement | Ylläpitäjänä haluan että voin liittää avaimia järjestelmään |


**Liiketoiminnan vaatimukset**

| VaatimusID | Tyyppi | Kuvaus | 
|:-:|:-:|:-:|
| BUSINESS-REQ-0001 | Business Requirement | Palvelun käytön tulee nopeuttaa avainten käsittellyyn kuluvaa aikaa | 
| BUSINESS-REQ-0002 | Business Requirement | Palvelun käytössä tulee huomioida käyttäjän teknisten taitojen vähäisyys |
| BUSINESS-REQ-0003 | Business Requirement | Palvelun tulee olla helposti hallinnoitavissa |
| BUSINESS-REQ-0004 | Business Requirement | Palvelun tulee olla skaalautuva jatkokehitystä varten |

**Rajoitukset / Standardit**

| Id | Vaatimuksen kuvaus | kategoria | Vastuullinen |
|:-:|:-:|:-:|:-:|
| CONSTRAINT-REQ-S00000 | Constrain | Henkilötietojen käsittely tulee tapahtua GDPR-säädösten mukaisesti  | [Käyttäjänhallinta ft2](ominaisuudet/ominaisuus-kayttajanhallinta.md) |
| CONSTRAINT-REQ-S00001 | Constrain | Asiakkailta on saatava suostumus lukon asentamiseen sekä henkilötietojen käsittelyyn palvelussa | [Avaintenhallinta](ominaisuudet/ominaisuus-avaintenhallinta.md)|



# Järjestelmätason /Ohjelmiston vaatimukset

**SYSTEM REQUIREMENTS**

| VaatimusID | Tyyppi | Kuvaus | Ominaisuus johon vaikuttaa |								
|:-:|:-:|:-:|:-:|
|System-HW-REQ-0001| System Technical Requirement | Palveluun tarvitaan palvelimelle yhteydessä oleva laite | Palvelun saatavuus | 
| SYSTEM-HW-REQ-0002 | System Technical Requirement | Palvelimen fyysinen sijainti on kotimaassa (FI) | Tietoturva |
| SYSTEM-HW-REQ-0003 | System Technical Requirement | Tietojen tulee olla salattuja | Tietoturva |
| SYSTEM-HW-REQ-0004 | System Technical Requirement | Tietoliikennenopeuden tulee olla vähimmiltään 25 MB/S | Tietoliikenne |
| SYSTEM-HW-REQ-0005 | System Technical Requirement | Tietokannat tulevat olla saavutettavissa backup-palvelimelta ongelmatilanteissa | Palvelun saatavuus |
| SYSTEM-HW-REQ-0006 | System Technical Requirement | Ovenavaus tulee onnistua sähkökatkon aikana | Turvallisuus |

**Tekniset vaatimukset**

Tekniset vaatimukset esitetään yleensä erillään ohjelmiston vaatimuksista. Ne liittyvät oleellisen osana
järjestelmävaatimuksiin. Teknisiä vaatimuksia voivat olla esim:

* Suoritusympäristö (Linux, Windows, Pilvi etc)
* Muisti (4GB, 16GB ?)
* Suoritin (Intel/AMD/ARM ?)
* Tietokanta (MySQL, DynamoDB, Orient etc?)
* Ajoalustan ratkaisut JAVA VM, Docker Container ?
 



### Toiminnalliset vaatimukset**

| VaatimusID | Tyyppi | Kuvaus | Ominaisuus johon vaikuttaa |								
|:-:|:-:|:-:|:-:|
| FUNCTIONAL-REQ-C0001 | Functional Requirement | Käyttäjänä (Asiakas, työntekijä, huoltopalvelu, turvapalvelu) saan oven auki tunnisteella/avaimella | [ft1 - Oven aukaisu ](ominaisuudet/) |
| FUNCTIONAL-REQ-C0002 | Functional Requirement | Käyttäjänä (Asiakas) jos oveni jää auki, saan äänimerkin aukijäämisestä | [ft2 - Oven aukijääminen]() |
| FUNCTIONAL-REQ-C0003 | Functional Requirement | Ylläpitäjänä voin käyttöliitymän avulla hallinnoida avaimia, oikeuksia ja käyttäjiä | [ft3 - Ylläpitäjä Käyttöliittymä](ominaisuudet/)  |
| FUNCTIONAL-REQ-C0004 | Functional Requirement | Ylläpitäjänä voin lisätä avaimen järjestelmään | [ft4 - Avainten lisäys](ominaisuudet/ominaisuus-avaintenhallinta.md)  |
| FUNCTIONAL-REQ-C0005 | Functional Requirement | Ylläpitäjänä voin muokata avaimen tietoja| [ft5 - Avainten muokkaus](ominaisuudet/ominaisuus-kayttajanhallinta.md)  |
| FUNCTIONAL-REQ-C0006 | Functional Requirement | Ylläpitäjänä voin poistaa vanhentuneita avaimia| [ft6 - Avainten poisto](ominaisuudet/)  |
| FUNCTIONAL-REQ-C0007 | Functional Requirement | Ylläpitäjänä voin lisätä käyttäjän järjestelmään|[ft7 - Käyttäjien lisäys ](ominaisuudet/)  |
| FUNCTIONAL-REQ-C0008 | Functional Requirement | Ylläpitäjänä voin muokata käyttäjiä| [ft8 - Käyttäjien muokkaus ](ominaisuudet/) |
| FUNCTIONAL-REQ-C0009 | Functional Requirement | Ylläpitäjänä voin poistaa käyttäjiä|[ft9 - Käyttäjien poisto ](ominaisuudet/)  |
| FUNCTIONAL-REQ-C0010 | Functional Requirement | Käyttäjänä voin pyytää lisäoikeuksia ylläpidolta tarpeen mukaisesti | [ft10 - Oikeuksien pyyntö](ominaisuudet/) |
| FUNCTIONAL-REQ-C0011 | Functional Requirement | Käyttäjänä voin tarkistaa omat oikeuteni| [ft11 - Omien oikeuksien tarkistus ](ominaisuudet/) | 
| FUNCTIONAL-REQ-C0012 | Functional Requirement | Ylläpitäjän voin seurata avainten käyttöä | [ft13 - Avainten käytön seuranta](ominaisuudet/)  |
| FUNCTIONAL-REQ-C0013 | Functional Requirement | Ylläpitäjänä voin saada hälytyksen oven jäädessa auki liian pitkäksi aikaa|[ft14 - Hälytys mikäli ovi auki pitempään](ominaisuudet/)  |
| FUNCTIONAL-REQ-C0014 | Functional Requirement | Käyttäjänä voin tarkistaa mobiilisovelluksesta oikeuteni |[ft15 - Mobiilisovellus](ominaisuudet/)  |
| FUNCTIONAL-REQ-C0015 | Functional Requirement | Käyttäjänä voin hallinnoida tietojani ja avaimiani käyttöliittymän kautta |[ft16 - Avainkäyttäjän käyttöliittymä ](ominaisuudet/) |



### Ei-Toiminnalliset vaatimukset


**Tietoturva**

| VaatimusID | Tyyppi | Kuvaus | Ominaisuus johon vaikuttaa |								
|:-:|:-:|:-:|:-:|
| SECURITY-REQ-0001 | Non-Functional Security | Salasanassa on käytettävä vähintään MD5-tason salausta, koska standardi XY112 sitä edellyttää | [Kirjautuminen ft1](ft1-ominaisuus.md) |								
| SECURITY-REQ-0002 | Non-Functional Security | Palvelun kirjatuminen tulee tapahtua salatusti||
| SECURITY-REQ-0003 | Non-Functional Security | Avainkoodien tulee olla salattuja ||
| SECURITY-REQ-0004 | Non-Functional Security | Avainkoodit eivät saa linkittyä henkilöön avainta lukiessa||
| SECURITY-REQ-0005 | Non-Functional Security | Avain tulee olla suljettavissa väärinkäyttöä ilmetessä ||
| SECURITY-REQ-0006 | Non-Functional Security | Lukon tulee päivittää sallittujen avainten tiedot viiden minuutin välein ||


**Suorituskyky**

| VaatimusID | Tyyppi | Kuvaus | Ominaisuus johon vaikuttaa |								
|:-:|:-:|:-:|:-:|
| PERFORMANCE-REQ-0000 | Non-Functional Performance | Kirjautuminen on mahdollista yhtäaikaa 100 käyttäjällä (100 request/s) | [Kirjautuminen ft1](ft1-ominaisuus.md) |								
| PERFORMANCE-REQ-0001 | Non-Functional Performance |||
| PERFORMANCE-REQ-0002 | Non-Functional Performance |||
| PERFORMANCE-REQ-0003 | Non-Functional Performance |||
| PERFORMANCE-REQ-0004 | Non-Functional Performance |||
| PERFORMANCE-REQ-0005 | Non-Functional Performance |||


**Käytettävyys**

| VaatimusID | Tyyppi | Kuvaus | Ominaisuus johon vaikuttaa |								
|:-:|:-:|:-:|:-:|
| USABILITY-REQ-0000 | Non-Functional Usability | Käyttöliittymän on toimittava myös ääniohjattuna, koska käyttäjillä saattaa olla näkövammoja |  [Kirjautuminen ft1](ft1-ominaisuus.md) | |	
| USABILITY-REQ-0001 | Non-Functional Usability |||
| USABILITY-REQ-0002 | Non-Functional Usability |||
| USABILITY-REQ-0003 | Non-Functional Usability |||
| USABILITY-REQ-0004 | Non-Functional Usability |||
| USABILITY-REQ-0005 | Non-Functional Usability |||



**Palautuminen**

| VaatimusID | Tyyppi | Kuvaus | Ominaisuus johon vaikuttaa |								
|:-:|:-:|:-:|:-:|
| RECOVERY-REQ-00100 | Non-Functional Recovery | Kirjautumis-palvelun on käynnistyttävä ensimmäisen palvelun ylösajon aikana | [Kirjautuminen ft1](ft1-ominaisuus.md)	 |							
| RECOVERY-REQ-00100 | Non-Functional Recovery |||							


**Testattavuus**

| VaatimusID | Tyyppi | Kuvaus | Ominaisuus johon vaikuttaa |								
|:-:|:-:|:-:|:-:|
| TESTABILITY-REQ-0000 | Non-Functional Testability | Käyttäjärekisteri on kyettävä palauttamaan alkutilaan ennen testien ajoa  | [Kirjautuminen ft1](ft1-ominaisuus.md)	 |	
| TESTABILITY-REQ-0001 | Non-Functional Testability |||	
| TESTABILITY-REQ-0002 | Non-Functional Testability |||	
| TESTABILITY-REQ-0003 | Non-Functional Testability |||	
| TESTABILITY-REQ-0004 | Non-Functional Testability |||	
| TESTABILITY-REQ-0005 | Non-Functional Testability |||	


**Turvallisuus**

| VaatimusID | Tyyppi | Kuvaus | Ominaisuus johon vaikuttaa |								
|:-:|:-:|:-:|:-:|
| SAFETY-REQ-0000 | Non-Functional Safety |  Tähän tuotteesen ei voida osoittaa turvallisuus vaatimuksia  | [Kirjautuminen ft1](ft1-ominaisuus.md)	|	
| SAFETY-REQ-0001 | Non-Functional Safety |||	
| SAFETY-REQ-0002 | Non-Functional Safety |||	
| SAFETY-REQ-0003 | Non-Functional Safety |||	


# Mekaaniikka vaatimukset 

| VaatimusID | Tyyppi | Kuvaus | Ominaisuus johon vaikuttaa |								
|:-:|:-:|:-:|:-:|
| MECHANICAL-REQ-000 | Mechanical Requirement | || 	
| MECHANICAL-REQ-001 | Mechanical Requirement | || 	
| MECHANICAL-REQ-002 | Mechanical Requirement | || 	
| MECHANICAL-REQ-003 | Mechanical Requirement | || 	
| MECHANICAL-REQ-004 | Mechanical Requirement | || 	
| MECHANICAL-REQ-005 | Mechanical Requirement | || 	

