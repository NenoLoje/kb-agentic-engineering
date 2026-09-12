# Stufe 4: Spec-Driven Development

## Kernbotschaft

Spec-Driven Development externalisiert Intent und Entscheidungen aus dem Context Window in versionierbare Artefakte.

## Prinzip

```text
Specify → Clarify → Plan → Tasks → Implement → Verify
```

## Was sich strukturell ändert

Statt eines langen Chats entstehen explizite Projektartefakte:

```text
specs/
  feature-x/
    spec.md
    plan.md
    tasks.md
```

Diese Dateien können reviewed, versioniert, verändert und von späteren Agentenläufen erneut gelesen werden.

## Beispiel: GitHub Spec Kit

Spec Kit trennt:

- `specify`: Was soll gebaut werden?
- `clarify`: Welche Anforderungen sind noch unklar?
- `plan`: Wie soll es technisch umgesetzt werden?
- `tasks`: Welche konkreten Arbeitsschritte entstehen daraus?
- `implement`: Umsetzung
- `converge`: Abgleich von Implementierung gegen Spec, Plan und Tasks

Quelle:  
https://github.com/github/spec-kit/blob/main/README.md  
https://github.com/github/spec-kit/blob/main/docs/reference/agentic-sdd.md

## Beispiel: OpenSpec

OpenSpec organisiert Änderungen als zusammengehörige Artefakte:

```text
proposal.md   # why + what
specs/        # behavior / requirements
design.md     # how
tasks.md      # implementation checklist
```

Der Default-Workflow lautet:

```text
proposal → specs → design → tasks → implement
```

Quelle:  
https://github.com/Fission-AI/OpenSpec/blob/main/docs/concepts.md

## Warum das mehr ist als "mehr Dokumentation"

- Intent wird zur Source of Truth
- Entscheidungen werden diffbar
- Review kann vor der Implementierung stattfinden
- Neue Sessions müssen nicht den gesamten Gesprächsverlauf kennen
- Traceability zwischen Anforderung, Design und Umsetzung wird möglich

## Take-away

> Der wichtigste Schritt ist nicht, mehr Kontext ins Modell zu packen. Der wichtigste Schritt ist, relevanten Kontext außerhalb des Modells zu strukturieren.

## Übergang

Eine gute Spec sagt, was passieren soll. Für verlässliche Ausführung braucht der Agent zusätzlich Regeln, Tools, Tests und Feedback-Loops.
