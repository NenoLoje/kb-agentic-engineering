# Stufe 2: Grilling / Clarification

## Kernbotschaft

Vor dem technischen Plan steht die Klärung der Anforderungen. Der Agent soll nicht sofort bauen, sondern zuerst die offenen Entscheidungen finden.

## Rollenwechsel

```text
Vibe Coding:
Mensch fragt → AI antwortet

Grilling:
AI fragt → Mensch entscheidet
```

## Typische Fragen

- Was ist das eigentliche Ziel?
- Wer nutzt die Funktion?
- Was gehört explizit nicht zum Scope?
- Was sind Erfolgskriterien?
- Welche Randfälle sind relevant?
- Welche Constraints gelten?
- Welche Entscheidung ist Produktentscheidung und welche technische Entscheidung?

## Was sich verbessert

- Implizite Annahmen werden sichtbar
- Scope wird klarer
- Akzeptanzkriterien entstehen früher
- Der Mensch behält Entscheidungen, statt sie unbewusst an das Modell zu delegieren

## Reihenfolge: vor Planning

GitHub Spec Kit beschreibt für Agentic SDD explizit folgende Reihenfolge:

```text
constitution → specify → clarify → plan → checklist → tasks → analyze → implement → converge
```

`/speckit.clarify` soll unterdefinierte Bereiche klären und wird ausdrücklich **vor** `/speckit.plan` empfohlen.

Quelle: GitHub Spec Kit  
https://github.com/github/spec-kit/blob/main/docs/reference/agentic-sdd.md

## Konkretes Pattern

Das Open-Source-Skill `grill-me` führt ein design-only Requirements Interview durch. Es fragt unter anderem nach Ziel, Verhalten, Inputs/Outputs, Scope, Erfolgskriterien, Prioritäten, Constraints und Edge Cases, jeweils eine Frage nach der anderen.

Quelle:  
https://github.com/JRA-CodingLab/grill-me

## Take-away

> Gute Agenten beantworten nicht nur Fragen. Sie helfen, die richtigen Fragen zu stellen.

## Übergang

Nach dem Grilling wissen wir besser, **was** wir wollen. Erst jetzt lohnt sich die nächste Frage: **Wie bauen wir es?**
