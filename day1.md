# Tag 1 — 2026-09-07

## Was habe ich gelernt?

Ich habe mich intensiv mit dem Weg vom lokalen Repo bis auf GitHub beschäftigt:
Wie ich ein Repo auf dem Rechner anlege, wie ich es mit GitHub verbinde und was
dabei ein SSH-Key ist. Bei mir hängt der Schlüssel als Deploy Key an genau diesem
einen Repo, nicht global an meinem GitHub-Konto. Ausserdem habe ich die drei Stufen
Working Directory, Staging Area und Repository verstanden, was HEAD und ein Branch
technisch sind, und wie Push, Pull und Pull Request zusammenhängen.

## Welches Problem hatte ich?

Viele einzelne Schritte hatte ich noch nicht verstanden und nicht verinnerlicht.
Es gab schon mehrere SSH-Schlüssel auf meinem Rechner, und ich konnte nicht
zuordnen, welcher wofür ist und ob ein neuer Schlüssel etwas kaputt macht.
Dazu kam, dass mich zu viele Schritte auf einmal aus dem Konzept bringen.

## Wie habe ich es gelöst?

Durch ein langes Gespräch mit Claude Code. Ich habe immer wieder nachgefragt,
bis ich jeden einzelnen Schritt wirklich verstanden hatte: was passiert, was
stagen und committen bedeutet, und wie alles zusammenhängt. Dabei kam heraus,
dass meine anderen Projekte gar nicht über SSH laufen, sondern über HTTPS mit
einem Token im Schlüsselbund. Deshalb konnte ich gefahrlos einen eigenen Deploy
Key nur für dieses Repo anlegen.