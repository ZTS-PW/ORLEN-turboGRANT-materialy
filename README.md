# ORLEN turboGRANT – „Energia Kreatywności”

Repozytorium zawiera materiały edukacyjne przygotowane przez **Koło Naukowe „Zrób To Sam” Politechniki Warszawskiej** w ramach projektu **„Energia Kreatywności”**, realizowanego dzięki programowi **ORLEN turboGRANT**.

## O projekcie

„Energia Kreatywności” to projekt edukacyjny oparty na praktycznej nauce nauk technicznych i rozwijaniu zainteresowań inżynierskich wśród uczniów szkół podstawowych i średnich.

W ramach projektu członkowie KN ZTS prowadzili zajęcia i warsztaty dotyczące m.in.:

* elektroniki i podstaw budowy układów elektronicznych,
* Arduino i mikrokontrolerów,
* robotyki,
* energii i odnawialnych źródeł energii,
* modelowania oraz druku 3D.

Uczestnicy mogli samodzielnie budować układy, wykonywać eksperymenty, programować urządzenia oraz tworzyć i testować własne rozwiązania techniczne.

## Materiały w repozytorium

Repozytorium stanowi jeden z trwałych rezultatów projektu i umożliwia dalsze wykorzystywanie przygotowanych materiałów również po zakończeniu prowadzonych warsztatów.

Znajdują się tutaj:

### Scenariusze zajęć z elektroniki

* `Elektronika_scenariusz_1_ORLEN_ZTS.pdf`
* `Elektronika_scenariusz_2_ORLEN_ZTS.pdf`
* `Elektronika_scenariusz_3_ORLEN_ZTS.pdf`

Materiały mogą służyć jako podstawa do samodzielnego przeprowadzenia praktycznych zajęć z elektroniki.

### Druk 3D

* `Instrukcja_druk_3d_ORLEN_ZTS.pdf`

Instrukcja wprowadza uczestników w podstawy przygotowania modeli i realizacji wydruków 3D.

Przed drukowaniem modeli znajdujących się w folderze `modele_3d` zalecamy zapoznanie się z instrukcją.

### Modele 3D

W folderze `modele_3d` udostępniono trzy zestawy modeli:

* `generator` – elementy modelu generatora z ręczną korbą,
* `panel_słoneczny` – elementy ruchomego stanowiska z panelem słonecznym,
* `sygnalizacja` – elementy modelu sygnalizacji świetlnej.

Każdy model został podzielony na kilka plików STL, które należy wydrukować, a następnie połączyć w kompletną konstrukcję.

---

# Jak przygotować modele do druku?

## 1. Wybierz model

Przejdź do folderu:

`modele_3d`

i wybierz jeden z zestawów:

* `generator`,
* `panel_słoneczny`,
* `sygnalizacja`.

Do wykonania kompletnego modelu należy pobrać wszystkie wymagane pliki STL znajdujące się w odpowiednim folderze.

## 2. Otwórz pliki STL

Pliki należy otworzyć w programie typu slicer, np.:

* Bambu Studio,
* PrusaSlicer,
* OrcaSlicer,
* Ultimaker Cura.

Szczegółowe informacje dotyczące przygotowania wydruku znajdują się w:

`Instrukcja_druk_3d_ORLEN_ZTS.pdf`

## 3. Przygotuj wydruk

Przed rozpoczęciem drukowania:

1. zaimportuj wszystkie potrzebne części,
2. sprawdź orientację modeli,
3. w miarę możliwości ustaw największą płaską powierzchnię części na stole,
4. sprawdź w podglądzie, czy model wymaga podpór,
5. pozostaw skalę modelu na poziomie **100%**,
6. nie zmieniaj skali tylko jednej części zestawu – elementy mogą wtedy przestać do siebie pasować.

Do typowych zastosowań edukacyjnych można wykorzystać filament PLA i standardową wysokość warstwy około `0,20 mm`.

## 4. Po zakończeniu drukowania

Przed składaniem:

* usuń podpory,
* oczyść elementy z pozostałości filamentu,
* sprawdź drożność otworów,
* wykonaj próbne dopasowanie części,
* nie wciskaj elementów na siłę.

W przypadku druku FDM niewielkie różnice wymiarowe są normalne. W razie potrzeby otwory lub powierzchnie łączenia można delikatnie oczyścić.

---

# Składanie modeli

## 1. Generator

Folder:

`modele_3d/generator`

Model składa się z trzech drukowanych elementów:

### `ObudowaZoltyV2.stl`

Główna obudowa generatora i podstawa całej konstrukcji.

### `TulejaNaKorbe.stl`

Element łączący mechanizm obrotowy z korbą.

### `KorbaZolty.stl`

Ręczna korba umożliwiająca wprawianie mechanizmu generatora w ruch.

### Kolejność montażu

**Obudowa → Tuleja → Korba**

1. Wydrukuj wszystkie trzy części.
2. Oczyść otwory montażowe.
3. Umieść element generatora lub mechanizmu obrotowego w obudowie.
4. Na osi mechanizmu zamontuj `TulejaNaKorbe.stl`.
5. Do tulei przymocuj `KorbaZolty.stl`.
6. Sprawdź, czy korba może obracać się swobodnie i nie ociera o obudowę.

Model może służyć do demonstracji przemiany energii mechanicznej w energię elektryczną.

---

# 2. Panel słoneczny

Folder:

`modele_3d/panel_słoneczny`

Model składa się z pięciu elementów:

### `spód.stl`

Dolna część konstrukcji. Stanowi podstawę właściwego mechanizmu panelu.

### `środek.stl`

Środkowa część konstrukcji łącząca dolny element z ruchomą częścią modelu.

### `ramię.stl`

Ramię służące do zamontowania i ustawiania ruchomej części konstrukcji.

### `mocowanie.stl`

Element montowany w górnej części konstrukcji. Służy jako mocowanie elementów związanych z panelem i układem śledzenia światła.

### `podstawa (dodatkowo).stl`

Dodatkowa, opcjonalna podstawa zwiększająca stabilność całego stanowiska.

Model można złożyć również bez tego elementu.

## Zalecana kolejność składania

**Podstawa opcjonalna → Spód → Środek → Ramię → Mocowanie**

czyli:

`podstawa (dodatkowo).stl`
↓
`spód.stl`
↓
`środek.stl`
↓
`ramię.stl`
↓
`mocowanie.stl`

### Montaż krok po kroku

1. Wydrukuj:

   * `spód.stl`,
   * `środek.stl`,
   * `ramię.stl`,
   * `mocowanie.stl`.

2. Opcjonalnie wydrukuj również:

   * `podstawa (dodatkowo).stl`.

3. Jeżeli korzystasz z dodatkowej podstawy, rozpocznij montaż od umieszczenia na niej elementu `spód.stl`.

4. Do elementu `spód.stl` zamontuj `środek.stl`.

5. Do środkowej części konstrukcji zamontuj `ramię.stl`.

6. Na odpowiedniej części ramienia zamontuj `mocowanie.stl`.

7. Następnie można zamontować panel słoneczny oraz elementy elektroniczne wykorzystywane w stanowisku.

8. Przed podłączeniem elektroniki sprawdź ręcznie, czy ruchome elementy konstrukcji:

   * nie blokują się,
   * nie ocierają o siebie,
   * mogą zmieniać położenie w wymaganym zakresie.

9. Dopiero po sprawdzeniu mechaniki zamontuj przewody, czujniki oraz pozostałe elementy elektroniczne.

Model może zostać wykorzystany jako stanowisko pokazujące działanie panelu słonecznego oraz układu automatycznego ustawiania panelu względem źródła światła.

---

# 3. Sygnalizacja świetlna

Folder:

`modele_3d/sygnalizacja`

Model składa się z czterech części:

### `PODSTAWA_syg.stl`

Dolna podstawa zapewniająca stabilność konstrukcji.

### `NOGA_syg.stl`

Pionowy element łączący podstawę z właściwą obudową sygnalizatora.

### `CASE_syg.stl`

Główna obudowa sygnalizacji, w której można umieścić elementy elektroniczne.

### `FRONT_syg.stl`

Przednia część zamykająca obudowę sygnalizatora.

## Kolejność montażu

**Podstawa → Noga → Obudowa → Elektronika → Front**

czyli:

`PODSTAWA_syg.stl`
↓
`NOGA_syg.stl`
↓
`CASE_syg.stl`
↓
**montaż elektroniki**
↓
`FRONT_syg.stl`

### Montaż krok po kroku

1. Wydrukuj wszystkie cztery części.
2. Zamontuj `NOGA_syg.stl` w `PODSTAWA_syg.stl`.
3. Na górnej części nogi zamontuj `CASE_syg.stl`.
4. Umieść w obudowie wymagane elementy elektroniczne.
5. Przeprowadź i uporządkuj przewody.
6. Przed zamknięciem obudowy sprawdź działanie elektroniki.
7. Na końcu zamontuj `FRONT_syg.stl`.

Jeżeli model jest wykorzystywany z Arduino i diodami LED, warto uruchomić i przetestować cały układ **przed zamknięciem obudowy**.

---

# Zalecana kolejność pracy

Niezależnie od wybranego modelu warto stosować następującą kolejność:

**1. Pobranie modeli**
↓
**2. Zapoznanie się z instrukcją druku 3D**
↓
**3. Przygotowanie plików w slicerze**
↓
**4. Wydruk elementów**
↓
**5. Usunięcie podpór i oczyszczenie części**
↓
**6. Próbne złożenie konstrukcji**
↓
**7. Montaż elementów elektronicznych**
↓
**8. Test działania**
↓
**9. Ostateczne złożenie modelu**

Nie zalecamy trwałego klejenia elementów przed sprawdzeniem, czy wszystkie części oraz elektronika zostały poprawnie dopasowane.

## Ważne

Modele mają charakter edukacyjny i mogą wymagać niewielkiego dopasowania zależnie od:

* użytej drukarki,
* zastosowanego filamentu,
* ustawień slicera,
* tolerancji wydruku,
* użytych elementów elektronicznych.

Nie należy niezależnie zmieniać skali pojedynczych części należących do tego samego zestawu.

---

## Dla kogo są te materiały?

Materiały zostały przygotowane przede wszystkim z myślą o:

* nauczycielach,
* uczniach,
* szkołach,
* kołach naukowych,
* organizatorach warsztatów technicznych,
* osobach zainteresowanych praktyczną nauką elektroniki i druku 3D.

Zachęcamy do ich wykorzystywania podczas zajęć dydaktycznych, warsztatów oraz własnych projektów.

## Koło Naukowe „Zrób To Sam”

Koło Naukowe „Zrób To Sam” działa na Politechnice Warszawskiej i zajmuje się praktycznymi projektami z obszaru elektroniki, programowania, mikrokontrolerów, robotyki, druku 3D i szybkiego prototypowania.

Jednym z ważnych elementów działalności Koła jest popularyzacja nauk technicznych i przekazywanie wiedzy poprzez praktyczne warsztaty dla uczniów.

## Projekt „Energia Kreatywności”

Projekt został zrealizowany przez **Koło Naukowe „Zrób To Sam” Politechniki Warszawskiej** w ramach programu **ORLEN turboGRANT**.

Materiały powstały podczas przygotowania i realizacji działań edukacyjnych projektu i zostały udostępnione, aby mogły być dalej wykorzystywane przez szkoły, nauczycieli, uczniów i innych zainteresowanych.

## Licencja

Repozytorium jest udostępnione na warunkach licencji **MIT**. Szczegóły znajdują się w pliku `LICENSE`.
