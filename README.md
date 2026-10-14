# mod_quiz Mock – ByCS Lernplattform

[Deutsch](#deutsch) · [English](#english)

---

## Deutsch

Klickbarer Prototyp für eine überarbeitete Bedienung der Moodle-Aktivität **Test** (`mod_quiz`) auf Basis von Moodle Boost. Der Mock ist eine einzelne HTML-Datei ohne Backend – alle Daten sind Beispieldaten, nichts wird gespeichert.

### Starten

- **Online:** über GitHub Pages (sofern im Repository aktiviert): `https://bycs-lp.github.io/mod_quiz_mock/`
- **Lokal:** `index.html` im Browser öffnen. Bootstrap und Font Awesome werden aus einem CDN geladen, daher ist eine Internetverbindung nötig.

### Sprache und Rolle wechseln

Links am Bildschirmrand befindet sich der Reiter **🌐**. Darüber lassen sich

- die **Sprache** (Deutsch / English) und
- die **Rolle** (Schüler · Lehrer · Admin) umschalten.

Standard ist **Englisch** und **Lehrer**.

### Rolle Lehrer

| Was | Wo |
|---|---|
| Kurs öffnen | Meine Kurse → *Geografie Leistungskurs* |
| Neuen Test anlegen | Bearbeiten-Schalter oben rechts einschalten → **+** zwischen den Abschnitten → *Test* → Assistent |
| Bestehenden Test öffnen | Kursseite → Abschnitt *Tests* → *Asien — China und Indien im Vergleich* |

**Test-Assistent (5 Schritte):**

1. **Allgemeines** – Name, Beschreibung
2. **Voreinstellungen** – Vorlage wählen (Klassenarbeit, Schnelltest, Übungstest, Selbstlerntest)
3. **Details** – Zeit (Moodle-Datumsfelder mit „Aktivieren“), Bestehensgrenze, optional alle erweiterten Einstellungen
4. **Notenschlüssel** – Noten 1–6 oder Punkte 15–0, Grenzen in % oder Punkten („ab ≥“), Feedbacktexte
5. **Fragen** – neue Frage, Zufallsfrage, aus der Fragensammlung, Abschnitte; Gewichtung im Kurs

**Reiter eines Tests:**

- **Übersicht** – Testinfos; *Vorschau anzeigen* startet einen nicht gespeicherten Vorschau-Versuch
- **Fragen** – Fragenübersicht des Tests bearbeiten
- **Einstellungen** – Vorlage wechseln; *Erweiterte Einstellungen öffnen* zeigt alle Testeinstellungen (Zeit, Bewertung, Fragenanordnung, Frageverhalten, Überprüfungsoptionen, Darstellung, Safe Exam Browser, Zugriffsbeschränkungen, Gesamtfeedback/Notenschlüssel, Abschlussbedingungen …)
- **Ergebnisse** – Ansicht *Pro Schüler* oder *Pro Frage*, Spalte **Note** (automatisch aus dem Notenschlüssel, per Klick manuell überschreibbar), Bewertungsverteilung
  - Klick auf einen Namen → Korrektur pro Schüler
  - Ansicht *Pro Frage* → Korrektur pro Frage (inkl. gleicher Punkte für identische Antworten)
- **Fragensammlung** – Suche, erweiterte Filter, **Spalten** ein-/ausblenden, *Frage anlegen* (Assistent für Drag&Drop auf Bild, umschaltbar auf erweiterte Bearbeitung)
- **Mehr → Überschreibungen** – abweichende Zeiten, Versuche oder Kennwort für einzelne Lernende oder Gruppen, Schnellauswahl für Nachteilsausgleich (+25/+50/+100 %)

**Frage erstellen (Multiple Choice):** Im Schritt *Fragen* → **+** → *Neue Frage erstellen* → Fragetyp → *Erweiterte Bearbeitung* zeigt Bewertung je Antwort und alle Zusatzoptionen.

### Rolle Schüler

1. Kurs → Test öffnen → **Test starten**
2. Während des Versuchs: Timer „Verbleibende Zeit“, **Frage markieren**, Navigation nach Aufgaben
3. **Versuch beenden …** → Zusammenfassung mit Status je Frage → *Alles abgeben und beenden*
4. Reiter **Ergebnisse** → **Überprüfung**: Rückschau des bewerteten Versuchs mit Note, Punkten, Feedback, Kommentar der Lehrkraft und Filter nach richtig/teilweise/falsch

### Rolle Admin

Zusätzlich zur Lehrerrolle:

- **Vorlagen verwalten** (Assistent Schritt 2 und 3, Reiter *Einstellungen*): Testvorlagen anlegen; alle Testeinstellungen lassen sich je Vorlage vorbelegen
- **Mit Assistent bearbeiten** (Reiter *Einstellungen*): bestehenden Test im Assistenten bearbeiten

### Hinweise

- Reiner Klick-Prototyp: Eingaben werden nicht gespeichert; nach dem Neuladen ist alles wieder im Ausgangszustand.
- Einige Elemente sind Platzhalter ohne Funktion (z. B. *Filter*, *Berechtigungen*, *Sicherung* im Menü *Mehr*).
- Moodle-Funktionen, die bewusst erweitert wurden: Vorlagen-Assistent, Notenschlüssel mit Überschreiben, Korrektur pro Frage, Schüler-Rückschau, erklärender Gewichtungsdialog, Schnellauswahl Nachteilsausgleich.

---

## English

Clickable prototype for a reworked user experience of the Moodle **Quiz** activity (`mod_quiz`) based on Moodle Boost. The mock is a single HTML file without a backend – all data is sample data, nothing is saved.

### Getting started

- **Online:** via GitHub Pages (if enabled for the repository): `https://bycs-lp.github.io/mod_quiz_mock/`
- **Locally:** open `index.html` in a browser. Bootstrap and Font Awesome are loaded from a CDN, so an internet connection is required.

### Switching language and role

The **🌐** tab on the left edge of the screen lets you switch

- the **language** (Deutsch / English) and
- the **role** (Student · Teacher · Admin).

Defaults are **English** and **Teacher**.

### Teacher role

| What | Where |
|---|---|
| Open the course | My courses → *Geography advanced course* |
| Create a new test | Turn on the edit toggle (top right) → **+** between sections → *Test* → wizard |
| Open an existing test | Course page → section *Tests* → *Asia — China and India compared* |

**Test wizard (5 steps):**

1. **General** – name, description
2. **Presets** – choose a template (class test, quick test, practice test, self-study test)
3. **Details** – timing (Moodle date fields with “Enable”), pass grade, optionally all advanced settings
4. **Grading key** – marks 1–6 or points 15–0, boundaries in % or points (“from ≥”), feedback texts
5. **Questions** – new question, random question, from question bank, sections; weighting in the course

**Test tabs:**

- **Overview** – test information; *Show preview* starts a preview attempt that is not saved
- **Questions** – edit the test's question list
- **Settings** – switch template; *Open advanced settings* shows all test settings (timing, grading, layout, question behaviour, review options, appearance, Safe Exam Browser, extra restrictions, overall feedback/grading key, completion conditions …)
- **Results** – *By student* or *By question* view, **Mark** column (calculated from the grading key, can be overridden manually by clicking it), grade distribution
  - Click a name → grading by student
  - *By question* view → grading by question (incl. same points for identical answers)
- **Question bank** – search, advanced filters, show/hide **columns**, *Create question* (wizard for drag and drop onto image, switchable to advanced editing)
- **More → Overrides** – different dates, attempts or password for individual learners or groups, quick select for extra time (+25/+50/+100 %)

**Create a question (multiple choice):** In step *Questions* → **+** → *Create new question* → question type → *Advanced editing* shows the grade per answer and all additional options.

### Student role

1. Course → open the test → **Start test**
2. During the attempt: “Time left” timer, **Flag question**, navigation by task
3. **Finish attempt …** → summary with status per question → *Submit all and finish*
4. Tab **Results** → **Review**: review of the graded attempt with mark, points, feedback, teacher's comments and a filter for correct/partially correct/incorrect

### Admin role

In addition to the teacher role:

- **Manage templates** (wizard steps 2 and 3, *Settings* tab): create test templates; every test setting can be preset per template
- **Edit with wizard** (*Settings* tab): edit an existing test in the wizard

### Notes

- Pure click prototype: input is not saved; reloading the page resets everything.
- Some elements are placeholders without function (e.g. *Filters*, *Permissions*, *Backup* in the *More* menu).
- Moodle features deliberately extended: template wizard, grading key with override, grading by question, student review, explanatory weighting dialog, quick select for extra time.
