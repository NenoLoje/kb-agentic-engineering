# Stufe 6: Agentic Team

## Kernbotschaft

Die nächste Stufe verteilt Verantwortung auf spezialisierte Rollen. Ein Orchestrator koordiniert nicht nur Tasks, sondern auch unterschiedliche Perspektiven und Qualitätsverantwortung.

## Beispielstruktur

```text
                    Human
                      |
               Orchestrator
                      |
        +-------------+-------------+
        |             |             |
       PM         Architect         UX
        |             |             |
        +-------+-----+-------------+
                |
             Developer
             /       \
          Tests     Reviewer
             \       /
                QA
```

## Was Rollen explizit machen

- Zuständigkeit
- Input und Output
- erlaubte Entscheidungen
- Qualitätskriterien
- Übergaben an andere Rollen
- Eskalationspunkte an den Menschen

## Rollen können selbst Artefakte sein

```text
agents/
  product-manager.md
  architect.md
  developer.md
  reviewer.md
  qa.md

skills/
  create-prd/
  architecture-review/
  test-plan/
```

## Beispiel: BMAD

BMAD dokumentiert spezialisierte Rollen wie Analyst, Product Manager, Architect, Developer, Scrum Master, UX Designer und Test Engineering Architect. Ein BMad Master übernimmt Meta-Orchestrierung und Multi-Agent-Kollaboration.

Quellen:  
https://github.com/bmad-code-org/BMAD-METHOD/blob/main/docs/index.md  
https://github.com/bmad-code-org/bmad-method-test-architecture-enterprise/blob/main/docs/glossary/index.md

## Wann mehrere Agenten sinnvoll werden

- Arbeit lässt sich klar schneiden
- unterschiedliche Perspektiven sind wirklich wertvoll
- Ergebnisse können unabhängig geprüft werden
- Parallelisierung spart mehr Zeit als Koordination kostet
- Rollen haben eindeutige Inputs und Outputs

## Wann nicht

- kleine, eng gekoppelte Aufgabe
- unklare Verantwortlichkeiten
- mehrere Agenten lesen und schreiben dieselben Artefakte ohne Governance
- Koordinationskosten übersteigen den Nutzen

## Take-away

> Mehr Agenten sind kein Qualitätsmerkmal. Klare Verantwortung ist eines.
