# Railframe — Privacyverklaring

Laatst bijgewerkt: 27 oktober 2026.

## 1. Over Railframe

Railframe wordt zelfstandig ontwikkeld en aangeboden als hobbyproject. De app wordt niet namens een werkgever of opdrachtgever aangeboden.

Er is geen helpdesk of mogelijkheid om contact op te nemen voor ondersteuning. Er is geen afzonderlijke privacycontactpersoon of functionaris gegevensbescherming aangesteld.

Gebruik je Railframe voor je werkgever of opdrachtgever? Die organisatie kan zelf verantwoordelijk zijn voor de inhoud van projecten, foto's en exports en voor het gebruik daarvan. Raadpleeg in dat geval ook de privacyinformatie van die organisatie.

## 2. Welke gegevens gebruikt Railframe?

| Gegevens | Doel en verwerking |
| --- | --- |
| Locatie, GPS-nauwkeurigheid en kompasrichting | Spoorpositie bepalen, kaartweergave, nabijgelegen objecten vinden en locatiegegevens aan foto's koppelen. |
| Foto's en eventueel originelen zonder overlay | Werkzaamheden en objecten vastleggen binnen een project. Foto's kunnen herkenbare personen of andere persoonsgegevens bevatten. |
| Fotometadata | Onder meer tijdstip, coördinaten, geocode, kilometrering, spoornaam, kijkrichting, tags en opmerkingen vastleggen en exporteren. |
| Projectnaam, geocodes en projectgegevens | Projecten ordenen en de relevante spoorgegevens beschikbaar maken. |
| Instellingen | Je voorkeuren voor onder meer overlay, bestandsnamen, zoekradius en Watch-updates bewaren. |
| Netwerkgegevens | Externe diensten kunnen bij verzoeken je IP-adres, het tijdstip en de opgevraagde zoektermen, gebieden of kaarttegels ontvangen. |

Railframe haalt spoor- en kaartgegevens op om je locatie te bepalen en je foto's van passende labels te voorzien. De opgehaalde gegevens worden ook gebruikt voor de kaartweergave en objectmeldingen.

Je foto's, opmerkingen en projectbestanden blijven lokaal op je apparaat en worden niet automatisch naar de maker of een centrale server geüpload. Je deelt deze bestanden alleen wanneer je zelf een foto of project deelt. Het ophalen van spoor- en kaartgegevens vereist wel uitwisseling van netwerk- en aanvraaggegevens met de betrokken diensten. Ook kan de app een locatiesamenvatting naar je gekoppelde Apple Watch sturen. Deze uitwisseling staat beschreven in onderdeel 5; apparaatback-ups staan beschreven in onderdeel 4.

De huidige publieke app vereist geen Railframe-account. In de onderzochte appcode is geen eigen uploaddienst voor projecten of foto's en geen advertentie- of analytische tracking ingebouwd.

## 3. Locatie en camera

Railframe vraagt via iOS toegang tot je locatie en camera. Je kunt die toegang weigeren of later wijzigen in de instellingen van je apparaat. Zonder locatie kan de app je actuele spoorpositie niet betrouwbaar bepalen. Zonder cameratoegang kun je in de app geen nieuwe foto maken.

Voor **Live Watch updates op achtergrond** kan Railframe ook locatie blijven gebruiken wanneer de app niet op de voorgrond staat. Deze instelling is standaard ingeschakeld. De app kan daarvoor aanvullende locatietoestemming vragen. Je kunt achtergrondupdates uitschakelen onder **Watch en haptiek** en de locatietoestemming aanpassen in iOS.

De app bewaart locatiegegevens bij opgeslagen foto's. De huidige implementatie bevat geen afzonderlijke opslag van een doorlopend routeverleden. Dat betekent niet dat er geen locatiegegevens worden opgeslagen: foto-informatie, gedeelde bestanden en verzoeken aan externe diensten kunnen locaties bevatten.

## 4. Waar worden gegevens opgeslagen?

Projecten, gedownloade spoorgegevens, foto's, beschikbare originelen, metadata en exports worden lokaal in de appopslag bewaard. Instellingen worden eveneens lokaal opgeslagen.

Afhankelijk van je apparaatinstellingen kunnen appgegevens worden opgenomen in een iCloud- of computerback-up. Als je bestanden zelf in iCloud Drive of een andere opslagdienst bewaart, geldt ook het beleid van die dienst. Railframe biedt in de huidige implementatie geen eigen centrale projectsynchronisatie.

## 5. Externe diensten en ontvangers

### Spoorgegevens en kaartbeelden

Railframe haalt spoor- en objectgegevens op bij ProRail via `maps.prorail.nl`. Daarbij kunnen zoektermen, geocodes of een opgevraagd geografisch gebied worden meegestuurd. De dienst ontvangt daarnaast netwerkgegevens, zoals het IP-adres waarmee je verbinding maakt.

Voor kaartweergave gebruikt de app Apple MapKit en, afhankelijk van de gekozen achtergrond, luchtfoto-tegels via `storage.georizon.nl`. De opgevraagde kaarttegels geven aan welk gebied je bekijkt. Dat gebied kan samenvallen met je actuele locatie.

Kies je **Route plannen in Kaarten**, dan wordt de gekozen bestemming aan Apple Kaarten doorgegeven. Het verdere gebruik valt onder de instellingen en privacyvoorwaarden van Apple Kaarten.

### Apple Watch en CarPlay

De app geeft een samenvatting door aan je gekoppelde Apple Watch en kan die tonen via CarPlay. Deze omvat onder meer projectnaam, geocodes, baanvak, kilometrering, spoornamen, GPS-nauwkeurigheid, nabijgelegen objecten en het tijdstip van de update. De Watch-uitwisseling verloopt via Apple's WatchConnectivity.

### Functies die in de huidige publieke configuratie uitstaan

De code bevat ondersteuning voor NS-treinmeldingen en afgeschermde ProRail-diensten. In de huidige publieke configuratie staan treinmeldingen uit en worden opgeslagen ProRail-tokens en NS-API-sleutels bij het laden van de configuratie gewist uit de actieve configuratie. Deze functies worden daarom hier niet als reguliere gebruikersfuncties aangeboden.

Als een toekomstige of aangepaste versie deze functies activeert, kunnen voor NS-treinmeldingen exacte breedte- en lengtegraad, zoekradius en een API-sleutel naar `gateway.apiportal.ns.nl` worden gestuurd. Voor afgeschermde ProRail-diensten kunnen aanmeldgegevens naar het ProRail-tokenendpoint gaan en tokens met gegevensverzoeken worden meegestuurd. Deze verklaring moet vóór het beschikbaar stellen van zulke functies worden bijgewerkt.

### Door jou gekozen ontvangers

Als je een foto of export deelt, bepaalt jouw keuze welke app, opslagdienst of ontvanger die gegevens krijgt. Een ZIP-export kan foto's met overlay, originelen en een CSV met locatiegegevens en opmerkingen bevatten. Het verbergen van velden in de overlay verwijdert die velden niet uit de metadata.

### Verwerking door dienstverleners

Externe diensten kunnen eigen logbestanden bijhouden. Railframe bepaalt hun bewaartermijnen niet vanuit de app.

## 6. Doelen van het gegevensgebruik

Railframe gebruikt gegevens om de door jou gekozen project-, locatie-, foto- en exportfuncties uit te voeren. Optionele achtergrondfuncties dienen om locatie-informatie ook op verbonden apparaten actueel te houden.

Een iOS-toestemming voor camera of locatie is een technische toegangsinstelling en bepaalt op zichzelf niet de AVG-grondslag. Als een verwerking berust op toestemming, kun je die intrekken. Intrekking verandert niets aan de rechtmatigheid van de verwerking vóór dat moment.

## 7. Bewaren en verwijderen

Lokale projecten en foto's blijven bewaard totdat je ze verwijdert; de huidige app kent hiervoor geen automatische vervaltermijn.

- Je kunt foto's afzonderlijk verwijderen vanuit de fotodetails.
- Met **Project verwijderen** verwijder je de lokale projectgegevens, foto's en bijbehorende projectexports.
- Eerder gemaakte exports kunnen nog gegevens bevatten van foto's die je later afzonderlijk hebt verwijderd. Verwijder zulke exports apart als je die gegevens ook daar wilt wissen.
- Bestanden bij ontvangers, kopieën in andere apps en apparaatback-ups worden niet automatisch aangepast of verwijderd wanneer je in Railframe gegevens verwijdert.
- Het verwijderen van de app verwijdert normaal gesproken de lokale appopslag. Het opruimen of ontladen van een app door iOS kan gegevens juist bewaren. Controleer back-ups en los opgeslagen bestanden afzonderlijk.

Omdat geen supportkanaal wordt aangeboden, is er geen proces voor het ontvangen en bewaren van supportcorrespondentie of projectbestanden voor ondersteuning.

## 8. Beveiliging

Railframe gebruikt de appopslag van iOS. De in de app ingestelde externe webadressen gebruiken HTTPS. De app voegt geen eigen wachtwoordbeveiliging toe aan geëxporteerde ZIP-bestanden.

Beveilig je apparaat met een toegangscode en deel bestanden alleen met de bedoelde ontvangers. De aanbieder heeft via de huidige app geen centrale kopie waarmee verwijderde lokale projecten kunnen worden teruggezet.

## 9. Je privacyrechten

Afhankelijk van de verwerking en de toepasselijke voorwaarden kun je vragen om inzage, correctie, verwijdering, beperking of overdracht van persoonsgegevens en bezwaar maken tegen verwerking. Voor gegevens die uitsluitend op jouw apparaat staan, kun je veel handelingen zelf via de app uitvoeren. De maker heeft via de app geen toegang tot die lokale bestanden. Voor projectverwerking door je werkgever kun je die organisatie benaderen. Voor verwerking door externe diensten kun je de privacyinformatie van de betreffende dienst raadplegen.

Meer informatie staat op de pagina [Uw privacyrechten gebruiken van de Autoriteit Persoonsgegevens](https://autoriteitpersoonsgegevens.nl/nl/onderwerpen/algemene-informatie-avg/rechten-van-betrokkenen).

Je kunt een klacht indienen bij de Autoriteit Persoonsgegevens. Neem eerst contact op met de betrokken organisatie om een oplossing te zoeken. Zie [een tip of klacht indienen bij de AP](https://autoriteitpersoonsgegevens.nl/nl/contact-met-de-autoriteit-persoonsgegevens/tip-ons/).

Railframe bevat in de huidige implementatie geen geautomatiseerde besluitvorming met juridische of vergelijkbare ingrijpende gevolgen. De berekende spoorpositie is een ondersteunende indicatie.

## 10. Wijzigingen

Als de functies of gegevensverwerking veranderen, wordt deze verklaring aangepast. De datum bovenaan geeft aan wanneer dit document voor het laatst is bijgewerkt.

Praktische instructies voor de app staan in de [handleiding](HELP.md).
