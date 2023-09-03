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

    - zredukuje budżet zapisany w tabeli SalaryBudgets po usunięciu dowolnego rekordu z tabeli Salaries.

```sql
CREATE TABLE Salaries (
    employeeNumber INT PRIMARY KEY,
    salary DECIMAL(10,2) NOT NULL DEFAULT 0
);
CREATE TABLE SalaryBudgets(
    total DECIMAL(15,2) NOT NULL
);
INSERT INTO Salaries(employeeNumber,salary) VALUES
    (1002,5000),
    (1056,7000),
    (1076,8000);
INSERT INTO SalaryBudgets(total) SELECT SUM(salary) FROM Salaries;
```
