# Physics Study Tutor

[English](https://github.com/Marcel-Rodekamp/physics-AI-tutor/tree/main-english) | **Deutsch**

Ein KI-Lerntutor zum bearbeiten von Übungsblättern und Vorlesungen in Physik. Er wurde für eine Teilchenphysik-Vorlesung nach Griffiths, *Introduction to Elementary Particles*, entwickelt, funktioniert aber für jede Physikvorlesung.

Er gibt dir **keine** fertigen Lösungen. Stattdessen fragt er, was du schon versucht hast, gibt Schritt für Schritt Hinweise, prüft deine eigenen Ergebnisse, erklärt Konzepte und fragt dich zu älterem Stoff ab. Die Idee: Du denkst selbst, die KI macht das Denken leichter.

## Warum so?

Mehrere Studien zu KI-Tutoren finden: Wenn eine KI Studierenden fertige Lösungen liefert, werden die Hausaufgaben besser, aber was sie danach selbstständig können, wird tendenziell *schlechter*. Dieselbe KI, so eingestellt, dass sie Hinweise statt Antworten gibt, hat diesen Effekt weitgehend verhindert, und Tutoren, bei denen man selbst argumentieren muss, führten zu echten Lernerfolgen. Fertige Antworten fühlen sich hilfreicher an – aber dieses Gefühl sagt wenig darüber aus, was man tatsächlich lernt.

## Installation

### Claude (claude.ai, Desktop- oder Mobile-App)

Erfordert einen Pro-, Max-, Team- oder Enterprise-Plan.

1. Lade **[`physics-study-tutor.zip`](physics-study-tutor.zip)** aus diesem Repository herunter (Datei anklicken, dann auf den Download-Button).
2. Öffne in Claude **Settings → Capabilities** und stelle sicher, dass **Code execution and file creation** eingeschaltet ist.
3. Klicke unter Skills auf **Upload skill** und wähle die ZIP-Datei aus.
4. Stelle sicher, dass der Skill eingeschaltet ist.

Claude verwendet den Skill automatisch, wenn du nach Physikaufgaben oder Vorlesungsstoff fragst. Du kannst ihn auch ausdrücklich anfordern: *„Nutze den Physics Study Tutor dafür.“*

### Claude Code

Kopiere den Ordner `physics-study-tutor/` nach `~/.claude/skills/`.

### Andere KI-Tools (ChatGPT, Gemini, kostenloser Claude-Plan, …)

Der Skill ist nur eine Textdatei mit Anweisungen. Öffne [`physics-study-tutor/SKILL.md`](physics-study-tutor/SKILL.md), kopiere alles unterhalb des `---`-Kopfbereichs und füge es in die benutzerdefinierten Anweisungen des Tools ein – zum Beispiel in ein ChatGPT-Projekt oder einen Custom GPT, ein Gemini-Gem oder ein Claude-Projekt. Tools, die das offene Agent-Skills-Format unterstützen, können den Ordner auch direkt laden.

Die Anweisungen sind auf Englisch geschrieben; der Tutor antwortet aber in der Sprache, in der du schreibst.

## So benutzt du ihn

- **Übungsblätter:** Lade die Aufgabe hoch oder füge sie ein und schreib dazu, was du schon versucht hast und wo du hängst. Rechne mit Rückfragen, nicht mit einer Lösung.
- **Vorlesung nacharbeiten:** „Lass uns die heutige Vorlesung zum Quarkmodell durchgehen“ – er bittet dich zuerst, die wichtigsten Ergebnisse aus dem Gedächtnis aufzuschreiben, und geht dann die Schritte mit dir durch.
- **Kontrolle:** „Ich habe X raus – stimmt das?“ Er sagt dir, ob es stimmt, und falls nicht, *wo* der Fehler liegt, damit du ihn selbst korrigieren kannst.
- **Abfragen:** „Frag mich zu Woche 1–4 ab“ – eine Frage nach der anderen, gemischt über die Themen.

**Gut zu wissen:**
- KI macht Fehler, besonders bei langen Rechnungen. Prüfe Ergebnisse selbst mit Einheiten, Grenzfällen und Abschätzungen.
- Du kannst das jederzeit umgehen, indem du KI ohne den Skill nutzt. Das ist deine Entscheidung – aber überleg dir, was du am Ende selbst können willst.

## Feedback

Wenn der Tutor zu viel verrät, zu wenig hilft oder sich seltsam verhält, eröffne bitte ein Issue oder sag deinem Tutor Bescheid.
