# Zadanie 3

### Zapytania DDL

Zapytania wykonaj na nowej bazie danych !

1) Napisz zapytanie SQL odpowiedzialne za tworzenie tabeli `companies`, która powinna zawierać kolumny:
  - `id` typu int pole nie powinno być puste - automatyczna inkrementacja, klucz główny
  - `trade` typu varchar z maksymalną długością 40
  - `number_of_employees` typu int
    
Kolumna `id` powinna być jednoznacznym identyfikatorem tabeli. Kolumny `trade` i `number_of_employees` nie powinny zawierać wartości `null`. Kolumna `number_of_employees` powinna być domyślnie ustawiona na 0.


2) Napisz zapytanie SQL odpowiedzialne za tworzenie tabeli `job_offers`, która powinna zawierać kolumny:
  - `id` typu int pole nie powinno być puste - automatyczna inkrementacja, klucz główny
  - `offer_title` typu varchar z maksymalną długością 40 `NOT NULL`,
  - `offer_min_salary` typu decimal,
  - `offer_max_salary` typu decimal,

3) Napisz zapytanie SQL odpowiedzialne za tworzenie tabeli `candidates`, która powinna zawierać pola:
 - `id` typu int pole nie powinno być puste - automatyczna inkrementacja, klucz główny
 - `first_name` typu varchar z maksymalną długością 40 `NOT NULL`,
 - `last_name` typu varchar z maksymalną długością 40 `NOT NULL`,
 - `email` typu varchar z maksymalną długością 30 `NOT NULL`,
 - `phone_number` typu varchar z maksymalną długością 12
 - `job_offer_id` klucz obcy do tabeli `job_offers` 
 - `company_id` klucz obcy do tabeli `companies`
