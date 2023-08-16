ZABEZPIECZENIE PRZED WPISYWANIEM BŁĘDNYCH WARTOŚCI

````
ALTER TABLE Pracownicy MODIFY imie NOT NULL;

ALTER TABLE Pracownicy MODIFY nazwisko NOT NULL;

ALTER TABLE Pracownicy MODIFY plec CHECK(plec in ('M', 'K'));

ALTER TABLE Pracownicy MODIFY plec NOT NULL;

ALTER TABLE Produkty MODIFY Stawka_podatku CHECK(Stawka_podatku INALTER TABLE Produkty MODIFY Stawka_podatku CHECK(Stawka_podatku IN (5, 8, 23));

ALTER TABLE Produkty MODIFY Cena_sprzedazy CHECK(Cena_sprzedazy <= 20000);

ALTER TABLE Produkty MODIFY Cena_zakupu CHECK(Cena_zakupu <= 15000);

ALTER TABLE Pracownicy ADD CONSTRAINT pracownicy_pk PRIMARY KEY(ID);
````

KLUCZE GŁÓWNE I OBCE 

````
ALTER TABLE Produkty ADD CONSTRAINT produkty_pk PRIMARY KEY(ID_PRODUKTU);

ALTER TABLE DEPARTAMENTY ADD CONSTRAINT departamenty_pk PRIMARY KEY(KOD_DEPARTAMENTU);

ALTER TABLE Departamenty ADD CONSTRAINT departamenty_fk FOREIGN KEY(ID_KIERWONIKA)
REFERENCES pracownicy(id);
````
