# Stufe 1: One-shot / Vibe Coding

## Kernbotschaft

Moderne Modelle können aus sehr wenig Input erstaunlich viel funktionierenden Code erzeugen. Das ist schnell, aber viele Produkt- und Architekturentscheidungen bleiben implizit.

## Typischer Ablauf

```text
Idee → Prompt → Code → Ausprobieren
```

## Was daran stark ist

- Sehr geringe Einstiegshürde
- Hohe Geschwindigkeit bei Prototypen und klar abgegrenzten Aufgaben
- Direkter Feedback-Loop
- Besonders geeignet für explorative oder leicht reversible Arbeit

## Wo die Qualität kippt

- Anforderungen sind unvollständig oder mehrdeutig
- Das Modell ergänzt fehlende Entscheidungen selbst
- Ergebnisse können zwischen Runs variieren
- Lokale Plausibilität ersetzt noch keine Systemqualität
- Review- und Debugging-Aufwand kann den Zeitgewinn auffressen

## Beleg

Im Stack Overflow Developer Survey 2025 nannten **66 %** der Befragten als größte Frustration AI-Lösungen, die fast richtig, aber nicht ganz richtig sind. **45 %** nannten zeitaufwendigeres Debugging von AI-generiertem Code. Außerdem misstrauten **46 %** der Genauigkeit von AI-Outputs, gegenüber **33 %**, die ihnen vertrauten.

Quelle: Stack Overflow Developer Survey 2025  
https://survey.stackoverflow.co/2025/ai

## Kontrast für die Bühne

Eine kontrollierte METR-Studie mit erfahrenen Open-Source-Entwicklern in ihren eigenen, großen Repositories fand für frühe 2025er Tools eine **19 % längere Bearbeitungszeit** mit AI. Die Autoren warnen ausdrücklich vor Verallgemeinerungen. Im Februar 2026 schrieb METR zudem, dass neuere Tools wahrscheinlich stärker beschleunigen, die aktuelle Größenordnung aber wegen methodischer Probleme nicht zuverlässig geschätzt werden könne.

Quellen:  
https://metr.org/blog/2025-07-10-early-2025-ai-experienced-os-dev-study/  
https://metr.org/blog/2026-02-24-uplift-update/

## Take-away

> Das Problem ist nicht mehr, ob AI Code schreiben kann. Das Problem ist, ob sie dasselbe Verständnis von "richtig" hat wie wir.

## Übergang

Wenn das Ergebnis von fehlenden Entscheidungen abhängt, hilft nicht automatisch ein längerer Prompt. Der nächste Schritt ist, die fehlenden Entscheidungen sichtbar zu machen.
