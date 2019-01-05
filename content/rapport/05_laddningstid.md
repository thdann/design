---
---

Analys: laddningstid och användbarhet
=======================

Uppgiften gick ut på att analysera, utvärdera och jämföra tre olika webbplatser i form av laddningstid och användarbarhet.

Urval
-----------------------

Jag fortsatte på resespåret och valde i detta kursmoment att analysera tre webbplatser som säljer vandringsresor. Jag googlade rätt och slätt "vandringsresor" och tog de tre första träffarna (som inte var annonser) och det var följande webbplatser:

[Prima Travel](https://www.primatravel.com/vandringsresor)
[Temaresor](https://www.temaresor.se/resa/vandringsresor/)
[Wiresor](https://www.wiresor.se/vandringsresor)

Metod
-----------------------

Webbplatsernas laddningstid analyserades med [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/), resultatet presenteras som desktop/mobil i tabellerna nedan, samt Google Chrome och DevTools.

Vid analysen med DevTools laddades varje sida om tre gånger och det är ett snitt av de tre laddningstiderna som presenteras i resultatet.

Resultat
-----------------------
[FIGURE src=image/primatravel.png&fill-to-fit caption="Startsida för primatravel.com"]

<table>
<tr><th>Sida</th><th>PageSpeed</th><th>Requests</th><th>Storlek</th><th>Laddningstid</th></tr>
<tr><td><a href="https://www.primatravel.com/vandringsresor">Prima Travel start</a></td>
<td>93/53</td><td>55</td><td>2,90MB</td><td>3,11s</td></tr>

<tr><td><a href="https://www.primatravel.com/alpina-expeditioner">Prima Travel Alpina expeditioner</a></td>
<td>94/78</td><td>47</td><td>941,33KB</td><td>2,98s</td></tr>

<tr><td><a href="https://www.primatravel.com/vandring-i-kappadokien">Prima Travel Kappadokien</a></td>
<td>93/76</td><td>66</td><td>1,73MB</td><td>3,35s</td></tr>
</table>

Prima Travel har hastighetsbetyg på över 90 för desktop och låga laddningssiffror jämfört med de andra sidorna, däremot skulle de kunna förbättra sin webbplats i förhållande till mobila enheter.

[FIGURE src=image/temaresor.png&fill-to-fit caption="Startsida för temaresor.se"]

<table>
<tr><th>Sida</th><th>PageSpeed</th><th>Requests</th><th>Storlek</th><th>Laddningstid</th></tr>
<tr><td><a href="https://www.temaresor.se/resa/vandringsresor/">Temaresor vandring start</a></td>
<td>86/36</td><td>109</td><td>2,60MB</td><td>22,31s</td></tr>

<tr><td><a href="https://www.temaresor.se/resor/europa/schweiz/vandring-i-fyra-lander/">Temaresor vandring i fyra länder</a></td>
<td>80/37</td><td>108</td><td>2,73MB</td><td>19,48s</td></tr>

<tr><td><a href="https://www.temaresor.se/resor/europa/frankrike/vinvandring-i-alsace-och-champagne/">Temaresor Vinvandring Frankrike</a></td>
<td>97/40</td><td>93</td><td>2,70MB</td><td>22,49s</td></tr>
</table>

Temaresor har lägst hastighetsbetyg av de tre webbplatserna och speciellt låga betyg för mobila enheter. Sidorna är inte de största men däremot väldigt långa laddningstider jämfört med de andra webbplatserna så där finns stora förbättringsmöjligheter.

[FIGURE src=image/wiresor.png caption="Startsida för wiresor.se"]

<table>
<tr><th>Sida</th><th>PageSpeed</th><th>Requests</th><th>Storlek</th><th>Laddningstid</th></tr>
<tr><td><a href="https://www.wiresor.se/vandringsresor">Wi-resor start</a></td>
<td>99/80</td><td>94</td><td>5,3MB</td><td>2,39s</td></tr>

<tr><td><a href="https://www.wiresor.se/destination/italien/resor/gardasjon-vandring">Wi-resor Gardasjön</a></td>
<td>99/70</td><td>106</td><td>8,07MB</td><td>4,60s</td></tr>

<tr><td><a href="https://www.wiresor.se/destination/usa/resor/utah-colorado-vandring">Wi-resor Utah och Colorado</a></td>
<td>96/39</td><td>169</td><td>15,13MB</td><td>10,94s</td></tr>
</table>

Wiresor har mycket bra hastighetsbetyg för desktop men sämre för mobil. De har varierande laddningstider och storleken på sidorna är rätt mycket större än de andra webbplatserna. Ett förbättringsförslag skulle kunna vara att minska storleken genom att jobba om åtminstone de största bilderna. På en av de tre sidorna fanns bilder uppåt 1MB.

Analys
-----------------------

1. Primatravel - snabbast laddningstide och bäst betyg på PageSpeed sett till desktop och mobil sammanslaget.
2. Wiresor - långa laddningstider men förklarligt med tanke på stor storlek. Bäst betyg på PageSpeed sett till enbart desktop.
3. Temaresor - långa laddningstider i förhållande till storleken, dessa har mest att jobba på. Lägsta betyg på PageSpeed både för desktop och mobil var för sig men också sammanslaget.

Primatravel har snabbast laddningstider vilket förmodligen förklaras av att de också har minst storlek och inte riktigt lika många requester som de andra. Wiresor hade aningen längre laddningstider och även största storleken samt många requests, genom att minska storleken på sidorna skulle förmodligen laddnigstiderna också gå ner. Den största delen av storleken beror på bilderna. Den absolut största sidan i analysen var Wiresors sida om vandringar i Colorado och Utah, på den sidan var det många bilder som var över 500KB och ända upp till 1MB, vilket inte fanns på de andra sidorna så i synnerhet där kan de jobba om bilderna för att minska storleken. Temaresor hade extremt långa laddningstider i förhållande till både requests och storlek jämfört med de andra.

Förslag från PageSpeed på i princip samtliga webbplatser var  att skicka bilderna i modernare format samt koda bilderna effektivt. Detta gällde för både desktop och mobil. Temaresor fick även som förslag att skjuta upp inläsning av bilder som inte visas på skärmen, vilket jag antar då är en del av förklaringen till de långa laddningstiderna eftersom jag jämförde också storleken på bilderna på Temaresors och Wiresors startsida och där de var ungefär lika stora på båda webbplatserna.

Jag anser att en snabb sida laddas på ett par sekunder men kan även tycka att uppåt fem-sex sekunder också är snabbt. Jag hinner ju ändå inte leta fram exakt info jag söker snabbare än så. För den här uppgiften störde de längre laddningstiderna inte mig, eftersom jag inte var ute efter att hitta exakt information på själva sidan, men hade jag varit ute efter att leta information så hade jag nog blivit lite otålig när laddningstiden är över 20 sekunder. Speciellt på mobilen då jag ofta vill hitta någon specifik information när jag surfar mobilt.


Referenser
-----------------------
[Rådata](https://docs.google.com/spreadsheets/d/1_5eTg4k9iBVA3EvQuSCOPJr6hUnmw3x2bbXSRfuszbU/edit?usp=sharing)


Övrigt
-----------------------

Theresa Dannberg
