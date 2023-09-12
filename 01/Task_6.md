# Zadanie 6

### Wyzwalacze

1) Napisz wyzwalacz, który:

    - ustawi aktualny czas w polu `change_date`, oraz wprowadzi dowolne imię w polu `first_name`, wyzwalacz musi działać przed operacją INSERT `BEFORE INSERT`  

```sql
CREATE TABLE employees (
    id INT AUTO_INCREMENT PRIMARY KEY,
    first_name VARCHAR(50) NOT NULL,
    last_name VARCHAR(50) NOT NULL,
    change_date DATETIME DEFAULT NULL
);
```
