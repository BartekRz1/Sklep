````
CREATE USER C##sklep IDENTIFIED BY a123;

GRANT ALL PRIVILEGES TO C##sklep;

CREATE TABLE Pracownicy(
id number,
imie varchar2(30),
nazwisko varchar2(60),
pesel number,
plec varchar2(1),
data_ur date
);
ALTER TABLE Pracownicy ADD pensja number;

CREATE TABLE Produkty(
id_produktu number,
nazwa_poduktu varchar2(100),
typ_produktu varchar2(20),
cena_sprzedazy number,
cena_zakupu number,
stawka_podatku number
);

CREATE TABLE Departamenty(
kod_departamentu number,
nazwa_departamentu varchar2(30),
id_kierwonika number,
miejscowosc varchar2(40)
);
````
Tabela Pracownicy

![image](https://github.com/BartekRz1/Sklep/assets/131479846/93407d11-eda9-4c08-a160-a0714426e462)

Tabela Produkty

![image](https://github.com/BartekRz1/Sklep/assets/131479846/f9974fc9-15af-408e-9cba-c9202365de0d)

Tabela Departamenty

![image](https://github.com/BartekRz1/Sklep/assets/131479846/a7696bad-b7a8-43d8-8650-5ae521ee76cf)


![image](https://github.com/BartekRz1/Sklep/assets/131479846/cb81de9c-d2a6-47f4-b3ee-8f00ed3ff7d3)
