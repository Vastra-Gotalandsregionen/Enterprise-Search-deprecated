#Västra Götalandsregionens sökstrategi#

##Snabbintro & licens##
Denna sökstrategi är inte klar och den kommer aldrig bli klar. Se detta som ett levande dokument som jagar det rörliga målet att **relevant information ska vara lätt att hitta samt återanvända**.

###Licens##
Detta material har tagits fram av [Västra Götalandsregionen (VGR)](http://vgregion.se). Det är inte att betrakta som färdigt. VGR sprider sån här information för att samverka med externa intressenter.  
Materialet går under licensen [CC-BY-SA](https://creativecommons.org/licenses/by-sa/3.0/) vilket bland annat medger vidareanvändning.

##Utgångspunkt##

###Definitioner###

- **Sök & sökteknik** - med ordet sök avses det ekosystem av mjukvaror som hjälper till med att låta användare söka efter information, såväl sök-gränssnittet gentemot användare men också den bearbetning som görs för att en källa ska bli sökbar.
- **API** - står för *Application Programming Interface* och är det tekniska gränssnittet för att utföra en sökning eller mellan system kommunicera med sökmotorn.
- **Relevansmodell** - de utvalda viktningsfaktorer som styr vilken informations som anses viktig i relation till annan. Exempelvis att ett sökords förekomst i en titel är viktigare än i en brödtext.
- **Metadata** - information om information. Kan exempelvis vara ett nyckelord webbredaktören satt på en webbsida eller datumet när ett dokument senast ändrades.
- **Metadata-märkning** - själva aktiviteten att skaparen av informationen märker, beskriver alltså, sin skapelse med extra information som dess kategori, skriver en kort beskrivningstext, relaterar den till någon etablerad branschterm etc.
- **Keymatch** - ibland kommer det en träff ovanför det vanliga sökresultatet. Det är vad som kallas för sponsrad träff på kommersiella sökmotorer men används internt för att vägleda till "rätt" träff som av någon anledning inte kommer högt nog i träfflistan.

###Syfte###
Syftet med sök är att **relevant information ska vara lätt att hitta samt återanvända** för alla berörda av information VGR har i sina informationssystem.

###Söks roll i den totala informationsförsörjningen (målgrupper)###
Grov uppdelning av målgrupper kan göras till **medborgare** samt **anställda**, men man bör även komma ihåg följande grupper:

- *Privata vårdgivare* med avtal. Har viss domänexpertis men kan vara nybörjare på VGR:s synsätt.
- *Andra externa intressenter* och aktörer som har en yrkesmässig anledning i sin kontakt med VGR, exempelvis de som vill söka bidrag.
- Andra *tekniska plattformar* som behöver åtkomst till information sök-miljön samlat på sig. Det kan bland annat vara att tipsa en anställd om internutbildning viktat på faktorer som geografisk närhet, kostnad och yrkesroll.

Den största skillnaden mellan medborgare och anställda är att medborgare inte har, eller bör ha, anledning att förstå verksamhetens komplexitet eller struktur - de har ett informationsbehov och det bör räcka för att hitta fram.

####Sök är mer än en sökruta####
Både som sökruta men också som informationskälla (via API) till andra system. Jämför med Google Now och andra relevansstyrda "tips".

##Övergripande mål##
Målet med sök är att det ska vara lätt att komma över den information man behöver, när man behöver den och på det sätt man behöver den.

##Handlingsplan i det korta perspektivet##

###Förslag på aktiviteter år 1###

####1. Upprätta rollen organisationsövergripande sökredaktör####
Arbetsuppgifter... Verksamhetsperson...

####2. Sök-scopes vara eller icke-vara####
Hur ska man jobba med de scope (avgränsande organisatoriska filter) som idag används frekvent? Ett förslag har varit att helt ta bort scope, ett annat att baserat på första träffens relevans matcha mot träffar utanför scope.

####3. Arbeta med frassökning, stoppord och synonym-hantering####


####4. Utvärdera keymatches i sökresultatet####
Finns bättre lösning? MDM/Knowledge Graph/Termlista om plats finns & relevans är hög nog?

####5. Modernt användargränssnitt####
Det som möter en användare _måste_ idag fungera i en mobiltelefon och vara anpassat för pekskärm som inmatningsmetod.

####6. Utreda möjligheter till personaliserat sök####
Finns behov till ett personaliserat sök och vad är i så fall viktigast att fixa först? Behöver hantera att användaren inte ska hamna i någon filterbubbla.  
En förutsättning för detta är att veta lite mer om vem den sökande är. På externa webben (om vi väljer att använda det även där) finns indikationer som geografisk plats och beteendedata, internt kan vi ofta komplettera samma uppgifter med eventuell inloggning tillsammans med koppling till medarbetarregister.


###Förslag på aktiviteter år 2###

####1. Sökanalys på bredden####
Meddela skapare av information vilken av deras information som inte är särskilt sökbar på grund av SEO-faktorer. Kan bli lång lista...

Idag listas inte om det är extern sökare, vilket scope man befann sig i etc vilket gör det svårarbetat.

Utvärdera nuvarande systemstöd för sökanalys. Troligtvis borde vi försöka hitta en standardprodukt för detta eller annat arbetssätt som är lättare för noviser att använda/omsätta till kunskap. Kanske funkar [SSA](http://sematext.com/search-analytics/)?

####2. Utreda möjligheter och behov av svarsmotor####
Erbjuda funktionalitet som inspirerats av Google Now, Wolfram Alpha och Knowledge Graph. En simpel början är att kunna söka upp definitionen av de termer verksamheten använder sig av (likt _define: term_).

####3. Påbörja arbete med konsekvensbeskrivning av dokument vs webbsidor####
Går det att få till en vettig relevansmodell när dokument och webbsidor har så olika förutsättningar till metadata-märkning.

####4. Inventera externa källor att indexera####
De externa platser där VGR bidrar med innehåll. Exempel på dessa är publikt tillgängliga sociala medier såsom Twitter, Instagram mfl.

####5. Utvärdera möjligheten att boosta källor baserat på sökterm####
Jobba med register över "aktiveringsord". Exempelvis en sökning på *blodgivning* på externa sökfunktionen kanske bör boosta källan geblod.nu?

Går detta att automatisera eller göras hanterbar i större skala över längre tid?

###Förslag på aktiviteter i mån av tid & energi###

####Se över kriterier för att indexera datakälla####
Vilka kriterier talar för och vilka talar emot? Data-discovery...

####Utreda möjligheterna till bättre metadata-hantering####
RDFa bland annat.

####Utreda möjligheten till testbarhet inom relevansmodell####
Går det att förutse påverkan på sökresultat baserat på ett antal sökpersonas, 1000 vanligaste söktermerna eller liknande?

##Ansvar och genomförande##
Under förutsättning att budget tilldelas kommer sökstrategins förverkligande drivas av *Objektet för kommunikation via webbtjänster* i samarbete med andra intressenter.

##Utestående relaterade frågor##
Denna strategi har beroenden till bland annat följande:

- Digital livscykelhantering för information (dvs hur man får användare att metadata-märka korrekt, välja rätt format, arkivera samt ibland återanvända).
- PSI-data, öppna data och länkade data.
- IT-produktstrategi i den mån IT:s beslut påverkar verksamheten i form av tekniska plattformar.

Inspirationskällor:

- [Intranet Focus: Developing an enterprise search strategy](http://www.intranetfocus.com/wp-content/uploads/Enterprise-Search-Strategy.pdf)
- [Findwise: Enterprise Search and Findability Survey 2014](http://www.slideshare.net/findwise/mattias-enterprise-search-and-findability-survey-2014-findability-day-2014) [[beställ rapporten](http://www2.findwise.com/findabilitysurvey2014)]