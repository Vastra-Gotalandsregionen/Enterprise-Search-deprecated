# Västra Götalandsregionens strategiska plan för sökfunktionen

Detta dokument är de aktiviteter Västra Götalandsregionen har för avsikt att jobba med. Det baseras på [mallen för strategisk plan som du finner här](sokstrategi-aktivitetsplan.md).

## Licens

Detta material har tagits fram av [Västra Götalandsregionen (VGR)](http://www.vgregion.se/) i samarbete med flertalet andra offentliga aktörer. Det är inte att betrakta som färdigt. Vi sprider sådan här information för att samverka med externa intressenter. Materialet går under licensen [CC-BY-SA](https://creativecommons.org/licenses/by-sa/3.0/) vilket bland annat medger vidareanvändning.

## VGRs aktiviteter - 2017
Prioritering är att börja med de som är överst och gäller en själv. "Förväntas färdigt" är en önskad prioritering. I april kommer ett avstämningsmöte ske med objektledarna för stämma av hur det går, samt att eventuellt prioritera om de återstående aktiviteterna.

###2017.1 Hitta medarbetare
Ansvarig för punkten: Kristian Norling/intranätprojektet.  
Förväntas vara färdigt: Q2 2017

Följa prioriteringar och värderingar för intranätprojektet. Bland annat att denna personsök ska vara en sammanställning av flera källor, vissa etablerade regulatoriska (HSA/KiV) och andra mer av självservice-karaktär (social personprofil på intranätet).

### 2017.2 Gerilla-tester & inspelad session av sök + hitta medarbetare
Ansvarig för punkten: Frida Erhard + Evelyn Stolfer  
Förväntas vara färdigt: Q2 och en under HT 2017

Både fortsätta med gerilla-testning, men också på distans spela in användares sessioner där de fått uppgifter att lösa.

Frida: leta rätt på lämpligt verktyg för att spela in sessioner på distans.

### 2017.3 Erbjuda sökstatistik till bl.a. Episervers redaktörer
Ansvarig för punkten: Frida Erhard (förnya lösningsförslag och tidsuppskattning), samt Marcus Österberg   
Förväntas vara färdigt: Q1 2017 

Man bör från andra webbaserade system kunna få enklare sammanställningar från verktyget för sökanalys. Exempelvis att från webbredaktörssystem kunna ta del av enklare uppgifter som sökanalys-verktyget samlat in, som nollresultat (att innehåll saknas) och vad som är mest eftersökt, vilka söktrender som finns, etc.

Frågor:

- Vad i Kibana är klokt att lyfta ut till en enskild webbredaktör att se inne i Episerver?
- Kan signal-funktionen till ELK-stacken kan hjälpa till med redaktionella prioriteringar?
- Behöver detta byggas som ett plugin till Episerver?

### 2017.4 Dokumentera sökfunktionens krav på informationskällor
Ansvarig för punkten: Marcus Österberg -> Evelyn Stolfer för peer-review
Förväntas vara färdigt: Q1+Q2 2017

Vilka krav är det som ställs? Dessa behöver dokumenteras, gärna som ett tjänsteutlåtande med förslag till beslut i lämplig nivå inom organisationen. Publicera på Github.

Exempel på punkter att ta med:

 -	Om det ska vara frivilligt att ha med sin informationskälla i sök (förutsatt att den efterfrågats av användare/behov finns).-	Vem som betalar för respektive källas inkluderande/förvaltande i sök.
-  Att lokala eller enskilda initiativ kring sök inte ska betyda att man då “slipper” delta i det gemensamma. Exempelvis huruvida det ska vara valfritt att med avvikande söklösningar rapportera in statistik till verktyget för sökanalys.

### 2017.5 Pitch om; relevansutvärdering, arkivering och indexanalys
Ansvarig för punkten: Frida Erhard -> Marcus för peer-review  
Förväntas vara färdigt: Q2 2017

Testa relevansen, utvärdera och utveckla. Vad döljer det sig för insikter i vårt index, något som kan göra sök mer träffsäkert? Bland annat att jämföra hur interna och externa källor rankas sinsemellan.

Även besvara frågan om hur ett automatiskt "arkiv" skulle kunna bidra. Säg exempelvis att allt äldre än 24 månader är potentiellt dåligt utifall ett visst antal kvalitetskriterier är uppfyllda.

Leverans som presentation / utredning för objektledarna.

### 2017.6 Sök ger feedback om innehållets sökbarhet
Ansvarig för punkten: Marcus Österberg  
Förväntas vara färdigt: Q2 2017

Skrivelse om hur sökmotorn+dess ekosystem skulle kunna bidra till att recensera en webbsidas kvalitet, direkt inne i Episerver. Så redaktören vet om ifall den gjort sökbarheten tillräckligt bra.  
Skrivelsen ska komma med konkreta förslag på åtgärder, om sådana upptäcks. Jämföra med Yoast, mfl.

### 2017.7 Ta med Yammer som källa
Ansvarig för punkten: Evelyn Stolfer  
Förväntas vara färdigt: Q2 2017

Första leverans handlar om de öppna grupperna.

### 2017.8 Keymatch-integration i Episervers redaktörsmiljö?
Ansvarig för punkten: Marcus Österberg  
Förväntas vara färdigt: Q2 2017

Skriva om för- och nackdelar med att göra keymatches integrerat i ett CMS. KM ≈ sponsrade sökningar, med skillnaden att det saknas utgifter eller hårdare prioritering. Hur lösa detta? Med krediter för antal KM:s utanför eget scope, hur många inom sitt eget utan att man helt överger sökredaktionella sysslor?

### 2017.9 Sökfunktionen ger svar på frågor
Ansvarig för punkten: Marcus Österberg  
Förväntas vara färdigt: Q3 2017
  
Utreda vilken verksamhetsnytta som finns i att komplettera vanliga sökfunktionen med svarsmotorfunktionalitet likt [Wolfram|Alpha](http://www.wolframalpha.com/input/?i=v%C3%A4stra+g%C3%B6taland) mfl. Möjligen i form av fakta likt Googles Knowledge Graph, där vi till en början har en kuraterad lista med system som ger träffar, senare för personer och organisationer. Nota bene: Detta behöver synonymhanteras.

### 2017.10 Etablera synonymverktyg i sökredaktörsportalen (Kibana)
Ansvarig för punkten: Frida Erhard + Evelyn Stolfer för genomförande, Marcus Ö för att sprida evangeliet  
Förväntas vara färdigt: Q3 2017

För att kunna göra sökredaktionella synonymer och kunna placera dem inom lokala scope. 

Associationsverktyget kan bli en sökredaktionell motsvarighet till keymatches/bestbets, exempelvis för att kunna koppla ett visst begrepp till ett visst systems adress (som en genväg) eller för att manuellt knyta samman ett mötesprotokoll med dess videoinspelning. Skapa informationspaket genom relationer mellan material som hör ihop.

Leveranser:
1. Frida: Enkel utredning om hur de språkliga relationerna det här verktyget samlar kan återanvändas i andra sammanhang än strikt till sök.
2. Marcus: Utlåtande för på vilket sätt detta kan konkurrera med keymatches.
3. Evelyn: Få upp miljön i SEP samt få till en första manual.

### 2017.11 Införa kompletterande kodverk
Ansvarig för punkten: Evelyn Stolfer  
Förväntas vara färdigt: Q4 2017

Komplettera SweMeSH med något som bättre beskriver kultur, administration, ekonomi, samhälle, pedagogisk, och annan typ av verksamhet. Lösningen behöver integreras med nyckelordsfunktionen i Episerver.

### 2017.12 Estimat på "rika träffar"
Ansvarig för punkten: Frida Erhard  
Förväntas vara färdigt: Q3 2017

Vilken nytta har VGR av att kombinera information från flera datakällor när vi presenterar träffar för sökanvändaren?

### 2017.13 Utreda behörighetsstyrda sök
Ansvarig för punkten: Kristian Norling/intranätprojektet  
Förväntas vara färdigt: Q3 2017

Utreda hur ett behörighetsstyrt sök ska kunna göras. Exempel på källor som ligger nära i tid är Alfresco som mellanarkiv med innehåll som kräver behörighetskontroll, samt Yammers stängda grupper.

Utredningen behöver ha någon form av konceptuell bild, kanske en prototyp.

En fråga att ta upp är hur vi hanterar externa/mobila användare med tanke på att TMG:n inte kan hjälpa till med att förmedla en inloggad användares behörighet.

### 2017.14 Utreda sökdriven navigering och listning
Ansvarig för punkten: Marcus Österberg  
Förväntas vara färdigt: Q3 2017

Utreda och komma med förslag på hur Solr erbjuder sökdrivna menyer, listningar via ett API till exempelvis Episerver CMS. Lämna som förslag till beslut för objektledarna.

### 2017.15 Inventera informationskällor att lyfta till i3
Ansvarig för punkten: Evelyn Stolfer  
Förväntas vara färdigt: Q2 2017

Komma med förslag på i vilken ordning och hur snabbt vi kan lyfta över befintliga källor till i3. Måste alla med? Finns kompetens för att göra en relevansbedömning för respektive fält i varje källa?

Lämna förslag till objektledarna.

## Önskvärda aktiviteter - 2018
Inget ännu.

# Arkiverat

## Utvalda aktiviteter - 2016
###2016.1 "Hitta medarbetare"

Följa prioriteringar och värderingar för intranätprojektet. Bland annat att denna personsök ska vara en sammanställning av flera källor, vissa etablerade regulatoriska (HSA/KiV) och andra mer av självservice-karaktär (social personprofil på intranätet).

Utreda hur detta ska fungera som en mix av DELV, KiV och eventuellt andra personuppgiftskällor. Är det logiskt för en användare att endast interna personkällor används?

###2016.2 Sök- och webbanalys

Påbörja aktiv sök- och webbanalys och ta fram användarstöd. Inrätta funktioner för sökredaktör och community manager (ansvarig för samarbetsytor och sociala kanaler).

Kibana ska läggas under sokanalys.vgregion.se

Se också punkt 2016.11

###2016.3 Komma igång med löpande uppföljning inom sök

Etablera modell för användbarhetstester av sökfunktionen (personsök och övriga).

###2016.4 Utbildningsmaterial till redaktörer och andra

En övergripande handbok är planerad, där bör det ingå en intro till gott innehållsarbete ur en sökmotors perspektiv, samt den dos sökanalys alla bör känna till.

Se också punkt 2016.11 och 2016.6

###2016.5 Söks relation till Sharepoint-sök/innehåll

Ansvarig för punkten: Evelyn Stolfer
Förväntas vara färdigt: Q1 2016

Exempel på punkter:

Hur samverkar sökfunktionen med Sharepoint som tänkt del i nästa intranät. Sharepoint har egen "sök".
Hur fungerar sökfunktionens insamling i relation till det Sharepoint-interna indexerandet?
Hur hanteras personsök genom DELV i kombination med KiV och andra källor (Linkedin, mfl?) som också kan vara externa?
[Marcus] Utreda om befintlig sökfunktion ska visa upp sig som en applikation inne i nästa intranät, snarare än som idag primärt en helt egen webbplats?
###2016.6 Ska sökfunktionen få ställa krav på informationskällor

Ansvarig för punkten: Marcus Österberg, teknikaliteter Frida Erhard
Förväntas vara färdigt: Q1 2016

Om ja så vilka krav är det som ställs? Dessa behöver dokumenteras, gärna som ett tjänsteutlåtande med förslag till beslut i lämplig nivå inom organisationen.

Exempel på punkter att ta med:

Om det ska vara frivilligt att ha med sin informationskälla i sök (förutsatt att den efterfrågats av användare/behov finns).
Vem som betalar för respektive källas inkluderande/förvaltande i sök.
Att lokala eller enskilda initiativ kring sök inte ska betyda att man då “slipper” delta i det gemensamma. Exempelvis huruvida det ska vara valfritt att med avvikande söklösningar rapportera in statistik till verktyget för sökanalys.
###2016.7 Relevansutvärdering

Ansvarig för punkten: Evelyn Stolfer
Förväntas vara färdigt: Q3 2016

Testa relevansen, utvärdera och utveckla. Bland annat att jämföra hur externa och externa källor rankas sinsemellan.

###2016.8 Ersätta befintligt sökgränssnitt

Ansvarig för punkten: Marcus Österberg
Förväntas vara färdigt: Q3 2016

Punkter:

Frida Erhard utvärderar alla delar av nya sökgränssnittet.
Förbättra fliksystemet.
Nya användbarhetstester (Kungälvs sjukhus, troligen).
Eventuellt ersätts befintlig sökfunktion innan midsommar, om det fungerar bra nog.
###2016.9 Erbjuda enkel sökstatistik till andra webbplattformar

Ansvarig för punkten: Frida Erhard (lösningsförslag och tidsuppskattning)
Förväntas vara färdigt: Q2 2016

Man bör från andra webbaserade system kunna få enklare sammanställningar från verktyget för sökanalys. Exempelvis att från webbredaktörssystem kunna ta del av enklare uppgifter som sökanalys-verktyget samlat in, som nollresultat (att innehåll saknas) och vad som är mest eftersökt, vilka söktrender som finns, etc.

Punkter:

Kolla om signal-funktionen till ELK-stacken kan hjälpa till med redaktionella prioriteringar.
###2016.10 Ha ett synonym- och associationsverktyg i sökredaktörsverktyget

Ansvarig för punkten: Frida Erhard (lösningsförslag och tidsuppskattning)
Förväntas vara färdigt: Q1 2016

För att kunna göra sökredaktionella synonymer och relationskopplingar för enkla ordlistor med synonymer och mer strukturerade relationer mellan olika resurser som sökmotorn känner till.

Associationsverktyget är en sökredaktionell motsvarighet till keymatches/bestbets, exempelvis för att kunna koppla ett visst begrepp till ett visst systems adress (som en genväg) eller för att manuellt knyta samman ett mötesprotokoll med dess videoinspelning.

###2016.11 Utbilda i sökanalys

Ansvarig för punkten: Frida Erhard (tidsuppskattning) / Marcus Österberg
Förväntas vara färdigt: Q1 2016

Hålla en enklare introduktion i sökanalysverktyget Kibana. Målgrupp är kommunikatörer och webbredaktörer.

Punkter:

Frida Erhard tar fram tidsuppskattning för introduktionen (om hon håller den).
Frida genomför kursen.
Marcus filmar kursen och producerar ett användarstöd baserat på detta, möjligen som en intern poddsändning.

## Utvalda aktiviteter - 2015

### 1. Vi har behov av en organisationsövergripande sökredaktör
Ansvarig för punkten: Marcus Österberg  
Förväntas vara färdigt: Q1 2015  
Antecknat: Meddela den det berör i organisationen.

### 2. Vi behöver förstå vad användarna söker efter och hur de söker, det vill säga kunna göra sökanalys
Ansvarig för punkten: Marcus Österberg  
Förväntas vara färdigt: Q4 2015  
Antecknat: Utvärdera standardprodukter.  

### 4. Vi upplever att dokument och webbsidor inte riktigt är jämnbördiga i sökresultatet
Ansvarig för punkten: Evelyn Stolfer  
Förväntas vara färdigt: Q2? 2015  
Antecknat: Vilka källor, genomgång av relevansmodell.

### 5. Det finns externa informationskällor vi borde ha i vår interna sökfunktion
Ansvarig för punkten: Evelyn Stolfer  
Förväntas vara färdigt: Q3 2015  
Antecknat: Vårdhandboken har varit på tal bl.a. 

### 6. Ibland är vissa källor lite mer relevanta än andra
Ansvarig för punkten: Evelyn Stolfer  
Förväntas vara färdigt: Q3 2015  
Antecknat: Vårdhandboken har varit på tal bl.a. 

### 7. De som fyller sökmotorn med innehåll skulle behöva hjälp med sin metadata
Ansvarig för punkten: Marcus Österberg  
Förväntas vara färdigt: Q3 2015  
Antecknat: Kolla EPiServer 7 etc. 


### 8. Våra system ställer för låga krav på den metadata man som användare tvingas ange
Ansvarig för punkten: Evelyn Stolfer  
Förväntas vara färdigt: Q2 2015  
Antecknat: Ta fram ett förslag på minsta mängd metadata och koppling mot exempelvis extern metadata-server för verifiering.

### 9. Användarna söker inom ett filter utan att veta om vad de möjligen missar
Ansvarig för punkten: Marcus Österberg  
Förväntas vara färdigt: Q2 2015  

### 10. Sökfunktionen tycks inte förstå min sökfras
Ansvarig för punkten: Evelyn Stolfer  
Förväntas vara färdigt: Q4 2015  
Antecknat: Börja med just frassökning.