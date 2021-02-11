---
layout: post
title: "GPU Encoding"
tags: technik
---

Befasst man sich mit dem Thema Livestreaming wird man zwangsläufig auch mit sogenannten Encodern konfrontiert. Ein Encoder ist für die Komprimierung des Videostroms zuständig. Durch die Komprimierung wird sichergestellt, dass nicht mehr Daten als nötig übertragen werden. 

Die Wahl des Encoder beeinflusst maßgeblich die Bildqualität. Prinzipiell stehen zwei Arten von Encodern zur Verfügung: Software- und Hardware-Encoder.

<!--more-->

Software-Encoder sind Programme die in Tools wie OBS oder XSplit eingebettet sind. Daher ist es Aufgabe der CPU die Encoder-Software während des Streamens auszuführen und alle Berechnungen durchzuführen. Da dies sehr aufwendig ist kann die Nutzung eines Software-Encoders dazu führen, dass die CPU zu stark ausgelastet wird und nur noch wenige Ressourcen zur Ausführung anderer Programme (z.B. Spiele) übrig hat.

Bei Hardware-Encodern handelt es sich um spezielle Schaltkreise die sich z.B. auf Mainboards, Grafikkarten oder Capture Cards wiederfinden. Inzwischen werden entsprechende Komponenten sowohl in Intel-, als auch in AMD- und NVIDIA-Grafikchips verbaut.

## Ok, und was bringt mir das jetzt?

Hardware-Encoder, v.a. jene in Grafikchips ("GPU-Encoder"), sind deshalb so attraktiv weil sie die CPU entlasten. Dadurch sind mehr Ressourcen für andere Anwendungen übrig die während des Streamens so genutzt werden.

## Nachteil

Leider liefern GPU-Encoder bei gleicher Bitrate (d.h. bei gleicher Datenmenge) im Schnitt eine etwas schlechtere Bildqualität als Software-Encoder. Wie gut die Qualität tatsächlich ist kann man sich in [entsprechenden Videos](https://www.youtube.com/watch?v=Z6uaPD_5r4w) angucken.

## Ok, aber dann ist das doch uninteressant, oder?

Ganz und gar nicht. Twitch hat nämlich kürzlich die maximale Bitrate seiner Server hochgedreht, d.h. ihr könnt jetzt mit bis zu 6.000kbit/s streamen. Tut ihr das, wird natürlich auch die Bildqualität besser wodurch der o.g. Nachteil quasi[^1] ausgebügelt wird.

## Wie kann ich wechseln?

Je nachdem ob euer Grafikchip von Intel, AMD oder NVIDIA ist müsst ihr in OBS/XSplit in den Encoder-Einstellungen von "x.264″ auf "VCE", "QuickSync" oder "NVENC" wechseln. Die Bitrate könnt ihr zum Vergleich erstmal so lassen und ein paar Testaufnahmen mit denselben Einstellungen machen. Gegebenenfalls könnt ihr die Bitrate danach immer noch hochdrehen.

## Fazit

Gerade für Twitch-Streamer sind GPU-Encoder durch die angehobene maximale Bitrate so attraktiv wie noch nie. Falls ihr jetzt Blut geleckt habt probier’ts doch einfach mal aus.

[^1]: Quasi deswegen da Software-Encoder bei gleicher Bitrate natürlich immer noch eine bessere Bildqualität liefern. Bei 6.000 kbit/s ist die Bildqualität mit einem GPU-Encoder aber imho locker so gut, dass man damit problemlos arbeiten kann.