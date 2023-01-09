---
Title: Design och webbplatser
Description: Analysis of my Art Ist project.
Template: index
---

Laddningstider
=======================

I denna rapport har laddningstider för mitt projekts webbplats till Art Ist samlats in för att se hur webbplatsen presterar samt om det finns några saker som kan förbättras.

Urval
-----------------------

Det har samlats in data från både det ordinarie temat och det optionella temat för att se om det blir någon skillnad. De tre undersidorna som valts ut på varje webbplats är startsidan, about och highlights.

Metod
-----------------------

För att samla in data om de olika webbplatserna användes PageSpeed Insights [1] som mäter, analyser och rapporterar webbplatsens prestanda både på desktop och mobil. I webbläsaren Firefox DeveloperEdition används även det inbyggda DevTools, och mer specifikt fliken "Nätverk/network" för att kunna få fram data om laddningstider, överförd storlek och antal laddade resurser. För varje tema laddas de tre valda sidorna in tre gånger, och sedan räknas medelvärdet ut från de tre mätningarna.

Resultat
-----------------------

### Ordinarie tema

<picture class="picture">
    <source media="(max-width: 450px)" srcset="%base_url%/image/11_eget/projekt-printscreen.jpg?w=600">
    <img src="%base_url%/image/11_eget/projekt-printscreen.jpg?w=1200" alt="Art Ist grundtemas startsida">
</picture>

### Optionellt tema

<picture class="picture">
    <source media="(max-width: 450px)" srcset="%base_url%/image/11_eget/projekt-printscreen-2nd.jpg?w=600">
    <img src="%base_url%/image/11_eget/projekt-printscreen-2nd.jpg?w=1200" alt="Art Ist grundtemas startsida">
</picture>

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRH0U5F9i3SpnYjen8WS2AMqkIpOjU7iKyUzTO0ygA5Fm4ONJBLjyEBkh5XenhlEhI01Kao4RYhks-7/pubhtml?gid=1495198024&amp;single=true&amp;widget=true&amp;headers=false" title="Art Ist data" class="embed-data"></iframe>

Först kan det nämnas att det är en liten skillnad beroende på vilket tema som är aktivt vid mätningarna, men skillnaden är såpass liten den kan man bortse ifrån i sammanhanget.

Sidan DOM-content laddas in på omkring 0.6 sekunder oavsett vilken sida man mäter på. Laddningstiden är sedan på strax under en sekund i snitt och den slutförda strax över en sekund i snitt för alla sidor. Antal resurser som överförs är 19-24 beroende på sida, och överförd data varierar från 0,33-0,66 MB där slutgiltig storlek är något större mellan 0,38-0,77 MB beroende på vilken sida man besöker.

Mätningarna visar ett bra resultat från PageSpeed Insights, där de förslag till förbättring man får är framförallt "ta bort resurser som blockerar renderingen" samt att "skicka bilder i modernare bildformat". Här är det 360 ms som är en möjlig besparing enligt PageSpeed om man skulle ta bort resurser som blockerar renderingen som består av två CSS filer (style samt font-awesome), och ca 100 kB sparad data med modernare bildformat.

Analys
-----------------------

Webbplatsen upplever jag som snabb och med tanke på att det är en stor hero-bild som fyller hela webbläsaren har en en förhållandevis liten mängd överförd data. På about-sidan är det endast logon och hero-bilden som laddas, vilket står för den största delen av den överförda datan. Hero-bilden skulle man kunna jobba med ännu mer, men då den endast har en storlek på 0,128-0,188 MB i mätningarna så är det trots allt lite begränsat hur mycket mer man kan komprimera en såpass stor bild utan att börja tappa för mycket kvalité.

Resultatet från PageSpeed Insights är också bra där det i nästan alla mätningar får ett betyg över eller strax under 90 av 100. Prestandan är något lägre för mobiler, men från tidigare analyser är erfarenheten att det många webbplatser presterar sämre på just den punkten [2]. Här skulle man kunna jobba mer med att "ta bort resurser som blockerar renderingen", men den möjliga besparingen här är totalt 360 ms och sett till helheten så skulle det troligen inte förändra upplevelsen för en besökare. Man skulle även kunna byta till ett modernare bildformat, men då t ex .webp inte fungerar i alla webbläsare (bl a äldre versioner av Safari) så anser jag att besparingen inte är värd risken att webbplatsen slutar fungera som tänkt i detta tillfället.

Man skulle kunna jobba med modernare bildformat och samtidigt ha en fallback till ett .jpg format, men besparingen anser jag är för liten på just denna webbplatsen. Man skulle också kunna byta ut hero-bilden på det optionella temat till en .svg bild, men även här är den förväntade besparingen begränsad samt att jag upplevt problem att använda mig just utav .svg filer i utvecklingsmiljön.

Slutsats
-----------------------

Under skapandeprocessen av denna webbplats märks det att man tänkt på vad som kan vara resurskrävande vid en inladdning av webbplatsen. Sidan är snabb och presterar bra jämfört med tidigare analyser som genomförts på liknande sätt [2]. Det finns absolut saker man kan förbättra, men det är begränsat hur stor skillnad det kan bli och därmed kanske inte värt att lägga allt för mycket tid på. I den tidigare analysen sattes min personliga "absoluta laddningstid" till 5 sekunder, och Art Ist webbplats hamnar långt under den gränsen.

Referenser
-----------------------

1. https://pagespeed.web.dev/ (besökt 2023-01-06)
2. https://www.student.bth.se/~poak22/dbwebb-kurser/design/me/portfolio/analysis/02_load (besökt 2023-01-06)

Övrigt
-----------------------

Rapporten är gjord helt självständigt av mig, Pontus Åkerberg.
