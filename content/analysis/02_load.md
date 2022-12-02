---
Title: Load
Description: Analysis of websites loadingtimes.
Template: index
---

Laddningstid
=======================

I denna rapport har laddningstider för tre olika hemsidor samlats in och jämförts emot varandra.

Urval
-----------------------

De tre webbplatser som valdes för rapporter är alla nyhetssidor. På nyhetssidor kan bilder och eventuellt videor vara viktiga för att spegla innehållet i olika artiklar, men där själva innehållet i olika artiklar är det mest intressanta. Därför vore det intressant att se hur olika nyhetssidors laddningstid förhåller sig till varandra. Nyhetssidorna som valts är:

1. https://www.svt.se/
<br>En av få, om inte den enda, svenska nyhetstjänsten som inte är direkt finansierad via reklam. 

2. https://www.omni.se
<br>2020 års bästa nyhetssida enligt idg.se [1]. Har även utsetts till bästa nyhetssidan av idg.se tidigare år.

2. https://www.expressen.se/
<br>Den mest besökta svenska hemsidan 2020 enligt ComputerSweden (idg.se) [2]

Metod
-----------------------

För att samla in data om de olika webbplatserna användes PageSpeed Insights [3] som mäter, analyser och rapporterar webbplatsens prestanda både på desktop och mobil. I webbläsaren Firefox DeveloperEdition används även det inbyggda DevTools, och mer specifikt fliken "Nätverk/network" för att kunna få fram data om laddningstider, överförd storlek och antal laddade resurser. Varje webbplats laddas tre olika sidor in tre gånger, och sedan räknas medelvärdet ut från de tre omladdningarna och mätningarna. För respektive webbplats har även varje startsida mäts ytterligare 3 gånger, denna gång med en AdBlocker [4] aktiverad för att se skillnaden när man exkluderar externt innehåll i form av reklam.

Resultat
-----------------------

För respektive webbplats användes startsidan, webbplatsens sportsida samt kultursida för insamling laddningstider, storlek och laddade resurser. 

1. SVT (besökt 2022-12-01)

<picture class="picture">
    <img src="%base_url%/image/02_load/svt-load.webp?w=1000" alt="SVT startsida">
</picture>


<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRH0U5F9i3SpnYjen8WS2AMqkIpOjU7iKyUzTO0ygA5Fm4ONJBLjyEBkh5XenhlEhI01Kao4RYhks-7/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false" class="embed-data"></iframe>

SVT:s nyhetssite laddar de olika sidornas innehåll inom 2-3 sekunder, laddar mellan 40-60 resurser och använder under en MB data vid överföringen vilket gör att alla sidor laddar snabbt och hela sidan är klar ungefär samtidigt. Spontant ser jag ingen anledning till förbättring utöver PageSpeeds förslag att "reducera JavaScript som inte används".

När en AdBlocker aktiverades märktes ingen direkt skillnad förutom en liten ökning i laddtid, men antalet resurser och datamängd var i stort sett oförändrade.

2. Omni (besökt 2022-12-01)

<picture class="picture">
    <img src="%base_url%/image/02_load/omni-load.webp?w=1000" alt="Omni startsida">
</picture>

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRH0U5F9i3SpnYjen8WS2AMqkIpOjU7iKyUzTO0ygA5Fm4ONJBLjyEBkh5XenhlEhI01Kao4RYhks-7/pubhtml?gid=157068620&amp;single=true&amp;widget=true&amp;headers=false" class="embed-data"></iframe>

Omni:s nyhetssite laddar DOM-content relativt fort, oftast under en sekund, men däremot är sidans laddningstid långsammare och där den upplevda laddningstiden (slutförd i tabellerna) är än långsammare. Sidan laddar 132-157 resurser och överför mellan 1,95-3,37 MB data. Då många resurser laddas, därav många bilder, skulle webbplatsen kunna jobba mer med komprimering av bilder för att spara data som behöver överföras till en besökare.

Värt att notera är att med en AdBlocker aktiverad förbättras alla mätvärden förutom laddningstiden för DOM-content, även om det handlar om väldigt kort tid.

3. Expressen (besökt 2022-12-01)

<picture class="picture">
    <img src="%base_url%/image/02_load/expressen-load.webp?w=1000" alt="Expressen startsida">
</picture>

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRH0U5F9i3SpnYjen8WS2AMqkIpOjU7iKyUzTO0ygA5Fm4ONJBLjyEBkh5XenhlEhI01Kao4RYhks-7/pubhtml?gid=1774099255&amp;single=true&amp;widget=true&amp;headers=false" class="embed-data"></iframe>

Expressen:s webbplats laddar sidans DOM-content likt Omni runt en sekund, men där den upplevda laddningstiden är desto långsammare då sidan innehåller mycket externt innehåll. Antal resurser som laddas är mellan 232-245 stk och mängden data som överförs ligger mellan 2,5-3,5 MB. Sett enbart till prestanda skulle en förbättring var att begränsa mängden externt innehåll, men är kanske inte möjligt då detta är en inkomstkälla till webbplatsen.

Likt Omni med en AdBlocker aktiverad förbättras alla mätvärden förutom tiden för DOM-contentet. Värt att notera här är att utan externt innehåll laddas det endast in 36 resurser, en minskning på 200 (!) vilket är en mycket stor skillnad. 

Analys
-----------------------

Analys KOMMER!

Referenser
-----------------------

1. https://topp100.idg.se/2.39772/1.742857/topp-100-2020-nyheter (besökt 2022-12-01)
2. https://computersweden.idg.se/2.2683/1.738698/sverige-mest-trafik-google (Besökt 2022-12-01)
3. https://pagespeed.web.dev/
4. https://adblockplus.org/

Övrigt
-----------------------

Rapporten är gjord helt självständigt av mig, Pontus Åkerberg.
