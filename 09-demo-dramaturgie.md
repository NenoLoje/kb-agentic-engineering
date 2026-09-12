# Demo-Dramaturgie: dieselbe Aufgabe durch alle Stufen

## Ziel

Nicht sechs isolierte Features zeigen, sondern dieselbe kleine Anwendung schrittweise professionalisieren. So wird sichtbar, was jede Stufe tatsächlich hinzufügt.

## Beispielaufgabe

"Baue einen kleinen Service, über den Kunden Support-Tickets anlegen und deren Status verfolgen können."

## 1. One-shot

Prompt geben, Ergebnis erzeugen lassen, kurz zeigen, dass es funktioniert.

**Publikumsfrage:**  
Welche Entscheidungen hat das Modell gerade für uns getroffen, ohne zu fragen?

## 2. Grilling

Fragen zu Rollen, Statusmodell, Prioritäten, Authentifizierung, Datenhaltung, SLA, Löschung und Erfolgskriterien beantworten.

**Sichtbarer Unterschied:**  
Aus einer vagen Idee entsteht ein definierter Scope.

## 3. Planning

Agent analysiert Stack und Codebase und schlägt Architektur, Datenmodell, API und Umsetzungsschritte vor.

**Sichtbarer Unterschied:**  
Technische Entscheidungen werden vor der Implementierung reviewbar.

## 4. SDD

Spec, Plan und Tasks als Markdown-Dateien erzeugen.

**Sichtbarer Unterschied:**  
Das Projektwissen überlebt die Session und kann versioniert werden.

## 5. Harness

Tests, Linting, Architekturregeln und ein Quality Gate hinzufügen.

**Sichtbarer Unterschied:**  
Der Agent bekommt nicht nur Anweisungen, sondern messbares Feedback.

## 6. Agentic Team

Eine Rolle erstellt oder schärft das Produktverhalten, eine zweite prüft Architektur, eine dritte implementiert, eine vierte reviewed oder testet.

**Sichtbarer Unterschied:**  
Arbeit und Qualitätsverantwortung werden getrennt.

## Abschluss der Demo

Zeige am Ende nicht nur den fertigen Code, sondern das entstandene Engineering-System:

```text
specs/
agents/
skills/
tests/
decisions/
CI
```

Die Pointe ist nicht "mehr Dateien". Die Pointe ist, dass Intent und Qualitätsmaßstab nicht mehr nur im Kopf des Entwicklers oder im Chat liegen.
