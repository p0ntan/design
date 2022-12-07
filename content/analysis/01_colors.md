---
Title: Färg
Description: Analysis of colors on different websites.
Template: index
---

Färg och typsnittsanalys
=======================

Analys av färg och färgscheman på tre stycken webbplatser, både nationella och internationella. 

Urval
-----------------------

Urvalet av de använda hemsidorna ses nedan, följt av förklaring till varför just dessa valdes.

1. https://www.skysport.se/<br>
Valet gjordes baserat på mitt egna intresse av skärmflygning, och jag valde därmed Skysport som är en svensk skärmflygskola.

2. https://www.expressen.se/<br>
Den mest besökta svenska hemsidan 2020 [1]

3. https://www.amazon.com<br>
Den populäraste hemsidan för detaljhandel i världen [2]

Urvalet gjordes på hemsidor som alla finns i Sverige, och som alla faller inom olika kategorier såsom sport, nyheter och shopping.

Metod
-----------------------
### Färg
För varje hemsida så togs en printscreen "above-the-fold". "Above-the-fold" är vad man möts av direkt på respektive webbplats startsida utan att man scrollar nedåt på webbplatsen. En adblocker [3] har använts för att reklam från externa webbplatser inte skall synas på respektive webbplats, detta för att minimera innehåll från externa källor. För att hålla antalet färger nere valdes endast färger som var i respektive webbplats header, footer eller navbar, och som även återkommer på webbplatsernas main-del (fotografier är inte inkluderade). Verktyget ColorZilla [4] har använts för att få fram färgernas HEX-värde, som sedan jämförts med HEX-värdet man finner under fliken "Style" i DevTools. Adobes färghjul [5] används sedan för att visuellt visa hur färgerna sitter på ett färghjul i förhållande till varandra.

### Typsnitt
För att se vilka typsnitt som läses in av sidan används fliken "Network" i webbläsarens DevTools. För att se vilken font som används till vilken typ av text används fliken "Computed", där man kan själv välja vilket element på sidan man önskar se de uträknade värdena för. Väljer där önskat element, t ex &#60;p&#62; eller &#60;h1&#62; och ser efter värdet på font-family.

Resultat
-----------------------
### 1. skysport.se <small>(besökt 26/11-2022)</small>

<div class="color-container">
    <img src="%base_url%/image/01_colors/skysport.png" alt="Startsida till skysport.se">
    <table style="border-spacing: 4px; border-collapse: separate">
    <tr>
    <td style="height: 50px; width: 50px; background-color: #0072BC">#0072BC
    <td style="height: 50px; width: 50px; background-color: #3360AE">#3360AE
    <td style="height: 50px; width: 50px; background-color: #3e6296">#3E6296
    <td style="height: 50px; width: 50px; background-color: #234176">#234176
    </tr>
    </table>
    <img src="%base_url%/image/01_colors/skysport-wheel.png" alt="skysport.se färghjul">
</div>

Webbplatsen använder sig utav ett monokromatiskt färgschema då alla färger är i någon nyans av blå. Sidan använder sig inte utav någon accentfärg. Stor del av webbplatsen har en vit bakgrundsfärg.

<table class="font-table">
<tr>
    <th></th>
    <th>h1</th>
    <th>h2</th>
    <th>h3</th>
    <th>p</th>
</tr>
<tr>
    <td>Typsnitt</td>
    <td>Open Sans</td>
    <td>Montserrat</td>
    <td>Open Sans</td>
    <td>Roboto</td>
</tr>
<tr>
    <td>Serif/sans-serif</td>
    <td>Sans-serif</td>
    <td>Sans-serif</td>
    <td>Sans-serif</td>
    <td>Sans-serif</td>
</tr>
</table>

Webbplatsens färgval tillsammans med typsnittet ger hemsidan ett stilrent utseende och en känsla av frihet/öppenhet, vilket troligen är webbplatsens intention.

### 2. expressen.se <small>(besökt 26/11-2022)</small>

<div class="color-container">
    <img src="%base_url%/image/01_colors/expressen.png" alt="Startsida till expressen.se">
    <table style="border-spacing: 4px; border-collapse: separate">
    <tr>
    <td style="height: 50px; width: 50px; background-color: #e30613">#E30613
    <td style="height: 50px; width: 50px; background-color: #fdf001" class="darker-font">#FDF001
    <td style="height: 50px; width: 50px; background-color: #0976b5">#0976b5
    </tr>
    </table>
    <img src="%base_url%/image/01_colors/expressen-wheel.png" alt="expressen.se färghjul">
</div>

Webbplatsen använder sig av ett triadiskt färgschema och saknar accentfärg. Däremot används den röda färgen #E30613 på olika element dit en besökares uppmärksamhet kan riktas. Stor del av webbplatsen har en vit bakgrundsfärg.

<table class="font-table">
<tr>
    <th></th>
    <th>h1</th>
    <th>h2</th>
    <th>h3</th>
    <th>p</th>
</tr>
<tr>
    <td>Typsnitt</td>
    <td>Siri</td>
    <td>Siri</td>
    <td>Siri</td>
    <td>Arial</td>
</tr>
<tr>
    <td>Serif/sans-serif</td>
    <td>Sans-serif</td>
    <td>Sans-serif</td>
    <td>Sans-serif</td>
    <td>Sans-serif</td>
</tr>
</table>

Webbplatsens färgval och typografi ger en lättläst webbplats som håller en besökare uppmärksam med sitt triadiska färgschema, vilket troligen är sidans intention då det är en nyhetssida.

### 3. amazon.com <small>(besökt 26/11-2022)</small>

<div class="color-container">
    <img src="%base_url%/image/01_colors/amazon.png" alt="Startsida till amazon.com">
    <table style="border-spacing: 4px; border-collapse: separate">
    <tr>
    <td style="height: 50px; width: 40px; background-color: #131A22">#131A22</td>
    <td style="height: 50px; width: 40px; background-color: #232F3E">#232F3E</td>
    <td style="height: 50px; width: 40px; background-color: #37475A">#37475A</td>
    <td style="height: 50px; width: 40px; background-color: #FFD814" class="darker-font">#FFD814</td>
    <td style="height: 50px; width: 40px; background-color: #febd69" class="darker-font">#FEBD69</td>
    </tr>
    </table>
    <img src="%base_url%/image/01_colors/amazon-wheel.png" alt="amazon.com färghjul">
</div>

Webbplatsen använder sig utav ett komplement färgschema med accentfärgerna #FEBD69 och #FFD814. Även den röda färgen #CC0C39 används för olika rabatterbjudanden.

<table class="font-table">
<tr>
    <th></th>
    <th>h1</th>
    <th>h2</th>
    <th>h3</th>
    <th>p</th>
</tr>
<tr>
    <td>Typsnitt</td>
    <td>Amazon Ember</td>
    <td>Amazon Ember</td>
    <td>Amazon Ember</td>
    <td>Amazon Ember</td>
</tr>
<tr>
    <td>Serif/sans-serif</td>
    <td>Sans-serif</td>
    <td>Sans-serif</td>
    <td>Sans-serif</td>
    <td>Sans-serif</td>
</tr>
</table>

Webbplatsens färgschema ihop med valt typsnitt ger en lugn känsla, där man kan rikta en besökares uppmärksamhet till olika delar av webbplatsen med accentfärger vilket är troligt med tanke på att amazon är en sida för handel.

Analys
-----------------------

Alla webbplatser som jag använt mig utav i analysen använder sig av någon form av blå färg. Två av sidorna, Amazon och Skysport, använder sig av någon nyans av blå som grundfärg där Amazon även använder sig utav komplement färger. Då blåa färger ger en känsla av lugn och trygghet är det mycket rimligt att man vill använda sig av den som en grundfärg, då det ger sin webbplats en känsla av lugn. Skysports val av blå färg hänger troligtvis ihop med att flygsport är förknippat med en blå himmel, vilket gör det naturligt att välja en grundfärg som återspeglar himlen på sin webbplats. Man hade kunnat använda sig av en komplementfärg för att rikta en besökares uppmärksamhet till önskade delar av sidan som t ex boka kurs eller boka tandem.

Amazon använder sig av en mörkare nyans av blå som grundfärg, för att sedan rikta en besökares uppmärksamhet till olika rabatter, sökfält eller andra klickbara element med hjälp av komplementfärger. Även om det är mycket innehåll på själva sidan ger färgvalet trots allt ett relativt lugnt och samlat intryck.

Expressens webbplats ger inte samma känsla av lugn som de andra sidorna i analysen, även om den använder sig utav en blå färg. Detta är troligen då de använder sig av ett triadiskt färgschema där de använder sig mer utav en röd färg, som är en starkare färg och kan framkalla olika typer av känslor. På så sätt borde en besökare kunna hållas mer alert vid ett besök på hemsidan, samt att man kan rikta uppmärksamheten hos besökaren dit man önskar med att använda sig utav den röda färgen.

Ang typsnitt är det värt att notera är att alla de besökta webbplatserna använder sig av olika typsnitt men där alla är utav typen sans-serif.

Alla webbplatsers färgscheman verkar vara väl framarbetade och utvalda för sitt syfte, vilket man ändå förväntar sig utav såpass stora hemsidor som amazon och expressen. 

Referenser
-----------------------

1. https://computersweden.idg.se/2.2683/1.738698/sverige-mest-trafik-google (Besökt 2022-11-24)
2. https://www.statista.com/statistics/274708/online-retail-and-auction-ranked-by-worldwide-audiences/ (Besökt 2022-11-24)
3. https://getadblock.com/sv/
4. https://www.colorzilla.com/
5. https://color.adobe.com/sv/create/color-wheel

Övrigt
-----------------------

Arbetet för denna analys har gjorts helt självständigt av mig, Pontus Åkerberg.
