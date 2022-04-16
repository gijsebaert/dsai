# H0 Introductie

## Leerdoelstellingen

- Beschrijvende statistieken

- Datavisualisatie

- Waarschijnlijkheid

- bivariante analyse

- tijdserie analyse

## cursusinhoud

- inleiding steekproeven
- univariate analyse
- Waarschijnlijkheid, centrale limiet theorie, statische testen
- bivariante analyse: qualitatieve variabelen
- bivariante analyse: qualitatieve vs quantitatieve variabelen
- bivariante analyse: quantitatieve variabelen
- tijdserie analyse

## Datavisualisatie kan leugens bevatten

- datavisualisatie fouten zijn
  - mediakanalen, politici, speciale groepen, louche mensen op FB die objectieve data verkeerd interpreteren of misrepresenteren. Om hun punt over te brengen.

## Waarom DataScience?

- hoeveelheid data is aan het exploderen
- data drijft bedrijfsbeslissingen
- correcte analyse is belangrijk!
- tools en data is meer bereikbaar dan ooit te voren

# H1 Basisbegrippen en steekproefonderzoek

## Basisconcepten en steekproefonderzoek

### Wetenschappelijke methode

gebaseerd op empirisch onderzoek we zijn geintereseerd in:

- exploratie
- descriptie
- voorspelling
- verificatie

### Onderzoeks process

PROBLEEMSTELLING
Wat is de onderzoeksvraag?

EXACTE INFORMATIENODEN
Wat moeten we onderzoeken?

UITVOERING RESEARCH
Enquetes, simulaties, experimenten ...

PROCESS DATA
Statische software

ANALYSEER DATA
Statische methode

FORMULEER CONCLUSIE
Schrijf research rapport

## Variabelen en Waarden

Variabele:
Algemene eigenschap van een object, die het mogelijk maakt objecten te onderscheiden

Waarde:
Specifieke eigenschap, interpretatie voor die variabele

## Meeteenheden

Qualitatieve:
Niet noodzakelijk numeriek
Beperkt aantal waarden

Quantitatieve:
Aantal + meeteenheid
Veel waarden, vaak uniek

Bij Qualitatieve:

Nominaal:
Categorieen
e.g : Gender, race, land, vorm

Ordinaal:
Order, Rank
e.g : Militaire rank, educatie niveau

Bij Quantitatieve:

Interval:
Geen gefixeerd 0 punt, geen proporties
e.g : °C, °F

Ratio:
Absoluut nulpunt, proporties
e.g : afstand (m), energie (J), gewicht (kg)

## Relaties tussen variabelen

variabelen zijn gerelateerd als waarden systematisch veranderen

Onderzoekers zoeken vaak casual relationships

- frustratie lijdt tot agressie
- alcohol lijdt tot verminderde alertheid

oorzaak
onafhankelijke variabele

gevolg
afhankelijke variabele

OPGELET:
een relatie is niet altijd noodzakelijk een casual relationship!

e.g :

- geweldadige videogames zorgen voor geweldadige acties
- vaccins veroorzaken autisme
- verband tussen drinken cola light en obesitas

## Voorbeeld testing

populatie:
collectie van alle objecten, personen die je wilt onderzoeken.

Sample:
een deel van de populatie die je zult onderzoeken.

Definitie van populatie
defineer sample frame
keuze van sample method (budget en tijd)

### Random Sample

elk element van de populatie heeft een gelijke kans om in de sample terecht te komen

### Non-Random Sample

de elementen van de sample zijn niet random geselecteerd. Objecten die makkelijker gecollecteerd kunnen worden hebben een grotere kans van in de steekproef te geraken.

## Mogelijke fouten

accidentieel <> systematisch
steekproeffout <> niet steekproeffout

systematische steekproeffout

- online > mensen zonder internet zijn uitgesloten
- straatafname > alleen wie daar wandelt
- vrijwillige enquete > enkel geintereseerden doen mee

accidentieel niet steekproeffouten

- incorrecte antwoorden aangeduid

systematische niet steekproeffouten

- slechte of niet gecalibreerde meetinstrumenten
- waarde kan beinvloed worden door het feit dat jij meet
- respondanten liegen

# H2 Univariate statistieken

Rekenkundig gemiddelde (x̄):

- som van alle waarden gedeeld door het aantal waarden

Mediaan:

- sorteer alle waarden en neem het middelste nummer

Mode:

- waarde dat het meest voorkomt in de dataset

Range:

- absolute waarde van het verschil tussen de hoogste en laagste waarde

Kwartielen:

- 3 waarden dat de dataset in 4 gelijke delen deelt, Q1, Q2, Q3
- Kwartielen berekenen
  - n is oneven
    - mediaan (Q2) is middelste waarde
    - laat de mediaan weg, Q1 is mediaan eerste helft, Q2 mediaan 2de helft
  - n is even
    - mediaan (Q2) is gemiddelde middelste 2 waarden
    - Q1 is mediaan van eerste helft, Q2 mediaan van 2de helft

Variantie (𝑠2 of 𝜎2):

- kwadratisch verschil tussen de waarden van een dataset en het rekenkundig gemiddelde

standaardafwijking (𝑠 of 𝜎):

- de vierkantswortel van de variantie

Spreiding en centrale tendens
![Spreiding eb centrale tendens](./img/spreiding.png)

Samenvatting van symbolen
![Samenvatting Symbolen](./img/symbolen.png)

## Datavisualisatie

Datavisualisatiemethodes overzicht
![Samenvatting Grafieken](./img/grafieken.png)

Vermijd ten alle tijden een taartdiagram!

- hoeken vergelijken is moeilijker als lengte vergelijken
- niet bruikbaar voor data met veel categorieen

### Interpretatie diagrammen

tips:

- label assen
- voorzie duidelijke titel
- geef een naam aan de unit, en indien nodig geef duiding bij de ordering, ranking
- voeg een label toe dat duidelijkheid brengt

# H3 centrale limietstelling, hypothesis testen

## Waarschijnlijkheid

relatieve frequentue van de gebeurtenis van de waargenomen evenementen

Makkelijke voorbeelden:
een 6 zijdige dobbelsteen wordt gegooid

- wat is de waarschijnlijkheid om 1 te gooien?
- wat is de waarschijnlijkheid een even nummer te gooien?
- wat is de waarschijnlijkheid om een nummer in de set {1,2,3,4,5,6} te krijgen?

## Axioma's van waarschijnlijkheid

1. waarschijnlijkheden zijn niet negatief, P(A) >= 0 for each A
2. the universe heeft waarschijnlijkheid 1, P(𝛺) = 1
3. wanneer A en B geen samenhangende gebeurtenissen zijn, P(A ∪ B) = P(A) + P(B)

Dit noemt men de somregel

Complementsregel: Voor elke A geldt: 𝑃(ā) = 1 − 𝑃(𝐴)

Waar ā het event "A komt niet voor voorstelt"

Het onmogelijke event heeft waarschijnlijkheid 0, 𝑃(∅) = 0

De generale somregel:

𝑃(𝐴 ∪ 𝐵) = 𝑃(𝐴) + 𝑃(𝐵) − 𝑃(𝐴 ∩ 𝐵)

### Onafhankelijke evenementen

De waarschijnlijkheid wordt niet aangepast door het andere event.

𝑃(𝐴 ∩ 𝐵) = 𝑃(𝐴)𝑃(𝐵)

### Kansverdelingsfunctie

om waarschijnlijkheden te berekenen en in kaart te brengen

![waarschijnlijkheidsgrafiek](./img/waarschijnlijkheidsgrafiek.png)

Expectatie van een random variabele

𝜇<sub>x</sub> of E(𝑋).

𝜇<sub>x</sub>=∑𝑖𝑥<sub>i</sub>𝑃(𝑋 = 𝑥<sub>i</sub>) =∑𝑖𝑥<sub>i</sub>𝑓<sub>x</sub>(𝑥<sub>i</sub>)

Variantie van een random variabele

![Variantie](./img/spreidingvariantie.png)

### Continue Willekeurige Variabele

meetresultaten van lengte, tijd ... zijn voorbeelden

#### Expectatie en variantie

![ExpVar](./img/expvar.png)

## Standaard normale verdeling

![Standaardafwijking](./img/standaardafwijking.png)

### Python functies

| functie                       | doel                                                    |
| ----------------------------- | ------------------------------------------------------- |
| norm.pdf(x, loc=m, scale=s)   | Probability density atx                                 |
| norm.cdf(x, loc=m, scale=s)   | Left-tail probability𝑃(𝑋 <x)                            |
| norm.sf(x, loc=m, scale=s)    | Right-tail probability𝑃(𝑋 >x)                           |
| norm.isf(1-p, loc=m, scale=s) | p% of observations are expected to be lower than result |

### Berekenen waarschijnlijkheden

Met een Z tabel

[Z tabel voorbeeld](http://sixsigmastudyguide.com/wp-content/uploads/2014/04/z-table.jpg)

![Zscores](./img/zscores.png)

#### Gebruikmakende van Python

```python
import scipy.stats as stats
stats.norm.sf(6, loc=5, scale=1.5)
```

## Exponentiele verdeling

![ExpVar](./img/expafw.png)

## (continue) Uniforme verdeling

![uniVer](./img/univer.png)

## van steekproef naar populatie

### centrale limietstelling

als de grootte van de steekproef groot genoeg is, dan zal de waarschijnlijkheidsverdeling van het steekproefgemiddelde een normaaldistributie benaderen, ongeacht de waarschijnlijkheidsverdeling van de onderliggende populatie.

- 1 test
- 25 testen
- 100 testen
- ...

## puntschatting

een puntschatting van een populatie parameter is een formule of vergelijking dat ons toestaat een waarde te berekenen die die waarde schat.

## betrouwbaarheidsinterval

een betrouwbaarheidsinterval is een vergelijking of formule die ons in staat stelt een interval te construeren dat de te schatten parameter bevat met een bepaald betrouwbaarheidsniveau.

[Voorbeeld](https://www.zoology.ubc.ca/~whitlock/Kingfisher/CIMean.htm)

Voor een kleine steekproef kunnen we vaststellen dat het betrouwbaarheidsinterval NIET geldig is.

## Student t-distributie

![tdist](./img/tdist.png)

```python
import scipy.stats
For a t-distribution with df degrees of freedom:
(df = degrees of freedom)
```

| functie           | doel                                                    |
| ----------------- | ------------------------------------------------------- |
| t.pdf(x, df =d)   | Probability density for x                               |
| t.cdf(x, df =d)   | Left-tail probability𝑃(𝑋 <x)                            |
| t.sf(x, df =d)    | Right-tail probability𝑃(𝑋 >x)                           |
| t.isf(1-p, df =d) | p% of observations are expected to be lower than result |

## Conf. int.: Small Sample

![confint](./img/confint.png)

