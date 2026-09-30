# Tag 3 — 2026-10-01

## Was habe ich gelernt?

Heute habe ich die Hausaufgabe M3.4 „Prompt Debugging & Optimierung“ gemacht.
Ich habe gelernt, eine schlechte KI-Antwort nicht einfach neu zu prompten, sondern
zuerst genau ein Symptom zu benennen, die Ursache im Prompt zu suchen und dann pro
Runde genau eine Sache zu ändern. Die Erwartung schreibe ich auf, bevor ich den
Prompt abschicke.

## Welches Problem hatte ich?

Beim Tarifvergleich (Fall B) hat die KI behauptet, der Team-Tarif decke fünf
Personen ab. Im Prompt stand dazu aber gar keine Personenzahl, die Angabe war
also erfunden.

## Wie habe ich es gelöst?

Mit Claude Code habe ich drei Runden durchgespielt und ein Log geführt. Am meisten
hat schon der erste Satz gebracht: „Verwende nur die Angaben unten. Wenn eine
Angabe fehlt, schreib das dazu, statt sie anzunehmen.“ Danach kamen noch ein festes
Ausgabeformat und der Input-Check aus der Session dazu. Ohne das Log hätte ich
gedacht, dass erst der Input-Check das Problem löst.
