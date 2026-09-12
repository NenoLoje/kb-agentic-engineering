# AI / LLM / Agentic Engineering – Begriffsglossar

## Überblick

Dieses Glossar übersetzt vier häufig verwendete Begriffe aus dem Kontext von AI, LLMs und Agentic Engineering ins Deutsche. Wo eine wörtliche Übersetzung wenig hilfreich wäre, wird bewusst eine praxisnahe deutsche Bezeichnung verwendet.

---

## 1. Harness

**Empfohlene deutsche Übersetzung:**  
**Ausführungs- und Steuerungsrahmen** bzw. **Agenten-Infrastruktur**

### Bedeutung

Ein **Harness** ist die Software-Schicht rund um ein Large Language Model (LLM), die aus dem Modell einen praktisch einsetzbaren Agenten macht.

Typische Bestandteile eines Harness sind:

- Tool-Zugriffe und API-Aufrufe
- Kontext- und Memory-Management
- Berechtigungen und Guardrails
- Ausführungs- und Agent-Loops
- Fehlerbehandlung und Wiederholungslogik
- Verifikation und Tests
- Logging, Tracing und Observability

Eine griffige Vereinfachung lautet:

> **Agent ≈ Model + Harness**

Das Modell liefert Sprachverständnis, Schlussfolgerungen und Entscheidungen. Das Harness stellt die Umgebung bereit, in der daraus kontrollierte Aktionen werden.

### Praxisbeispiel

Ein Coding-Agent erkennt, dass er für eine Aufgabe:

1. ein Repository durchsuchen,
2. eine Datei ändern,
3. Tests ausführen und
4. einen Fehler korrigieren muss.

Das **LLM entscheidet**, was als Nächstes sinnvoll ist.  
Das **Harness** stellt Dateizugriff und Terminal bereit, führt die Tool-Aufrufe aus, gibt Ergebnisse an das Modell zurück und kontrolliert, welche Aktionen erlaubt sind.

### Merksatz

**Das Modell denkt – das Harness ermöglicht, steuert und kontrolliert das Handeln.**

---

## 2. Grilling

**Empfohlene deutsche Übersetzung:**  
**gezieltes Ausfragen**, **kritisches Abklopfen** oder **Requirements-Stresstest**

### Bedeutung

„Grilling“ ist kein streng normierter AI-Fachbegriff, sondern ein zunehmend verwendeter informeller Begriff für einen Arbeitsmodus, bei dem ein AI-Agent **vor der eigentlichen Umsetzung systematisch Rückfragen stellt**.

Ziel ist es, unter anderem folgende Punkte frühzeitig sichtbar zu machen:

- unklare Ziele
- fehlende Anforderungen
- versteckte Annahmen
- Scope und Grenzen
- Risiken und Edge Cases
- Erfolgskriterien
- noch offene Entscheidungen

Statt mit einer vagen Aufgabe sofort loszuarbeiten, versucht der Agent zunächst, ein belastbares gemeinsames Verständnis herzustellen.

### Praxisbeispiel

Der Nutzer sagt:

> „Baue mir eine Buchungs-App.“

Ein Agent im „Grilling“-Modus beginnt nicht sofort mit der Implementierung, sondern fragt beispielsweise:

- Wer darf buchen?
- Können Buchungen storniert werden?
- Wie werden Doppelbuchungen verhindert?
- Gibt es Rollen und Berechtigungen?
- Sind Zahlungen Teil des Prozesses?
- Woran erkennen wir, dass die Lösung fertig und korrekt ist?

Erst wenn die entscheidenden Fragen geklärt sind, beginnt die Umsetzung.

### Merksatz

**Grilling = erst die Anforderungen herausarbeiten und stress-testen, dann bauen.**

---

## 3. Intent

**Empfohlene deutsche Übersetzung:**  
**Absicht**, **Zielabsicht** oder – im Engineering-Kontext oft am treffendsten – **gewünschtes Ergebnis**

### Bedeutung

Der **Intent** beschreibt, **was ein Nutzer tatsächlich erreichen möchte** – nicht nur, was wörtlich in einem Prompt steht.

Für agentische Systeme ist diese Unterscheidung besonders wichtig: Ein Agent soll nicht lediglich einzelne Anweisungen ausführen, sondern das zugrunde liegende Ziel, relevante Rahmenbedingungen und Erfolgskriterien verstehen.

Im Zusammenhang mit **Intent Engineering** wird die Aufgabe des Menschen daher zunehmend darin gesehen, das gewünschte Ergebnis so präzise zu beschreiben, dass ein Agent daraus eigenständig eine geeignete Umsetzung ableiten und deren Erfolg überprüfen kann.

### Praxisbeispiel

Ein Nutzer schreibt:

> „Mach den Checkout schneller.“

Das ist eine Anweisung, aber der eigentliche **Intent** könnte lauten:

> „Reduziere die wahrgenommene Ladezeit des Checkouts auf unter zwei Sekunden, ohne Zahlungsvalidierung, Betrugsschutz oder Datenintegrität zu schwächen.“

Die zweite Formulierung beschreibt nicht nur eine Aktivität, sondern **Ziel, Constraints und Erfolgskriterium**.

### Merksatz

**Prompt = was ich sage. Intent = was ich damit erreichen will.**

---

## 4. Squad / SQUAD

**Empfohlene deutsche Übersetzung:**  
**Agenten-Team**, **Multi-Agent-Team** oder **KI-Entwicklungsteam**

### Bedeutung

Im Agentic-Engineering-Kontext bezeichnet **Squad** häufig eine Gruppe spezialisierter AI-Agenten, die gemeinsam an einer Aufgabe arbeiten.

Dabei übernehmen verschiedene Agents unterschiedliche Rollen, zum Beispiel:

- Product / Requirements
- Architektur
- Backend
- Frontend
- Testing
- Review
- DevOps
- Orchestrierung

Ein übergeordneter Agent oder Orchestrator kann Aufgaben zerlegen, an spezialisierte Agents delegieren und deren Ergebnisse zusammenführen.

Wichtig: **„Squad“ ist in diesem Zusammenhang kein universell definiertes Akronym.** Die konkrete Bedeutung hängt vom jeweiligen Framework, Produkt oder Team ab.

### Praxisbeispiel

Statt einen einzelnen Coding-Agenten eine komplette Anwendung erstellen zu lassen, arbeitet eine kleine Agenten-Squad:

- ein **Architect-Agent** entwickelt die technische Struktur,
- ein **Developer-Agent** implementiert,
- ein **Test-Agent** prüft das Verhalten,
- ein **Reviewer-Agent** bewertet Qualität und Risiken.

So entsteht ein arbeitsteiliges Multi-Agent-System, das organisatorischen Rollen eines menschlichen Teams ähnelt.

### Merksatz

**Squad = mehrere spezialisierte Agents arbeiten wie ein kleines Team zusammen.**

---

## Achtung: Squad ≠ SQuAD

Der Begriff **SQuAD** mit kleinem „u“ bezeichnet etwas anderes:

**SQuAD = Stanford Question Answering Dataset**

Dabei handelt es sich um einen bekannten Datensatz bzw. Benchmark für Machine-Reading- und Question-Answering-Systeme.

SQuAD hat daher **keinen direkten Zusammenhang mit einem Agenten-Team oder einer Agentic Squad**.

---

## Empfohlene Schreibweise für deutschsprachige Unterlagen

Für Präsentationen, Workshops oder Kundendokumente empfiehlt sich, die englischen Begriffe beizubehalten und beim ersten Auftreten mit einer kurzen deutschen Einordnung zu versehen:

| Englischer Begriff | Empfohlene deutsche Einordnung |
|---|---|
| **Harness** | Agenten-Infrastruktur / Ausführungs- und Steuerungsrahmen |
| **Grilling** | gezieltes Ausfragen / Requirements-Stresstest |
| **Intent** | Zielabsicht / gewünschtes Ergebnis |
| **Squad** | Agenten-Team / Multi-Agent-Team |

So bleibt die Terminologie anschlussfähig an englischsprachige Fachliteratur, Tools und Frameworks, ist aber auch für ein deutschsprachiges Publikum unmittelbar verständlich.

---

## Kurzfassung

**Harness**  
Die technische Umgebung rund um das LLM, die Tools, Kontext, Ausführung, Sicherheit und Kontrolle bereitstellt.

**Grilling**  
Ein strukturierter Klärungsprozess, bei dem der Agent kritische Fragen stellt, bevor er mit der Umsetzung beginnt.

**Intent**  
Das eigentliche Ziel bzw. gewünschte Ergebnis hinter einer Nutzeranweisung.

**Squad**  
Ein Team mehrerer spezialisierter AI-Agenten, die arbeitsteilig an einer Aufgabe arbeiten.

---

## Quellen und weiterführende Hinweise

- TechTarget: *AI agent harnesses: The infrastructure behind autonomy*  
  https://www.techtarget.com/ai/tip/AI-agent-harnesses-The-infrastructure-behind-autonomy

- hiDaDeng / grill-me: *Agent skill for deep clarification before action*  
  https://github.com/hiDaDeng/grill-me

- teamvoth / claude-skills: *Grill Me – structured interview to surface unstated requirements*  
  https://github.com/teamvoth/claude-skills/blob/main/skills/grill-me/SKILL.md

- Cole Medin Knowledge Base: *Intent Engineering*  
  https://github.com/coleam00/cole-medin-knowledge-base/blob/main/concepts/intent-engineering.md

- bijutharakan / multi-agent-squad: *Multi-Agent Squad*  
  https://github.com/bijutharakan/multi-agent-squad

- Stanford Question Answering Dataset (SQuAD)  
  https://rajpurkar.github.io/SQuAD-explorer/

---

*Stand: September 2026. Die Terminologie im Bereich Agentic Engineering entwickelt sich schnell; insbesondere „Grilling“, „Harness“ und „Squad“ können je nach Anbieter oder Framework leicht unterschiedlich verwendet werden.*
