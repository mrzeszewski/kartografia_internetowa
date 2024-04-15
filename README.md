Materiały do zajęć z przedmiotu **Kartografia Internetowa (KI).** 

## Dlaczego KI?
W trakcie kursu będziemy zapoznawać się z technikami publikacji informacji przestrzennej w postaci dynamicznych map internetowych. Istnieje bardzo wiele powodów, dla których ta forma publikacji jest właściwie dominująca - wygoda, możliwość udostępniania szerokiemu gronu odbiorców, dynamiczna treść, możliwość integracji z platformami i usługami internetowymi (chociażby geolokalizacja użytkownika) czy wreszcie dostępność szerokiego spoektrum narzędzi kartograficznych. Popularność kartografii internetowej spowodowała powstanie licznych rozwiązan technicznych - celem tego kursy jest przedstawienie jednego z nich. Namacalnym efektem będzie stworzenie mapy internetowej i publikacja jej w sieci.   


## Tematyka zajęć
Poniższa lista przedstawia skróconą wersję tego co obejmuje każdy blok zajęć, wraz z niezbędnymi materiałami i linkami do dodatkowych treści. 

1. **Wprowadzenie do [Platformy Mapbox](https://www.mapbox.com/) i tworzenie stylu mapy**
   - rejestracja konta (wymagany mail z domeny uniwersyteckiej)
   - struktura danych przestrzennych w Mapbox: zestawy danych, kafelki, style.
   - interfejs użytkownika, [tutoriale](https://docs.mapbox.com/help/tutorials/), [przykłady](https://docs.mapbox.com/mapbox-gl-js/example/), [dokumentacja](https://docs.mapbox.com/), 
   - [Mapbox Studio](https://studio.mapbox.com/) - dostępne zasoby, stylizacja mapy przy pomocy komponentów
   - **Zadanie 1** - *stwórz własny spójny wizualnie styl, zmieniając właściwości komponentów. Udostepnij w formie podglądu (preview)* 
2. **Edycja stylu mapy przy pocy warstw i dodawanie własnych danych**
   - zaawansowana edycja stylu przy pomocy warstw
   - dodawanie własnych danych i tworzenie zestawu kafelków
   - metody wizualizacji danych w Mapbox
   - import danych: formaty i wymogi
   - tworzenie i edycja danych przy pomocy [Edytora Mapbox](https://studio.mapbox.com/datasets/)
   - publikacja podglądu mapy
   - **Zadanie 2** - *Stwórz mapę pokazującą rozkład wskaźnika feminizacji na przykładzie Poznania. Wykorzystaj wizualizację 3D. Użyj [zestawu danych demograficznych dla Poznania](https://raw.githubusercontent.com/mrzeszewski/kartografia_internetowa/main/dane/demography_poznan.geojson)*
3. **Zaawansowana stylizacja warstw**
   - stylizacja warstw liniowych i punktowych
   - stylizacja zależna od danych
   - mapy ciepła
   - grupy warstw
   - ikony i czcionki
   - style zależne od skali
4. **Publikacja mapy przy pomocy strony internetowej - Mapbox GL JS**
   - tworzenie własnej strony z mapą internetową na podstawie [przykładu prostej mapy Mapbox](https://docs.mapbox.com/mapbox-gl-js/example/simple-map/)
   - struktura strony internetowej (CSS, HTML)
   - podstawy skryptów Javascript
   - narzędzia developerskie przeglądarki
   - wprowadzenie do biblioteki Mapbox GL JS
   - **Zadanie 3** - *Opublikuj własny styl w postaci strony internetowej - pliku html*
5. **Dodawanie funkcji interaktywnych do mapy**
   - dodawanie funkcji interaktywnych do mapy - [przykład z popupami](https://docs.mapbox.com/mapbox-gl-js/example/popup-on-click/)
   - przełączanie warstw mapy przy pomocny funkcji Javascript - [przykład](https://docs.mapbox.com/mapbox-gl-js/example/toggle-layers/)
6. **Zadanie zaliczeniowe**
   - **Zadanie 4 - końcowy projekt** - *Zadanie w grupach 1-2 osoby. Stwórz i opublikuj własną stronę internetową zawierającą mapę na wybrany temat. Wykorzystaj dowoolne dane poza używanymi na zajęciach. Oceniane będzie część kartograficzna (czytelność, dobór kolorów i symboli, hierarchia wizulalna etc.) oraz część funkcjonalna (stopień interaktywności, dodane funkcje). *

## Sample data

1. [Voivodships (file poland_voivodships.geojson)](https://raw.githubusercontent.com/mrzeszewski/kartografia_internetowa/main/dane/poland_voivodships.geojson)
_Provincial boundaries and sample attribute data._
2. [Demographic data for Poznań (demography_poznan.geojson file)](https://raw.githubusercontent.com/mrzeszewski/kartografia_internetowa/main/dane/demography_poznan.geojson)
_2011 Census data: Grid with population, age and gender._
3. [Natural monuments in Poznań (natural_monuments.csv file](https://raw.githubusercontent.com/mrzeszewski/kartografia_internetowa/main/dane/natural_monuments.csv)
_Natural monuments near Poznań from GDOŚ - CSV format_
4. [Natural monument marking icon (file natural_monument.svg](https://raw.githubusercontent.com/mrzeszewski/kartografia_internetowa/main/dane/natural_monument.svg)
_Icon in SVG format_
5. [Data from bicycle counters for Poznań (file dzienniki_rowerowe_Poznan_21032024.geojson](https://raw.githubusercontent.com/mrzeszewski/kartografia_internetowa/main/dane/liczniki_rowerowe_Poznan_21032024.geojson)
_Icon in SVG format_
6. [Value of car noise emission in Poznań - LN index (halas_zdrowie_LN.geojson file)](https://raw.githubusercontent.com/mrzeszewski/kartografia_internetowa/main/dane/halas_zdrowie_LN.geojson)
_Icon in SVG format_

## Publication of the map on the Internet - hosting services
Certainly, at some point the created map must be made publicly available. For this you need space on the server (hosting). There are many platforms that allow free hosting, but you have to be careful (e.g. unwanted ads) and not all of them are user-friendly. Personally, I recommend two ways of publishing to start with:

1. [GitHub Pages](https://pages.github.com/) - a very simple and flexible way to publish a page to a GitHub repository (like this)
2. [Gitch](https://glitch.com/) - a free account that allows not only publishing a static website but also testing the construction of web applications


## Alternative software
Mapbox was chosen because it is a relatively closed solution and does not require knowledge of any programming language to create a readable map with basic functionality. But if you want something more, all you need are the basics of Javascript, HTML and CSS and the world of web maps is open to you. The basics of these three things are also needed when using Mapbox in a more advanced way. Alternative ways to create web maps for Mapbox (in no particular order):

1. [Leaflet](https://leafletjs.com/) - one of the most popular map libraries. Easy to implement, many extensions and integrations with GIS software and more, e.g.:
    - QGIS + [qgis2web plugin](https://plugins.qgis.org/plugins/qgis2web/) - a user-friendly plugin that allows you to export a QGIS project both as a map made in Leaflet and in OpenLayers (see below)
    - R + [Leaflet library](https://rstudio.github.io/leaflet/) a very interesting option for people working in the R programming environment
2. [ArcGIS Online](https://www.arcgis.com/index.html) - a proprietary platform that allows you to publish maps in many different ways (e.g. Story Maps), also for free to a limited extent. Advanced capabilities combined with ArcGIS/
3. [OpenLayers](https://openlayers.org/) - a very extensive and very well described mapping platform, an alternative to Leaflet (although it requires slightly more programming skills)
4. [MapLibre](https://maplibre.org/) - Open Source version of the Mapbox GL JS programming libraries. If you do not need Mapbox services such as Studio and the goal is to create a clear and functional map for the website, if you have knowledge of Javascript, it is worth considering a free alternative.


## To read

1. [W3Schools HTML Course](https://www.w3schools.com/html/)
2. [W3Schools CSS Course](https://www.w3schools.com/css/)
3. [W3Schools Javascript Course](https://www.w3schools.com/js/)
