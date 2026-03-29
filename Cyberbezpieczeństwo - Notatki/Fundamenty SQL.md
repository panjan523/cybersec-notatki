# Fundamenty SQL

Czym jest baza danych i do czego służy SQL?
Baza danych to zorganizowane miejsce gdzie znajdują się dane użytkowników.

Przykładowo mogą to być hasła, nazwy użytkownika

wygenerowane przez użytkownika rzeczy na social mediach takie jak posty i komentarze.

Rodzaje baz danych.

Relacyjne bazy danych    Nie-relacyjne bazy danych

Relacyjne bazy danych są zorganizowane. Są zachowywane w kolumnach i wierszach.

Jest używana w momentach gdy informacje są rzetelnie otrzymywane w  w spójny sposób.

Nie-relacyjne bazy danych nie sa w postaci tabel.

Są używane gdy dane się znacząco różnią.

Klucze

Dzieli się je na klucze podstawowe i klucze obce

Podstawowe klucze się upewniają że dane w kolumnach są unikatowe. Każda osobna wartość musi być zachowana w tabeli i nie powtarzalna. Każdy musi mieć własny unikatowy identyfikator.

Obce klucze natomiast są osobna kolumna w tabeli która istnieje w innej tabeli i podaje link pomiędzy dwoma tabelami.

![image.png](image%2012.png)

SQL

W SQL bazy danych są kontrolowane używając DBMS (Database Manegment System). 

Umożliwia on na używanie, aktualizowanie uzyskanych danych przez użytkownika.

Tworzenie baz danych:
`mysql> CREATE DATABASE database_name;`

Podgląd:
`mysql> SHOW DATABASES;`

Użycie:
`mysql> USE thm_bookmarket_db;`

Usuwanie:

```bash
 mysql> DROP database database_name;
```

Przykład utworzonej tabeli:

```bash
mysql> CREATE TABLE example_table_name (
    example_column1 data_type,
    example_column2 data_type,
    example_column3 data_type
);
```

Wyswietlanie zawartosci:

```bash
           mysql> DESCRIBE book_inventory;
```

Wyświetlanie zawartości wewnątrz tabeli:
`mysql> SHOW TABLES;`

CRUD (Create, Read, Update and Delete) 

Są to podstawowe operacje do zmieniania danych.

1. Create (tworzy nowe rekordy)

INSERT INTO

1. Read (Odczytuje wiadomosci z tabeli)

SELECT * FROM books;

1. Update ( aktualizuje dane)

UPDATE books

1. Delete (usuwa)

DELETE FROM books WHERE id = 1;

Zadania składniowe

W SQL oprócz jednowyrazowych komend, są także zadania składniowe jak:

DISTINCT - unika duplikatów, pokazuje ładniej dane w tabeli.

![image.png](image%2013.png)

GROUP BY - grupuje wyniki w kolumnach.

Kolejnosc alfabetyczna i na odwrót.

```bash
SELECT *
    FROM books
    ORDER BY published_date ASC;
```

```bash
 SELECT *
    FROM books
    ORDER BY published_date DESC;
```

W sql  można wyszukiwać dane według pewnych kryteriów:

```bash
SELECT *
    FROM books
    WHERE published_date <= "2021-11-15";
```

```bash
SELECT *
    FROM books
    WHERE published_date <= "2021-11-15";
```

W sql można także używać łańcuchów jak:

CONCAT(), GROUP_CONCAT(), SUBSTRING().

W tym labolatorium doświadczyłem przemieszczanie się po interfejsie SQL. Zrozumiałem że są w nim tabele oraz że stosuje on relacyjne bazy danych. Przeglądnałem podstawowe komendy SQL do tworzenia list czy tabeli. Udało mi się także prześledzić dane wewnątrz tabel przykładowo używając komendy SELECT * FROM żeby przejrzeć listę urządzeń do hakowania. Wyświetliłem listy w kolejności alfabetycznej i na odwrót. Można także wyszukiwać rzeczy w tabelach używajac roznych operatorow.