# scriptable.sonnenBatterie
![sbWidget](sb1.jpeg)

# sonnenBatterie-Widget
Widget für die sonnenBatterien EC8.0/SB10

## Kurzbeschreibung
Das Widget für die sonnenBatterie liest ausgewählte Betriebsdaten der sonnenBatterie über deren API-Schnittstelle aus und stellt diese in einer Übersicht zur Verfügung.

## Settings
Im Script ist in der oberen Zeile die gültige URL der sonnenBatterie im LAN einzugeben.

**APIurl:** - IP-Adresse der sonnenBatterie in der Form 999:999:999:999

## API-Schnittstelle der sonnenBatterie

Das Script liest die Livedaten der sonnenBatterie über die folgende Adresse aus:

````APIurl ="http://xxx.xxx.xxx.xx:8080/api/v1/status"````

Diese Daten werden zur Anzeige gebracht, eine Speicherung der Daten, bspw. in einer Datenbank, erfolgt nicht.

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

2020.11.11: sonnenBatterie V1.0 (Widget)
