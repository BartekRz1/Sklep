1 Polecenie:

Uporządkowane alfabetycznie zestawienie prezentujące średnią marżę oraz liczbę produktów wszystkich grup towarów, 
których produkty są wyżej opodatkowane niż stawka 8 lub cena zakupu jest niższa niż 1.  


````
SELECT ROUND(AVG(p.cena_sprzedazy - p.cena_zakupu),2) AS srednia_marza,
tp.pelna_nazwa
FROM PRODUKTY P 
INNER JOIN typy_prodoktow TP 
ON P.TYP_PRODUKTU = TP.TYP_PRODUKTU
WHERE stawka_podatku > 8 OR cena_zakupu < 1
GROUP BY tp.pelna_nazwa
ORDER BY tp.pelna_nazwa
````

![image](https://github.com/BartekRz1/Sklep/assets/131479846/ea925e8b-d329-45de-8d87-6f99bcd6c0cb)


2 Polecenie:

Uporządkowane alfabetycznie zestawienie prezentujące wszystkich pracowników który zarabiają więcej od pracownika z najwyższym id i urodzili się po roku 90.


````
SELECT imie, nazwisko, pensja, data_ur 
FROM pracownicy 
WHERE data_ur > TO_DATE('1990-01-01', 'YYYY-MM-DD') 
  AND pensja > (SELECT pensja 
                FROM pracownicy 
                WHERE id = (SELECT MAX(id) 
                            FROM pracownicy))
ORDER BY nazwisko;
````

![image](https://github.com/BartekRz1/Sklep/assets/131479846/03c8844b-2b86-45f6-bc62-b21eaedbd458)


3 Polecenie

Uporządkowane alfabetycznie zestawienie prezentujące pięcu pracowników, który zarabiają najwięcej.

````
SELECT * 
FROM (
     SELECT * FROM PRACOWNICY 
     ORDER BY PENSJA DESC
     )
WHERE ROWNUM <=5
ORDER BY NAZWISKO;
````

![image](https://github.com/BartekRz1/Sklep/assets/131479846/7d3c0a94-b45f-4ce9-88ab-4e8eb35191db)


4 Polecenie

Uporządkowane zestawienie prezentujące liczącą sumę ceny zakupu dla każdej z grup produktów, których cena przekracza 5.

````
SELECT SUM(CENA_ZAKUPU) SUMA_ZAKUPU, PELNA_NAZWA FROM PRODUKTY P
INNER JOIN TYPY_PRODOKTOW TP
ON p.typ_produktu = tp.typ_produktu
GROUP BY TP.PELNA_NAZWA
HAVING SUM(CENA_ZAKUPU) > 5
````

![image](https://github.com/BartekRz1/Sklep/assets/131479846/51d3e9d7-f623-4da1-9090-cc12ed9c5329)
