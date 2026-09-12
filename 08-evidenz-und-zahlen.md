# Evidenz und Zahlen für den Vortrag

Diese Datei ist als Quellenfolie oder Appendix gedacht.

## 1. Vertrauen und Friktion bei AI-generiertem Code

**Stack Overflow Developer Survey 2025**

- 66 %: größte Frustration sind AI-Lösungen, die fast richtig, aber nicht ganz richtig sind
- 45 %: Debugging von AI-generiertem Code ist zeitaufwendiger
- 46 % misstrauen der Genauigkeit von AI-Outputs
- 33 % vertrauen der Genauigkeit
- nur 3 % geben "highly trusting" an

Quelle:  
https://survey.stackoverflow.co/2025/ai

**Geeignete Aussage:**  
AI reduziert die Kosten der Code-Erzeugung, nicht automatisch die Kosten der Verifikation.

---

## 2. Produktivität ist stark kontextabhängig

**METR, Juli 2025**

Randomisierte Studie mit 16 erfahrenen Open-Source-Entwicklern, 246 realen Tasks und großen, ihnen vertrauten Repositories. Mit frühen 2025er AI-Tools benötigten die Teilnehmer im Mittel 19 % länger.

Quelle:  
https://metr.org/blog/2025-07-10-early-2025-ai-experienced-os-dev-study/

**Wichtige Einschränkung:**  
METR sagt ausdrücklich nicht, dass AI die Mehrheit der Entwickler langsamer macht. Untersucht wurde ein spezieller Brownfield-Kontext mit frühen 2025er Tools.

**Update, Februar 2026:**  
METR hält es für wahrscheinlich, dass neuere AI-Tools Entwickler inzwischen stärker beschleunigen. Das Nachfolgeexperiment liefert wegen Selektions- und Messproblemen jedoch keine zuverlässige Schätzung der aktuellen Effektgröße.

Quelle:  
https://metr.org/blog/2026-02-24-uplift-update/

**Geeignete Aussage:**  
Benchmark-Leistung, subjektiv empfundene Beschleunigung und reale Produktivität sind drei verschiedene Größen.

---

## 3. Lokale Verbesserung ist nicht automatisch bessere Delivery

**DORA 2024**

Ein Anstieg der AI-Adoption um 25 % war assoziiert mit:

- +7,5 % Dokumentationsqualität
- +3,4 % Codequalität
- +3,1 % Code-Review-Geschwindigkeit
- -1,5 % Delivery Throughput
- -7,2 % Delivery Stability

Quelle:  
https://cloud.google.com/blog/products/devops-sre/announcing-the-2024-dora-report

**Geeignete Aussage:**  
AI Productivity ist nicht dasselbe wie Software Delivery Performance.

---

## 4. Grilling vor Planning

**GitHub Spec Kit**

Der dokumentierte Agentic-SDD-Workflow lautet:

```text
constitution → specify → clarify → plan → checklist → tasks → analyze → implement → converge
```

`clarify` ist ausdrücklich für unterdefinierte Bereiche gedacht und wird vor `plan` empfohlen.

Quelle:  
https://github.com/github/spec-kit/blob/main/docs/reference/agentic-sdd.md

---

## 5. Persistente Artefakte im SDD

**GitHub Spec Kit**

Jede Phase erzeugt Markdown-Artefakte für die nächste Phase. Der Kernprozess ist Spec → Plan → Tasks → Implement, ergänzt um Clarify, Analyze und Converge.

Quelle:  
https://github.com/github/spec-kit/blob/main/README.md

**OpenSpec**

OpenSpec bündelt Änderungen als `proposal.md`, Specs, `design.md` und `tasks.md`. Der Standardprozess lautet Proposal → Specs → Design → Tasks → Implement.

Quelle:  
https://github.com/Fission-AI/OpenSpec/blob/main/docs/concepts.md
