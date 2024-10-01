---
Autor: Ingo Schlapschy
Ort: LBS Eibiswald
Gruppe: 24/25 LG1 2aAPC INFv JRZ
Datum: 2024-10-01
AbgabeErledigt: false
---
# Angabe
- [Link zur Angabe](https://www.eduvidual.at/mod/assign/view.php?id=6290138)
- Deadline: 2024-10-02
```
    1. Lernziele
    • Gestaltung von Anwendungen
    • Gestaltungsrichtlinien dokumentieren

    2. Aufgabenstellung
    • Layout mit Photoshop, Gimp, HTML, Word oder IntelliJ (nach belieben)
    • Begründung des Entwurfs
    • Wahl der Benutzeroberfläche (Web oder Applikation)
    • Erstelle einen Layoutentwurf (ohne Funktion) für eine Bruchrechner Applikation 
        ◦ mit allen wichtigen Funktionen auf einem Blick 
    • Berücksichtige die Grundlagen des Layoutdesigns
        ◦ Anwenderebene: erfahrene Anwender
        ◦ Regeln des Schnittstellendesigns (in Doku auch Shortcuts erklären)
    • Anwendungsbereiche
    3. Begründung des Entwurfs

Genaue Erläuterung der Bestandteile der Übersicht.

    4. Wahl der Benutzeroberfläche

Welche Programmform wird gewählt: Browser Client Entwicklungsumgebung ...

```
## Zusammengefasst
## Ziele
- Ziel 1
## ToDo
- [ ] Layout für Bruchrechner erstellen
- [ ] Dokumentieren, warum man was wie umsetzen möchte
# Protokoll
## Umsetzung mit Java Swing (IntelliJ)
- Verwendung von Java Swing (IntelliJ) weil
  - Aufgabe ist damit vermutlich lösbar
  - Habe (durch die letzten Einheiten) schon etwas Erfahrung damit.
## Designentscheidung
![java_UqkTItCDM3](https://github.com/user-attachments/assets/930964c8-ec69-4250-b88c-de0127b416ba)
### Anordnung
- Anordnung der Zahlenfelder wie ein typischer Bruch.
  - Nutzer sind erfahrene Nutzer, sollten mit der Darstellung einer Zahl als Bruch also umgehen können.
  - Auswahl Operator über Dropdown
  - Scheint bei 4 möglichen Operatoren adequat und lässt sich (wenig invasiv) an der richtigen Stelle einfügen
  - Keine Radio-Buttons weil:
    - Nicht verwendeten Operatoren werden dauernd (unnötigerweise) angezeigt
  - Hinweisfeld unter der Operation, für Informatives Feedback bei Fehleingaben
  - Ergebnis in einem Label, statt Textfeld, weil Texteingabe nicht möglich sein soll.
### Endgeräte
- Die Bedienung soll die Verwendung einer Maus unterstützen.
- Die Möglichkeit der Eingabe von Zahlen wird vorrausgesetzt
  - Physikalische oder OS-implementierte Tastatureinabe ist notwendig
  - Tastatur
  - Tastatur & Maus
### Nicht offensichtliche Bedienung
  - Berechnung des Ergebnisses automatisch, sobald alle Felder einen Wert beinhalten.
  - Hinweise:
    - Nicht alle 4 Felder haben einen Wert eingetragen
    - Eine Eingabe ist keien Zahl
    - Der Wert in einem Nenner ist 0
