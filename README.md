# Telvira
Linux Terminal based elvira(online timetable for MÁV)

Adat forrás (nem hivatalos elvira API) https://bitbucket.org/oroce/elvira-api/wiki/Home

Letöltés `git clone https://github.com/cinesky/Telvira.git`

Futtatási engedély adás  az adott mappából `chmod 755 telvira`

Keresés: Kiindulás és Érkezési állomás megadása több keresési feltétel a `details` kapcsolóval lehet megadni
Egyzerűsített keresés: `Sopron Győr`
Több keresési feltétel: `Sopron Győr details`

A kedvezméynek kódjának teljes listája: https://bitbucket.org/oroce/elvira-api/wiki/vegpontok/elvira.wiki#!jegy-tipusa

Válasz:

```
Ind.    Érk.    Átsz.   Ut. idő Táv     2.osztály       1.osztály
14:21   15:19           0:58    85 km   2.130 Ft        2.550 Ft
14:46   16:06           1:20    85 km   1.680 Ft
15:45   17:06           1:21    85 km   1.680 Ft
16:21   17:19           0:58    85 km   2.130 Ft        2.550 Ft
16:46   18:06           1:20    85 km   1.680 Ft
17:46   19:06           1:20    85 km   1.680 Ft
18:21   19:19           0:58    85 km   2.130 Ft        2.550 Ft
18:46   20:06           1:20    85 km   1.680 Ft
19:44   21:06           1:22    85 km   1.680 Ft
22:29   23:43           1:14    85 km   1.680 Ft
```


Több információt egy vonatról a `more` és a vonat indulási idejének megadásával lehet megtudni. pl.: `more 16:21`

```
Ind/Érk Vágány  Állmás                  Vonatinfo
16:21           Sopron                  TÛZTORONY IC ( - Budapest-Keleti)
17:19   3       Gyõr                    null
```


Jegyet a `buy` és a vonat indulási idejének megadásával lehet indítani. pl.: `buy 16:21`

Új keresést a `search` megadásával lehet indítani.

Kilépés az `exit` megadásával.
