TYPY_PRODOKTOW:

````
INSERT INTO TYPY_PRODOKTOW (TYP_PRODUKTU, PELNA_NAZWA, RABAT, OKRES_WAZNOSCI)
VALUES ('SLO', 'SLODYCZE', NULL, 'D')
INSERT INTO TYPY_PRODOKTOW (TYP_PRODUKTU, PELNA_NAZWA, RABAT, OKRES_WAZNOSCI)
VALUES ('SLO', 'SLODYCZE', NULL, 'D')
INSERT INTO TYPY_PRODOKTOW (TYP_PRODUKTU, PELNA_NAZWA, RABAT, OKRES_WAZNOSCI)
VALUES ('ALK', 'ALKOHOL', NULL, 'D')
INSERT INTO TYPY_PRODOKTOW (TYP_PRODUKTU, PELNA_NAZWA, RABAT, OKRES_WAZNOSCI)
VALUES ('KOS', 'KOSMETYKI', NULL, 'D')
INSERT INTO TYPY_PRODOKTOW (TYP_PRODUKTU, PELNA_NAZWA, RABAT, OKRES_WAZNOSCI)
VALUES ('NAP', 'NAPOJE', NULL, 'D')
INSERT INTO TYPY_PRODOKTOW (TYP_PRODUKTU, PELNA_NAZWA, RABAT, OKRES_WAZNOSCI)
VALUES ('NAB', 'NABIAŁ', NULL, 'K')
INSERT INTO TYPY_PRODOKTOW (TYP_PRODUKTU, PELNA_NAZWA, RABAT, OKRES_WAZNOSCI)
VALUES ('NAS', 'NASIONA', NULL, 'D')
INSERT INTO TYPY_PRODOKTOW (TYP_PRODUKTU, PELNA_NAZWA, RABAT, OKRES_WAZNOSCI)
VALUES ('PIE', 'PIECZYWO', NULL, 'D')
````
SELECT * FROM TYPY_PRODOKTOW

![image](https://github.com/BartekRz1/Sklep/assets/131479846/a88ffa5c-2901-443e-9fb4-0a866ab0b610)


PRODUKTY

````
INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(1, 'Chleb pszenny', 'PIE', 2.5, 1.2, 8);

INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(2, 'Mleko 2%', 'NAB', 2.0, 1.0, 5);

INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(3, 'Jogurt naturalny', 'NAB', 1.8, 0.9, 5);

INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(4, 'Jabłka', 'OWO', 3.0, 2.0, 8);

INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(5, 'Pasta do zębów', 'KOS', 8.0, 4.0, 23);

INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(6, 'Szampon nawilżający', 'KOS', 12.0, 6.5, 23);

INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(7, 'Mydło w kostce', 'KOS', 3.5, 1.8, 23);

INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(8, 'Ser żółty', 'NAB', 5.5, 3.2, 8);

INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(9, 'Woda mineralna', 'NAP', 1.2, 0.6, 5);

INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(10, 'Sok pomarańczowy', 'NAP', 3.5, 2.2, 8);

INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(11, 'Kawa ziarnista', 'NAP', 15.0, 9.5, 8);

INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(12, 'Szampon przeciwłupieżowy', 'KOS', 10.0, 5.8, 23);

INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(13, 'Krem nawilżający', 'KOS', 15.5, 8.7, 23);

INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(14, 'Nasiona słonecznika', 'NAS', 2.0, 1.2, 8);

INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(15, 'Nasiona dyni', 'NAS', 2.5, 1.5, 8);

INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(16, 'Piwo jasne', 'ALK', 3.5, 2.0, 23);

INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(17, 'Czekolada mleczna', 'SLO', 2.0, 1.0, 8);

INSERT INTO Produkty (id_produktu, nazwa_poduktu, typ_produktu, cena_sprzedazy, cena_zakupu, stawka_podatku) VALUES
(18, 'Lizaki owocowe', 'SLO', 0.5, 0.2, 8);
````

SELECT * FROM PRODUKTY

![image](https://github.com/BartekRz1/Sklep/assets/131479846/bae6f0fb-9efa-4030-a80f-cf83bb438882)


PRACOWNICY

````
INSERT INTO pracownicy (id, imie, nazwisko, pesel, plec, data_ur, pensja)
VALUES
(1, 'Jan', 'Kowalski', '12345678901', 'M', TO_DATE('2000-01-01', 'YYYY-MM-DD'), 5000);

INSERT INTO pracownicy (id, imie, nazwisko, pesel, plec, data_ur, pensja)
VALUES
(2, 'Anna', 'Nowak', '23456789012', 'K', TO_DATE('1995-05-15', 'YYYY-MM-DD'), 4500);

INSERT INTO pracownicy (id, imie, nazwisko, pesel, plec, data_ur, pensja)
VALUES
(3, 'Piotr', 'Wójcik', '34567890123', 'M', TO_DATE('1988-10-20', 'YYYY-MM-DD'), 6000);

INSERT INTO pracownicy (id, imie, nazwisko, pesel, plec, data_ur, pensja)
VALUES
(4, 'Aleksandra', 'Kaczmarek', '45678901234', 'K', TO_DATE('1992-03-28', 'YYYY-MM-DD'), 4800);

INSERT INTO pracownicy (id, imie, nazwisko, pesel, plec, data_ur, pensja)
VALUES
(5, 'Michał', 'Lewandowski', '56789012345', 'M', TO_DATE('1985-12-10', 'YYYY-MM-DD'), 5500);

INSERT INTO pracownicy (id, imie, nazwisko, pesel, plec, data_ur, pensja)
VALUES
(6, 'Magdalena', 'Zielińska', '67890123456', 'K', TO_DATE('2001-08-05', 'YYYY-MM-DD'), 4200);

INSERT INTO pracownicy (id, imie, nazwisko, pesel, plec, data_ur, pensja)
VALUES
(7, 'Krzysztof', 'Sikora', '78901234567', 'M', TO_DATE('1994-06-22', 'YYYY-MM-DD'), 5800);

INSERT INTO pracownicy (id, imie, nazwisko, pesel, plec, data_ur, pensja)
VALUES
(8, 'Monika', 'Witkowska', '89012345678', 'K', TO_DATE('1989-09-17', 'YYYY-MM-DD'), 5200);

INSERT INTO pracownicy (id, imie, nazwisko, pesel, plec, data_ur, pensja)
VALUES
(9, 'Grzegorz', 'Jaworski', '90123456789', 'M', TO_DATE('1978-04-12', 'YYYY-MM-DD'), 6000);

INSERT INTO pracownicy (id, imie, nazwisko, pesel, plec, data_ur, pensja)
VALUES
(10, 'Marlena', 'Krawczyk', '01234567890', 'K', TO_DATE('1993-11-03', 'YYYY-MM-DD'), 4700);
````

SELECT * FROM PRACOWNICY

![image](https://github.com/BartekRz1/Sklep/assets/131479846/dd8c759c-82dc-4995-9556-5e0bc74975fe)

