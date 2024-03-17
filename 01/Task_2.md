# Zadanie 2

### Złączenia

1) Wykonaj poniższy skrypt

```sql
ALTER TABLE sakila.city MODIFY COLUMN country_id smallint unsigned NULL;
update city set country_id = null where city_id  in (4,5);
```

2) Napisz zapytanie:

    - będzie zawierał powiązanie tabel `city` oraz `country`, wyświetli nazwę miast oraz nazwę państwa,
      wykorzystaj aliasy tak by kolumna nazwy miasta była wyświetlana jako `nazwa_miasta`, a kolumna 
      reprezentująca nazwę państwa nazywała się `nazwa_kraju` (wykorzystaj `LEFT JOIN`)

    - będzie zawierał wyświetlał informacje o aktorach grających w filmach, wyświetl nazwę filmu oraz imię i nazwisko aktora, zastosuj podobnie jak poprzedniu inne nazwy kolumn

    - będzie wyświetlał dane statystyczny - minimalną, maksymalną, średnią, sumę długości filmów, zgrupowanych wg ratingu

