---
---
Laddningstid
=======================

Uppgiften går ut på att se hur laddningstiden är på några olika webbplatser och se om det finns saker som kan förbättras när det gäller laddningstiden och andvändbarhet.

Urval
-----------------------

Jag valde att välja tre nyhetssajter, jag har redan gjort en rapport tidigare ang. färgchemat på Aftonbladet, Expressen och Dagens Nyheter och valde att analysera samma sidor då jag även är intresserad i hur laddningstiden och användbarheten är på sidorna. Jag tror även att det ärbra att ta tre liknande webbplaster, därav valet att ta tre nyhetssajter, då det är liknande innehåll som skall presenteras.

Metod
-----------------------
Jag använde mig av Google Kalkylark för att skriva ner mina värden jag mätte i uppgiften. Jag använde mig av PageSpeed för att se vad sidorna kunde förbättras i och vad de fick för betyg enligt PageSpeed och jag använde mig av Devtools för att se sidornas laddningstider, storlek och hur mycket resources som fanns.

Resultat
-----------------------

[Kalkylark resultat](https://docs.google.com/spreadsheets/d/18I4ZIz4S9L5z8BuzHKyEf8s7K2bvJvyHwGlIFzARB1Y/edit#gid=0)


[FIGURE src=image/dagens_nyheter.png?w=900]
[Dagens nyheter](https://www.dn.se/)
Dagens nyheter skulle kunna justera sin CSS, att endast den critical CSS (den CSS som behövs för att veta hur stylingen på sidan skall se ut) laddas direkt först medan den uncrtitical CSS (den CSS som behövs när man gör ngt på en sida, t.ex. ett popup-fönster som visas först efter att man tryckt på en knapp) som behövs istället laddas senare.


[FIGURE src=image/expressen.png?w=900]
[Expressen](https://www.expressen.se/)
Expressen kan försöka hålla sina serversvar-tiden lägre genom att optimera servern till att jobba så snabbt som möjligt när den hämtar saker från databasen, detta kan göras genom att först kolla vilka saker som tar längst tid för servern att ladda när en sidas innehåll skall visas och därifrån fixa så att de hämtas snabbare. Det finns flera möjliga orsaker till att servern jobbar långsamt och därför flera möjligheter till att förbättras.


[FIGURE src=image/aftonbladet.png?w=900]
[Aftonbladet](https://www.aftonbladet.se/)
Aftonbladet skulle spara in laddningstiden genom att ta bort  javascript som blockerar när sidan görs, när DOM trädet byggs måste HTML-koden analyseras innan och just nu finns det blockerande javascript kod som gör att processen stannar upp och löser av den koden först där saker måste hämtas innan de kan bli exekverade.


Analys
-----------------------
Alla tre olika webbplatser hade väldigt olika resultat, de hade tre olika grejer som var på topp-saker de måste fixa till med sina sidor. Alla sidor hade dock på topp tre saker att justera sin CSS kod som alternativ till att förbättra sidans laddningstid. Alla sidor kan alltså fixa till så att den främsta delen CSS-kod som behövs för en sida att laddas upp först läses av medan den delen av CSS-koden som behövs för saker man gör efter att man t.ex. klickat någonstans på sidan (t.ex för att komma in på en artikels brödtext) kan komma senare. Detta var Dagens Nyheters främsta sak som kunde förbättras, medan Aftonbladet hade blockerande javascriptkod och även långsamma servertider precis som expressen.

Sämst betyg får Aftonbladet då de enligt PageSpeed har absolut sämst betyg och flest saker som kan förbättras medans dagens nyheter hade bäst betyg och minsk antal saker som kan förbättras, dock har även Dagnes Nyheter minst storlek på sin sida medan Expressen har störst storlek.

Jag tycker att 4 sekunder är gränsen för en snabb långsam och vid 10 sekunder tycker jag den blir långsam samtidigt som man förstår att en sida med mycket innehåll självklart tar längre tid att ladda om för att visa allt det innehållet. Detta gör alltså att ingen av sidorna klarade min gräns, men det betyder inte att de får dåliga betyg eftersom det är webbplatser med mycket innehåll som måste laddas, men enligt mig är de inte snabba webbplatser.


Övrigt
-----------------------

Isabella Carrera heter jag och jag gjorde denna uppgift själv.
