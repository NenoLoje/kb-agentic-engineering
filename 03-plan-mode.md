# Stufe 3: plan mode

## Kernbotschaft

Der plan mode trennt Analyse und Entscheidung von der Umsetzung. Der Agent untersucht zuerst Codebase, Abhängigkeiten und Optionen und schlägt dann einen nachvollziehbaren Implementierungsweg vor.

## Typischer Ablauf

```text
Explore → Analyze → Decide → Plan → Implement
```

## Was der plan mode besser macht

- Bestehende Patterns werden berücksichtigt
- Auswirkungen auf mehrere Komponenten werden sichtbar
- Architekturentscheidungen können vor dem Coding diskutiert werden
- Der Mensch kann den Plan prüfen, bevor Änderungen entstehen
- Fehlstarts werden günstiger

## Abgrenzung zu Grilling

| Grilling | plan mode |
|---|---|
| Klärt den Intent | Klärt die Umsetzung |
| Produkt- und Scope-Fragen | Architektur- und Implementierungsfragen |
| "Was soll passieren?" | "Wie bauen wir es?" |
| Vor dem technischen Plan | Nach geklärten Anforderungen |

## Die Grenze des plan mode in einer einzelnen Session

Ein guter Plan ist wertvoll. Wenn er aber nur im Chat oder im flüchtigen Session-Kontext existiert, ist er schwer reviewbar, schwer versionierbar und beim nächsten Agentenlauf nicht automatisch verfügbar.

## Take-away

> Der plan mode macht aus Code-Generierung eine bewusste technische Entscheidung. Er macht die Entscheidung aber noch nicht automatisch zu dauerhaftem Projektwissen.

## Übergang

Der nächste Reifegrad entsteht, wenn Anforderungen und Plan nicht nur im Gespräch leben, sondern als Artefakte im Repository.
