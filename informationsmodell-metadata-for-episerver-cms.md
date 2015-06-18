# Informationsmodell: Metadata för Episerver CMS (version 0.9)

## Beskrivning och tolkning av uppdraget

Vår tolkning är att vi ska lämna ifrån oss en pragmatisk partsinlaga om vilken metadata vi anser att en modern och mångsidig webbplats bör innehålla. Då definitionen av “metadata” varierar stort har vi valt att göra en ganska inkluderande tolkning - all information som beskriver annan information anser vi ingå i begreppet metadata.

Med andra ord inkluderar vi saker som sidtitlar, huvudrubriker, nyckelord, beskrivningstexter ända ner till hänvisande data som enskilda HSA-IDn för en verksamhet, verksamhetskoder, koder till vokabulär som SweMeSH, geografiska platser genom latitud/longitud och så vidare.

Vi har ett antal utgångspunkter för arbetet, nämligen att:

1. Dra inspiration från [dokumenthanteringens metadataspec (version 1.6 från juni 2014)](https://drive.google.com/file/d/0B5NNZhJG9NGlYkZCUkF0YnpFX1E/view?usp=sharing).
2. Använda metadata-standarden Dublin Core där den är tillämplig.
3. Det behövs mer koppling mellan webbarbetet och kodverk/informatik-arbetet. Exempelvis saknas standardiserade nyckelord/begrepp av administrativ karaktär, för omvårdnad, rehabilitering och potentiellt ännu fler. Med andra ord får informatikgruppen vårt stöd i inventerandet av fler vokabulär ([EuroVoc](http://eurovoc.europa.eu/drupal/?q=sv) bland annat).
4. Ett ordnat arbete med att kuratera en regional folksonomi (motsvarar “författarens nyckelord” i Barium) behöver komma igång.
5. Vi räknar med en funktionell integration till kodverkservern Apelon, eller motsvarande, för att kunna använda vokabulär som SweMeSH, ICD-10 samt att kunna etablera vokabulär som behövs för webbarbetet.
6. Gränssnittskod på webben måste använda mikrodata-tekniker som [schema.org](https://schema.org/), bl.a. för Googles och vår egen sökmotors skull. Mikrodata berikar hela sidor och delar av sidor med maskinläsbar semantik avseende vad innehållet är.
7. Det måste vara genomförbart, att redaktörerna ska kunna använda det hela. Verktyget måste vara användbart. Hur skapas ett bättre stöd för redaktörerna? Automatik via mallar, sökordsförslag via Apelon osv. Det innebär inte att redaktörerna ska diktera villkoren men vi vill inte att det ska vara onödigt betungande att göra rätt.
8. Det ska gå att exkludera sidor från det ambitiösa arbetet, men att konsekvensen blir tydlig för skaparen. Om inte tillräcklig metadata anges får skaparen en varning om vad som saknas, väljer hen att inte rätta till missförhållandet kommer innehållet exkluderas från sök och andra sammanställningar där det enbart skulle bidra till informationsbrus.
9. Inte tillåta uppladdning av filer på webben - webben är till för webbinnehåll. De filer som hör hemma i andra system behöver integreras så det blir användbart. De system som är bra på dokument, bilder etc får ta hand om de filerna. Huruvida man knuffar över filer från Episerver till Alfresco lägger vi oss inte i, men ingen upload-katalog bör få lov att finnas. Eventuellt med undantag för att man får använda sidans lokala katalog i Episerver. Det kan ha ett syfte när man publicerar. Kortlivad info och vill koppla dokument som då också automatiskt raderas när webbsidan raderas.

## Med bra metadata får vi…

Att innehåll har bra metadata är en förutsättning för många andra tekniska verktyg. Tydligast blir det när man söker i en sökmotor - saknas metadata är “rätt” innehåll väldigt svårt att hitta oavsett vad man söker på.

Samtidigt är det svårt att bygga ett modernt och mångsidigt informationssystem utan metadata, då kan inte innehåll återanvändas inom webbplatsen eller uppstå i flera kombinationer utan blir väldigt redaktionellt och manuellt styrd, vilket kräver mycket onödigt arbete.

Drivkrafterna bakom ett genomtänkt metadata-arbete är bland annat:

- Kunna styra information bättre. Personalisera användarens upplevelse så den blir mer relevant och aktuell till dennes sammanhang.
- Lägger grunden till en smartare webbplats, exempelvis genom att kunna filtrera bättre.
- Ge sökmotorer bättre metadata så både internt och externt sök kan bli bättre, detta genom att innehållets art blir maskinläsbar.
- Lägga grunden för mer mångsidigt innehåll på webben, innehåll som kan kombineras på nya sätt för att möta den uppsjö med uppkopplade prylar som används.
- Kunna markera innehåll som mindre viktigt, som exempelvis olämpliga för sökmotorn (högerkolumner idag, testsidor m.m.).
- Avgränsa tolkningsutrymmet inom begrepp genom samordnad synonymhantering, folksonomi och etablerade vokabulär i kombination så innehållet blir mångsidigt, återanvändbart och kan kombineras även utanför den enskilda webbplatsen.

Vi föreslår att introducera tvingande fält, i lagom balans. Dessutom, om möjligt, ha kvalitetskrav på den metadata som fylls i, exempelvis att tillräckligt mycket metadata anges på respektive nivå samt att en grundnivå av strukturerad metadata uppfylls. 

På sikt föreslår vi en modell där den tvingande grundnivån uppfylls snabbare om skaparen använder nyckelord som finns i ett vokabulär än om man hittar på helt egna nyckelord, exempelvis. Introducera en varningsruta om innehåll skapas där inte tillräckligt mycket kvalitativ metadata finns och göra klart för skaparen vilka konsekvenser det får för hens innehåll och hens möjlighet att nå ut med det.

## Nivåer av metadata

Det går att sätta metadata på flera olika nivåer i ett webbpubliceringssystem. Nedan har vi något sånär följt atomisk design genom den minsta beståndsdelen är **block/komponent**, som kan kombineras med andra till en **sida**, sidor som sedan utgör en **webbplats**. 

Ett block kan vara en ruta med kontaktuppgifter hämtade från KiV (metadatan är HSA-ID för uppslag mot KiV), detta kan vara del av en kontaktsida bestående av ett flertal andra block (där metadata kan vara vem man vänder sig till, geografisk plats etc) och webbplatsen är ett av sjukhusens (med metadata som telenummer till växel, infoansvarig etc).

I samtliga fall skall den kommunikativa principen viktigast-först följas! Man kan idag inte räkna med att innehållet visas upp i sin helhet oavsett hur kort det är.

### Webbplatsövergripande

Viss metadata har enbart med den övergripande nivån att göra, ibland återanvänds den längre ner på en webbplats. Tänk på det som i vilka meningsbärande data som kan ingå för att göra en övergripande/gemensam konfiguration av hela webbplatsen.

Vad varje webbplats bör innehålla/beskriva på ett övergripande plan (_obligatoriska fält_):

- Information om eventuella webbplatsövergripande kopplingar till konton på sociala medier. Detta inkluderar bland annat Facebooks Open Graph, Twitters Cards. Detta är metadata som ger relation på toppnivå till toppnivån i andra kanaler verksamheten använder för att kommunicera.
- **(DC.audience)** Vem är målgrupp eller tilltänkt “läsare”? Helst om detta kan anges på ett standardiserat sätt med dropdowns snarare än fritext. Detta för att stödja personalisering. 
- Geografisk mittpunkt. En eller flera geografiska mittpunkter för en tilltänkt mottagare/användare - exempelvis latitud/longitud för en särskild klinik. Denna position ska kunna kompletteras med en graderad skala (1-10, 1 = hyperlokalt-> 5=regionalt intresse -> 10=nationellt intresse) av hur snabbt relevansen avtar med avståndet.
- Ämne/informationsdomän enligt någon lämplig standard, som dropdowns snarare än fritext. 
- Webbplatsnamn. En valfri version och en mycket kort version som strävar mot att få plats i flikar i webbläsaren bland annat.
- Beskrivning av hela webbplatsen. En med valfri längd och en som är mellan 80-160 tecken lång. Minst en av dessa ska fyllas i.

Valfria fält:

- Nyckelord som beskriver webbplatsen, synonymer. Koppla till metadata-tjänsten/Apelon för att få hjälp med nyckelord.
- Information om avsändaren samt ansvarig utgivare, angett som HSA-ID, samt kompletterande kontaktuppgifter. Kan vara organisationsnummer, utgivarens mejladress, telefonnummer med mera.

Dessa övergripande metadata ska ses som “smittsamma” nedåt i informationsmodellen! Exempelvis så att nyheter som skapats för Angereds Närsjukhus (med angiven intresseradie) kommer långt ner i relevansmodellen för nyhetssök för en på Frölunda Sjukhus och kanske inte alls i Mariestad.

### Webbsida (undersida)

En webbsida är en sammanställning av en eller flera block/komponenter. 

Obligatoriska fält:

- Minst 1 nyckelord ska anges. Antingen författarens egna (folksonomi) men allra helst ett nyckelord från metadata-tjänsten/Apelon. Behöver stöd av flera vokabulär än MeSH, ICD och SnoMed-CT för all övrig verksamhet. ÄÖven geografiska platser behöver hanteras, kanske plocka in GeoNames?
- **(DC.date.validto)** Gallring/förväntad livslängd - för att instruera arkiveringsrutinen. Samma fält som Epi har idag, “Sluta publicera-datum”.
- Titel och alternativ titel. En valfri version och en mycket kort version som strävar mot att få plats i flikar i webbläsaren bland annat.
- Beskrivning av webbsidan. En med valfri längd och en som är mellan 80-160 tecken lång.
- Vem är målgrupp eller tilltänkt “läsare”? Stödja personalisering. Följa standardiserade målgrupper, fylls i med dropdowns.

Andra fält:

- Vikta information per standardiserad tilltänkt målgrupp? Orkar redaktörerna? Kan det automatiseras genom att tillräckligt mycket god metadata finns har sidan 100% kvalitet. (återanvänds i sitemap, och hjälper till i personalisering).

Villkorad metadata:

- Eventuella undantag från webbplatsövergripande metadata, bland annat kan man stundtals behöva göra undantag för att nå utanför sin personaliseringsbubbla - som kan vara hyperlokal geografiskt. Eventuella kopplingar till Facebook Open Graph, Twitter Cards (sociala metadata på sidnivå).
- **(DC.source)** Där extern källa/ursprung behöver refereras ska URI samt status (same-as etc) alltid anges. Används ibland som kanonisk hänvisning, annars som metadata för framtida mångsidighet. Peka ut relation till exempelvis PDF-riktlinje. Kan vara en nyhet som sammanfattar ett längre protokoll.
- Behövs kontaktuppgifter eller annat som kan struktureras skall det anges enligt standarden schema.org (till en början åtminstone kontaktuppgifter, person och organisation, geografisk plats, typ av innehåll)

Automatisk metadata (eller “latent” metadata):

- (DC.type.templatename) Typ av sidmall.
- (DC.creator) Skapare av innehåll.
- (DC.identifier.version) Version.

Gränssnittsbehov:

- Dåligt med metadata ≈ varning att sidan inte kommer finnas i sökmotorn, A-Ö-listor etc. Avsaknad metadata får konsekvenser som blir påtagliga för redaktören.

### Komponenter/block

Detta är de standardiserade komponenter man ska kunna lägga till på en undersida. En komponent kan exempelvis vara en nyhetstext, ett kontaktblock med uppgifter från KiV osv. 

Då block kan vara av extrem variation så finns inga obligatoriska fält för alla fält, istället ska allt som kan struktureras också vara det - exempelvis med hjälp av mikrodata-teknik som schema.org - och referenser skall anges på ett maskinläsbart och identifierande sätt.

Obligatoriskt för redaktionella block:

- **(DC.date.validto)** Gallring/förväntad livslängd - för att instruera arkiveringsrutinen. Samma som “Sluta publicera-datum”.
- Vem är målgrupp eller tilltänkt “läsare”? Görs via dropdowns.
- Nyckelord som beskriver komponenter/block, och eventuellt nödvändiga synonymer. 

Automatisk metadata (eller “latent” metadata):

- (DC.type.templatename) Typ av komponent/block.
- (DC.creator) Skapare av innehåll.
- (DC.identifier.version) Version.

Villkorad metadata:

- “KiV-blocket” ska refereras via **HSA-ID**, både person och verksamhet ska stödjas. Plocka ut uppgifter på Roll, typ chefen-på-verksamhet-med-HSA-ID.
- Kunna länka in Tillgänglighetsdatabasen via **HSA-ID**, gå via TD:s öppna data.
- **(DC.source)** Där extern källa/ursprung behöver refereras ska URI samt status (same-as etc) alltid anges.
- Eventuella undantag från webbplatsövergripande metadata, bland annat kan man stundtals behöva göra undantag för att nå utanför blockets personaliseringsbubbla.
- Om komponenten/blocket är en webbmotsvarighet till material på annan plats skall URI anges. Används ibland som kanonisk hänvisning, annars som metadata för framtida mångsidighet. Kan exempelvis vara en nyhetstext om ett styrelsemöte vars kalenderuppgift finns på annan plats, då ska URI till den andra platsen anges. 
- Behövs kontaktuppgifter eller annat som kan struktureras skall det anges enligt standarden schema.org (till en början åtminstone kontaktuppgifter, person och organisation, geografisk plats, typ av innehåll)

———  
2015-06-18  
Förslag från metadata-grupp bestående av: Malena Sjöstrand, Marie Rezelius, Mikael Svahn, Marcus Österberg och Kenny Stolpe.