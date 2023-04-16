# Kartografia internetowa
Materiały do zajęć z przedmiotu Kartografia Internetowa (KI). 

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
2. **Zaawansowane edycja stylu mapy i dodawanie własnych danych**
   - zaawansowana edycja stylu przy pomocy warstw
   - dodawanie własnych danych i tworzenie zestawu kafelków
   - metody wizualizacji danych w Mapbox
   - import danych: formaty i wymogi
   - tworzenie i edycja danych przy pomocy [Edytora Mapbox](https://studio.mapbox.com/datasets/)
   - **Zadanie 2** - *Stwórz mapę pokazującą rozkład wskaźnika feminizacji na przykładzie Poznania. Wykorzystaj wizualizację 3D. Użyj [zestawu danych demograficznych dla Poznania]()* 

## Dane przykładowe

?MPZP?

## Publikacja mapy w internecie - serwisy hostingowe
Na pewno w jakimś momencie trzeba stworzona mapę udostępnić publicznie. Do tego potrzebne jest miejsce na serwerze (hosting). Istnieje wiele platform, które umożliwiają darmowy hosting, jednak trzeba być ostrożnym (np. niechciane reklamy) i nie wszystkie są przyjazne dla użytkownika. Osobiście na początek polecam dwa sposoby publikacji:

1. [GitHub Pages](https://pages.github.com/) - bardzo prosty i elastyczny sposób publikacji strony w repozytorium GitHub (takiego jak to)
2. [Gitch](https://glitch.com/) - darmowe konto umożliwiające nie tylko publikacje statycznej strony ale i testowanie budowy aplikacji sieciowych 


## Alternatywne oprogramowanie
Mapbox został wybrany dlatego, że jest w miarę zamknięty rozwiązanie i do stworzenia czytelnej mapy o podstawowej funkcjonalności nie wymaga znajomości żadnego języka programowanie. Ale jeśli chcesz czegoś więcej to wystarczą podstawy Javascript, HTML i CSS a świat map internetowych stoi otworem. Podstawy tych trzech rzeczy potrzebne są również w przypadku wykorzystania Mapboxa w bardzije zaawansowany sposób. Alternatywne dla Mapboxa sposoby tworzenia map internetowych (w przypadkowej kolejności):

1. [Leaflet](https://leafletjs.com/) - jedna najpoularnieszyj bibliotek mapowych. Łatwa w implementacji, wiele rozszerzeń i integracji z oprogramowaniem GIS i nie tylko np.:
   - QGIS + [qgis2web plugin](https://plugins.qgis.org/plugins/qgis2web/) - przyjazna dla użytkownika wtyczka, pozwalająca na eksport projektu QGIS zarówno w postaci mapy wykonanej w Leaflet jak i w OpenLayers (patrz niżej)
   - R + [biblioteka Leaflet](https://rstudio.github.io/leaflet/) bardzo ciekawa opcja dla osób pracujących w środowisku programistycznym R
2. [ArcGIS Online](https://www.arcgis.com/index.html) - właśnościowa platforma umożliwiająca publikowanie map na wielu różnych sposobów (np. Story Maps), również za darmo w ograniczonym zakresie. Zaawansowane możliwości w połączniu z oprogramowanie ArcGIS/
3. [OpenLayers](https://openlayers.org/) - bardzo rozbudowana i bardzo dobrze opisana platforma mapowa, alternatywa dla Leaflet (choć wymaga nieco wiekszych umiejętności programistycznych)
4. [MapLibre](https://maplibre.org/) - Open Source wersja bibliotek programistycznych Mapbox GL JS. Jeśli nie są potrzebne usługi Mapbox takie jak Studio a celem jest stworzenie czytelnej i funkcjonalne mapy na strone to przy posiadaniu znajomości Javascript warto sie zainteresować bezpłatną alternatywą.


## Do poczytania
