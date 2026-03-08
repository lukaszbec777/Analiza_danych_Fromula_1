# Formuła 1 - analiza wyników

W ramach projektu miałem za zadanie przeanalizować historyczne dane Formuły 1 zebrane z serwisu Kaggle, bazujące na API Ergast. Głównym celem analizy było zrozumienie czynników determinujących wyniki kierowców oraz ocena ich efektywności.

## Wstęp i Cel Projektu
Celem niniejszego projektu jest eksploracyjna analiza danych historycznych Formuły 1 w celu zrozumienia czynników determinujących wyniki kierowców, przyczyn nieukończenia wyścigów oraz oceny efektywności poszczególnych zawodników. Analiza koncentruje się na:
- identyfikacji sportowych, technicznych i strategicznych czynników wpływających na wyniki wyścigów,
- zrozumieniu głównych przyczyn DNF i ich wpływu na punktację kierowców oraz niezawodność techniczną zespołów,
- statystycznym określeniu, którzy kierowcy osiągali największą efektywność w historii F1, z uwzględnieniem liczby startów, zdobyczy punktowych i przewagi sprzętowej zespołów.

Projekt wykorzystuje metody statystyczne i wizualizacje danych, aby przekształcić surowe informacje sportowe w czytelne wnioski analityczne, pozwalające na porównania między kierowcami i zespołami oraz ocenę trendów historycznych.


## Pytania badawcze

Pytanie 1. Jakie czynniki determinują wynik kierowcy w wyścigu Formuły 1?
Hipoteza 1: Wynik końcowy kierowcy jest zależny od jednoczesnego wpływu czynników sportowych, technicznych i strategicznych.

Pytanie 2. Jakie są główne przyczyny nieukończenia wyścigów (DNF) w Formule 1 i w jaki sposób wpływają one na punktację kierowców oraz niezawodność techniczną zespołów w sezonie?
Hipoteza 2: Najczęstsze przyczyny DNF — w tym awarie techniczne, incydenty wyścigowe i błędy kierowców — prowadzą do obniżenia dorobku punktowego kierowców oraz ujawniają istotne różnice w niezawodności technicznej poszczególnych zespołów.

Pytanie 3. Czy można statystycznie określić, który kierowca jest najbardziej efektywny w historii Formuły 1?
Hipoteza 3: Najwyższą efektywność osiągają kierowcy charakteryzujący się najwyższym stosunkiem zdobyczy punktowych, zwycięstw i miejsc na podium do liczby startów, po uwzględnieniu przewagi sprzętowej zespołów.

---

## Kluczowe Odkrycia

* **Determinanty Sukcesu:** Stwierdzono, że na wynik końcowy kierowcy wpływają jednocześnie czynniki sportowe, techniczne i strategiczne, a długotrwałą dominację osiągają zespoły łączące stabilność operacyjną z talentem. 
* **Ewolucja Awaryjności:** Przeanalizowano, że historycznie główną przyczyną nieukończenia wyścigów (DNF) były awarie silników, podczas gdy obecnie dominują błędy kierowców i incydenty torowe. 
* **Indeks Efektywności:** Zidentyfikowano Lewisa Hamiltona i Michaela Schumachera jako najbardziej efektywnych kierowców wszech czasów, biorąc pod uwagę ich "gęstość sukcesu" skorygowaną o potencjał maszyny. 


## Tech Stack

| Kategoria | Narzędzia / Pakiety | Cel Użycia |
| :--- | :--- | :--- |
| **Język** | R | Podstawowy język analizy i wizualizacji. |
| **Manipulacja Danymi** | `dplyr`, `tidyverse`, `purrr` | Czyszczenie braków danych, łączenie wielu tabel relacyjnych i transformacja zmiennych. |
| **Wizualizacja** | `ggplot2`, `plotly` | Generowanie statycznych i interaktywnych wykresów. |
| **Formatowanie Tabel** | `gt` | Tworzenie estetycznych i zaawansowanych tabel podsumowujących. |
| **Raportowanie** | Quarto | Generowanie raportu końcowego w formacie HTML z interaktywnymi elementami. |

## Struktura Repozytorium

* `Projekt_Łukasz_Bęc.qmd`: Pełny kod źródłowy analizy i raportu.
* `Katalog dane/`: Zbiór kilkunastu plików CSV użytych do analizy
* `Katalog grafiki/:`: Zbiór plików graficznych wplecionych w treść dokumentu.
* `Projekt_Łukasz_Bęc.html`: Wygenerowany i gotowy do podglądu raport końcowy.


## Jak Odtworzyć Projekt

1.  Sklonuj repozytorium: `git clone [adres Twojego repo]`
2.  Otwórz plik `Projekt_Łukasz_Bęc.qmd` w środowisku RStudio.
3.  Zainstaluj brakujące pakiety R (jeśli to konieczne, użyj komendy `install.packages(c("tidyverse", "ggplot2", "plotly", "purrr", "gt"))`).
4.  Uruchom renderowanie dokumentu (Render to HTML), aby wygenerować ostateczny raport.
