# scriptable.sonnenBatterie
|Widget für iOS14 iPhone            |für sonnenBatterie Eco8.0 und Eco10.0    |
|:-------------------------------------:|:------------------------------------:|
|![sbWidget](sb1.jpg) | ![sonnenLogo](sonnen.png)             |

# sonnenBatterie-Widget
Widget für die sonnenBatterien EC8.0/SB10

## Kurzbeschreibung
Das Wiget für die sonnenBatterie iest ausgewählte Betriebsdaten der sonnenBatterie über deren API-Schnittstelle aus und stellt diese im Widget in einer Übersicht zur Verfügung.

## Settings
Im Script ist in der oberen Zeile die gültige URL der sonnenBatterie im LAN einzugeben.

**ip:** - IP-Adresse der sonnenBatterie in der Form 999:999:999:999

## API-Schnittstelle der sonnenBatterie

Das Script liest die Livedaten der sonnenBatterie über die folgende Adresse aus:

````APIurl ="http://xxx.xxx.xxx.xx:8080/api/v1/status"````

Diese Daten werden zur Anzeige gebracht und in den lokalen bzw. globalen Variablen als Momentanwerte gespeichert; eine Langzeitspeicherung der Daten, bspw. in einer Datenbank, erfolgt nicht.

Die folgenden API-Daten der Batterie werden verarbeitet:

##### JSON

````
{
...,
"Consumption_W":358,
...,
"GridFeedIn_W":5065,
...,
"Pac_total_W":-1031,
"Production_W":6458,
"USOC":58,
...
}
````
## Changelog

2020.11.11 Init sbWidget V1.0
