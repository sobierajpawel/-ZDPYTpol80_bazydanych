# Zadanie 1

### Zapytania DML - SELECT 

1) Utwórz nową bazę danych i wywołaj skrypt.

https://www.dropbox.com/s/950twvsg9065ulu/export_db.sql?dl=0

2) Zbuduj zapytania SELECT:

   - Pobierz wszystkie rekordy z tabeli `city`
   - Pobierz rekord z tabeli `city` gdzie nazwa miast jest równa `Moscow`
   - Pobierz wszystkie miasta zaczynające się na literę `A`
   - Pobierz wszystkie miasta kończące się na litery `at`, posortuj je malejąco po `city_id`
   - Pobierz tylko nazwę miasta zamiast całego rekordy dla dowolnego warunku.
  
3) Zapytania grupujące

   - Pobierz miasta z tabeli `city` gdzię nazwa miasta jest równa `London`
   - Pozbądź się duplikatu za pomocą zapytania GROUP BY
   - Pozbądź się duplikatów za pomocą zapytania DISTINCT

4) Zbuduj zapytania agregujące:

   -  Zbuduj zapytanie wyliczające średnią długość filmu z tabeli `film` dla ratingu `PG-13`
   -  Zbuduj zapytanie pokazujące minimalną długość oraz maksymalną długość (zmień nazwy kolumn) dla rating `PG-13` lub `PG`
   -  Zbuduj zapytanie pokazujące sumę długości filmów dla rating `PG-13` lub `PG`
   -  Zbuduj zapytanie pokazujące ilość filmów dla rating `PG-13` lub `PG`

5) Zbuduj zapytanie łączące:

   - Zbuduj zapytanie łączące tabele `city` oraz `county` wyświetl miasta oraz nazwę państw dla krajów = `Poland`, `Australia`, `France`
   - Zbuduj zapytanie łączące kategorie z filmami wyświetl tylko i wyłączeni film oraz nazwę kategorii

