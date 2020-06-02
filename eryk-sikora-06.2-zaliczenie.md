# Charakterystyka sieci
#### Autor: Eryk Sikora, nr albumu: 213512, gr WZISN1-2412Io

## Dane sieci:
- adres IP: 162.53.85.180
- maska: /20 -> 255.255.240.0
#### Ze względu na to, że nie można podzielić sieci na dowolne liczby przyjąłem, że sieć składa się z 4094 hostów
- 1 adres IP dla sieci
- 1 adres IP dla broadcast
- 4094 adresy dla hostów
Z tej puli mogę przeznaczyć 3000 miejsc na hosty wymagane w projekcie sieci.
## Podział sieci:
##### (obejmuje cz. II zadania - w dużej mierze tożsame z cz. I)
- LAN 1 162.53.80.0/22 (R1: 10.10.1.1)
- LAN 2 162.53.84.0/22 (R2: 10.10.4.1)
- - LAN 4 (2.2) 162.53.85.0/24
- - LAN 5 (2.3) 162.53.86.0/24
- - LAN 6 (2.4) 162.53.87.0/24
- LAN 3 162.53.88.0/22 (R3: 10.10.8.1)
- - LAN 7 (3.2) 162.53.89.0/23 (uwzględniłem 510 hostów z poprawki z github)
- - LAN 8 (3.3) 162.53.90.0/28
- - LAN 9 (3.4) 162.53.91.0/26
Sieci LAN 3.1 i LAN 2.1 są niewykorzystane.
Sieć LAN 4 pozostaje niewykorzystana (R4: 10.10.12.1)

Połączenie R1 z R2 następuje okrężnie - poprzez R3 (nie ma bezpośredniej wiązki).

Zestawienie urządzeń:
- 4x PC
- 3x laptop
- 3x router, w tym dwa rozszerzane o dodatkowe moduły/porty RJ45 by obsłużyć podsieci
- 7x Switch LAN
