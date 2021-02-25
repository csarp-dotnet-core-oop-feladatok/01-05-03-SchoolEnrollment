# 01-05-03-SchoolEnrollment
## Osztálydiagram UML kód alapján
Fejlessze ki az osztályokat az UML diagram alapján!  


![UML](https://github.com/csarp-dotnet-core-oop-feladatok/01-05-03-SchoolEnrollment/blob/main/SchoolEnrollment.png?raw=true)

Tesztkód a PointSummary osztályhoz:
```
PointSummary josephTakenScore=new PointSummary(83,94);
```
A teszt kód a következő eredményt adja:
```
Matematika pontszám: 83 pont.
Anyanyelv pontszám: 94 pont.
Összpontszám: 177 pont.
Átlag pontszám: 88,5 pont.
```
Teszkód a SchoolEnrollmentScore osztályhoz:
```
PointSummary josephTakenScore=new PointSummary(83,94);
PointSummary johephAdmissionScore = new PointSummary(74, 85);

SchoolEnrollmentScore josephEnrollment = new SchoolEnrollmentScore("József", josephTakenScore, johephAdmissionScore);
Console.WriteLine(josephEnrollment);
```
A teszt kód eredménye:
```
A felvételiző neve:József
József hozott pontszáma:
   Matematika pontszám: 83 pont.
   Anyanyelv pontszám: 94 pont.
   Összpontszám: 177 pont.
   Átlag pontszám: 88,5 pont.
József felvételin elért pontszáma:
   Matematika pontszám: 74 pont.
   Anyanyelv pontszám: 85 pont.
   Összpontszám: 159 pont.
   Átlag pontszám: 79,5 pont.
József felvételi összpontszáma:168
```


A teljes tesztkód:
```
PointSummary josephTakenScore=new PointSummary(83,94);
PointSummary johephAdmissionScore = new PointSummary(74, 85);
SchoolEnrollmentScore josephEnrollment = new SchoolEnrollmentScore("József", josephTakenScore, johephAdmissionScore);

PointSummary elisabethTakenScore = new PointSummary(87, 93);   
PointSummary elisabethAdmissionScore = new PointSummary(77, 89);
SchoolEnrollmentScore elisabethEnrollment = new SchoolEnrollmentScore("Erzsébet", elisabethTakenScore, elisabethAdmissionScore);

Console.WriteLine(josephEnrollment);
Console.WriteLine(elisabethEnrollment);
```
## Feladat
Írjon kódot, amely kiírja, hogy József vagy Erzsébet felvételi pontszáma a több! Esetleg lehet, hogy megegyeznek a pontszámaik.   
A kód a következő eredményt adja:   
```
Erzsébetnek több felvételi pontja van mint Józsefnek.
```
