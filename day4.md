# Tag 4 — 2026-10-04

## Was habe ich gelernt?

Heute habe ich im Rahmen der Hausaufgaben (Modul 4, No-Code Tools) eine
Bau-Kalkulation-App gebaut. Gelernt habe ich, wie sich drei Werkzeuge die Arbeit
teilen: Lovable für die App, Airtable als einzige Datenbank und n8n für die
Automation, die im Hintergrund die Materialpreise aktuell hält. Die KI-Bausteine
kommen von Claude: Haiku liest Preise aus Produktseiten, Sonnet sucht Produkte in
Shops.

## Welches Problem hatte ich?

Nicht jeder Shop lässt sich einfach auslesen. Bauhaus sperrt automatische Abrufe
(Fehler 403), und bei Konfigurator-Seiten steht der Preis erst nach der Auswahl
von Mass oder Länge da. Dazu kommt das Limit des Airtable-Free-Plans mit 1.000
API-Aufrufen im Monat.

## Wie habe ich es gelöst?

Gesperrte Quellen werden als „Fehler“ markiert, der Lauf geht trotzdem weiter.
Bei Konfiguratoren liest der Workflow die Variantentabelle aus dem Seitencode.
Gegen das Airtable-Limit lädt die App einmal pro Sitzung und schreibt gebündelt,
zehn Datensätze pro Aufruf.
