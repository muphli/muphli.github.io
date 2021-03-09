---
layout: post
title: "iOS-Shortcuts: Wie man sich einen Ausgaben-Tracker bastelt"
tags: technik
---

Da ich kürzlich auf iOS und das iPhone 11 umgestiegen bin, stellte sich für mich mal wieder die Frage nach den passenden Apps. Vor allem war ich auf der Suche nach einem minimalistischen Ausgaben-Tracker in den ich meine Ausgaben nach Kategorien sortiert eintragen konnte. Leider fand ich keinen, der mir wirklich gefiel und ich kam auf die Idee, stattdessen einen entsprechenden Shortcut zu basteln.

<!--more-->

## Wie funktioniert der Shortcut?

Die Idee dahinter ist, dass der Betrag, die Kategorie und noch eine (optionale) Beschreibung[^1] abgefragt werden und das alles anschließend mit dem aktuellen Datum in eine Numbers-Datei geschrieben werden. Dadurch lassen sich hübsche Visualisierungen/Auswertungen erstellen. Man kann mit den Daten eben all das machen, was mit einer Tabellenkalkulation/mit Pages möglich ist. Alternativ könnte man die Daten auch in eine .csv-Datei schreiben und dann über irgendein anderes Tool visualisieren. Für den Anfang hab‘ ich es aber mit Numbers getestet.

Ein paar Hinweise, falls ihr den Shortcut selbst ausprobieren wollt:

* Es wird davon ausgegangen, dass in eurer iCloud unter „Shortcuts" eine Datei namens „Ausgaben.numbers" existiert. Daher empfiehlt es sich, diese zunächst zu erstellen. Sollte die Datei nicht vorhanden sein, wirft der Shortcut einen Fehler.
* Die Kategorien könnt ihr natürlich anpassen.
* Falls ihr das Datum mit Zeitstempel ausgeben wollt, entfernt einfach den Block um das Datum zu formatieren.

Link zum Shortcut:

()[https://www.icloud.com/shortcuts/be9efdcd5602470cbfa5789e8ef0acdf]

[^1]: Optional in sofern, als dass die entsprechende Zelle dann leer gelassen wird.