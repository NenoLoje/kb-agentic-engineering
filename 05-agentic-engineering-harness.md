# Stufe 5: Agentic Engineering / Harness

## Kernbotschaft

Agentic Engineering beginnt dort, wo nicht nur der Auftrag strukturiert ist, sondern auch die Art, wie ein Agent arbeitet und wie sein Ergebnis überprüft wird.

## Vom Dokument zum System

```text
Specs
  + Regeln
  + Skills
  + Tools
  + Tests
  + Evals
  + CI
  + Permissions
  + Observability
= Engineering Harness
```

## Typische Artefakte

```text
AGENTS.md
architecture.md
skills/
tests/
evals/
.github/workflows/
decisions/
```

## Was der Harness leistet

- Gibt dem Agenten stabile Arbeitsregeln
- Beschränkt erlaubte Aktionen
- Macht Qualität maschinell prüfbar
- Liefert Feedback nach jedem Schritt
- Reduziert die Abhängigkeit von einem einzelnen perfekten Prompt
- Macht Agenten austauschbarer

## Warum das wichtig ist

DORA 2024 zeigt ein gemischtes Bild der AI-Adoption: Ein Anstieg der AI-Nutzung um 25 % war unter anderem mit **7,5 % höherer Dokumentationsqualität**, **3,4 % höherer Codequalität** und **3,1 % schnellerem Code Review** assoziiert. Gleichzeitig wurden **1,5 % geringerer Delivery Throughput** und **7,2 % geringere Delivery Stability** beobachtet.

Die Autoren betonen robuste Tests und kleine Batch-Größen als wichtige Grundlagen für zuverlässige Delivery.

Quelle: Google Cloud, DORA 2024  
https://cloud.google.com/blog/products/devops-sre/announcing-the-2024-dora-report

## Aussage für die Bühne

> Lokale Coding-Produktivität und globale Delivery-Performance sind nicht dasselbe.

## Take-away

> Agentic Engineering optimiert nicht nur den Agenten. Es optimiert die Umgebung, in der der Agent arbeitet.

## Übergang

Sobald Arbeit groß genug wird, reicht ein einzelner Generalist oft nicht mehr. Dann wird aus Prozessstruktur eine Organisationsstruktur.
