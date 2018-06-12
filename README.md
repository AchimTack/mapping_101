# Mapping 101 - The very basics every data journalist should know about mapping

A workshop held at German investigative journalist conference [Netzwerk Recherche 18](https://nr18.sched.com/event/E4vf) by Hannes Kröger, Patrick Stotz, Achim Tack and Marie-Louise Timcke.

**This document is very much work in progress - come back at the end of June to see the finished version**

*Interne Notiz: Die grobe Struktur stammt aus unserem Brainstorming. Lasst uns wie geplant versuchen, alles in diesem Repository zu sammeln. Sammlung auf englisch, Workshop dann auf deutsch. Die deutschen Texte zwischendrin sind die Umschreibungen was wir in den Kapiteln grob vor haben. Sollten dann nach und nach verschwinden, wenn wir das hier mit Inhalt füllen.*

## Quickstart QGIS (5 min)
*Wir zeigen die absoluten QGIS basics: Bedienelemente, File-Browser, Plugin-Installation, Info-I, Print composer,...*
> Am Ende steht der Hinweis: "Man zeichnet i.d.R. keine Karten bzw. Layer neu sondern erstellt diese aus ebstehenden Daten"

## Data sources (10 min)
*Hier die häufigsten / nützlichsten Quellen für Datenjournalisten (in Deutschland) aufführen und im Workshop ausschnittsweise zeigen. Am besten thematisch sortiert à la: adminstrative Grenzen, Luftbilder,OSM...*

- Natural Earth http://www.naturalearthdata.com/
- BKG
- TPHH http://suche.transparenz.hamburg.de/ & http://suche.transparenz.hamburg.de/?extras_registerobject_type=geodat
- OSM
  - Einzelne Features (via Query auf osm.org)
  - Regionale Extrakte
  - Overpass(-Turbo)
  - QuickOSM
- Copernicus, Landsat https://remotepixel.ca/, https://search.remotepixel.ca/, https://github.com/ungarj/awesome-sentinel-2, https://github.com/attibalazs/awesome-remote-sensing

## File formats (15 min)
*Wir sollten ganz kurz erklären, was der Unterschied zwischen Raster- und Vektordaten ist. Am besten anhand von Beispielen/Beispielabbildungen*

*Datentypen, die einem als Datenjournalist häufiger begegnen und wie man sie in QGIS einlädt. Beispiele in einen Repository-Unterordner packen und dann live vorführen*
- shapefile
- basemap
- WMS
- WFS
- xls(x) / csv with coordinates
- geotiff

## Handling geodata properly in QGIS (and some helper tools) (10 min)
*Projektionen, Generalisierung, Dateiformate kovertieren, Geodaten filtern ohne Originaldaten zu zerschießen*

Beispiele könnten sein:
- Projektion eingeladener Layer in QGIS checken
- otf-Projektionen verstehen
- Daten generalisieren mit http://mapshaper.org/
- BKG-Layer filtern
  - Filtern nicht nach Name sondern AGS
  - GS-2/4 Filterung erläutern

## Answering spatial questions (15 min)
*Table join, spatial join, buffer*

Beispiele könnten sein:
- Zensus Raster -> wie viele Menschen sind von X betroffen
- Wieviele Ärzte in irgendeinem Bereich
- Objekte finden auf die “etwas “ zutrifft

## Map Layout (10 min)
*Hinweis auf Print Composer als einzig korrekter Weg, Karten aus QGIS abzuspeichern, ggf. Atlas ansprechen*

## Last Resort: Editing Geodata
*If you have to (and you shouldn't): How to edit Geodata
- Kurzes Zeichnen eines Punktes (z.B. für Locator-Karte)
- Mergen von 2 BKG Gemeinden (Beispiel Gebietsreform)

