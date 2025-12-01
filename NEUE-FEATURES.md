# 🆕 Neue Features - Version 1.1

Diese Anleitung erklärt die neuen Funktionen der Version 1.1 des Listenwahl-Ranking Systems.

## 💾 Speichern & Laden von Rankings

### Ranking speichern

1. Fülle alle gewünschten Daten ein (Kandidaten, Gewichtungen)
2. Klicke oben auf den Button **"Aktuelles Ranking speichern"**
3. Gib einen aussagekräftigen Namen ein (z.B. "Szenario 1: Gleichverteilung" oder "Vorschlag Fraktion A")
4. Bestätige mit OK
5. Das Ranking wird in deinem Browser gespeichert

### Gespeicherte Rankings anzeigen

- Alle gespeicherten Rankings erscheinen automatisch im Bereich "Ranking speichern & laden"
- Du siehst:
  - Den Namen des Rankings
  - Das Speicherdatum und die Uhrzeit
  - Buttons zum Laden und Löschen

### Ranking laden

1. Klicke bei einem gespeicherten Ranking auf **"Laden"**
2. Bestätige die Sicherheitsabfrage
3. Alle Daten (Kandidaten + Gewichtungen) werden geladen
4. Die aktuellen Daten werden überschrieben

### Ranking löschen

1. Klicke bei einem gespeicherten Ranking auf das **Papierkorb-Symbol**
2. Bestätige die Sicherheitsabfrage
3. Das Ranking wird dauerhaft gelöscht

## 🗑️ Daten löschen

### Einzelne Person zurücksetzen

**Was wird gelöscht:**
- Stimmenzahl
- Arbeitsgruppen
- Sitzungsteilnahme
- Alle Pünktlichkeits-Werte
- Freistellungswünsche

**Was bleibt erhalten:**
- Vorname & Nachname
- Geschlecht
- Alter
- Mitgliedschaftsdauer

**So gehst du vor:**
1. Scrolle zur gewünschten Person
2. Klicke oben rechts in der Person-Card auf **"Daten löschen"**
3. Bestätige die Sicherheitsabfrage
4. Nur die Bewertungsdaten werden gelöscht

### Alle Personen zurücksetzen

**Anwendungsfall:** Du möchtest mit denselben Personen ein neues Szenario durchspielen.

**So gehst du vor:**
1. Klicke oben bei "Kandidaten (11 Personen)" auf **"Alle Bewertungsdaten löschen"**
2. Bestätige die Sicherheitsabfrage
3. Alle Bewertungsdaten aller 11 Personen werden zurückgesetzt
4. Namen, Geschlecht, Alter und Mitgliedschaft bleiben erhalten

## 📊 Verbesserte Pünktlichkeitsfelder

Die Pünktlichkeits-Eingabe wurde übersichtlicher gestaltet:

### Neue Struktur

Jedes der drei Pünktlichkeitsfelder hat jetzt eine eigene Überschrift:
- **Sitzungsbeginn**: Pünktlichkeit zum Start der Sitzung
- **Kurze Pause**: Pünktlichkeit nach kurzen Pausen
- **Mittagspause**: Pünktlichkeit nach der Mittagspause

### Eingabehilfen

- Platzhalter-Beispiele zeigen typische Werte (z.B. "-5" für 5 Minuten zu spät)
- Hauptüberschrift erklärt das System: "0 = pünktlich, negativ = zu spät"

## 💡 Praktische Anwendungsfälle

### Use Case 1: Verschiedene Szenarien vergleichen

1. Erstelle ein Ranking mit Gewichtung A → Speichere als "Szenario A"
2. Ändere die Gewichtungen → Speichere als "Szenario B"
3. Lade "Szenario A" und "Szenario B" abwechselnd, um die Unterschiede zu sehen

### Use Case 2: Vorbereitung für Gremiensitzung

1. Erstelle mehrere Rankings mit verschiedenen Gewichtungen
2. Speichere jedes mit aussagekräftigem Namen
3. In der Sitzung: Lade das passende Ranking basierend auf der Diskussion

### Use Case 3: Sensitivitätsanalyse

1. Erstelle ein Basis-Ranking → Speichere als "Basis"
2. Ändere nur eine Gewichtung (z.B. Pünktlichkeit von 10% auf 20%)
3. Speichere als "Test Pünktlichkeit +10%"
4. Vergleiche die Ergebnisse

### Use Case 4: Mehrere Wahlgänge

1. Nach dem ersten Wahlgang: Speichere das Ranking als "Wahlgang 1"
2. Für Wahlgang 2: Lösche die Bewertungsdaten, behalte die Personen
3. Trage neue Bewertungen ein
4. Speichere als "Wahlgang 2"

## 🔒 Datenspeicherung

### Wo werden die Daten gespeichert?

- **Lokal im Browser** (localStorage)
- **Nicht auf einem Server**
- **Pro Browser getrennt** (Chrome ≠ Firefox)
- **Pro Gerät getrennt** (PC ≠ Laptop ≠ Handy)

### Wie lange bleiben die Daten gespeichert?

- Unbegrenzt, bis du sie löschst
- Oder bis du den Browser-Cache löschst
- Oder bis du den Browser deinstallierst

### Sicherheit

✅ **Vorteile:**
- Völlig privat, keine Server
- DSGVO-konform
- Keine Internetverbindung nötig (nach erstem Laden)

⚠️ **Nachteile:**
- Daten sind nicht zwischen Geräten synchronisiert
- Bei Browser-Cache-Löschung gehen Daten verloren
- Nicht für mehrere Nutzer gleichzeitig geeignet

### Backup erstellen

Um deine Rankings zu sichern, bevor du den Browser-Cache löschst:

1. Öffne die App
2. Mache Screenshots der gespeicherten Rankings
3. Oder: Öffne die Browser-Konsole (F12)
4. Gebe ein: `console.log(localStorage.getItem('listenwahl-rankings'))`
5. Kopiere die Ausgabe in eine Textdatei

## ⌨️ Tastaturkürzel & Tipps

### Effiziente Dateneingabe

- **Tab-Taste**: Springe zum nächsten Feld
- **Shift + Tab**: Springe zum vorherigen Feld
- **Enter**: In Eingabefeldern → Nächstes Feld (in den meisten Browsern)
- **Pfeiltasten**: In Zahlenfeldern → Wert erhöhen/verringern

### Schnelles Ausfüllen

1. Kopiere Werte mit Strg+C / Cmd+C
2. Füge sie mit Strg+V / Cmd+V ein
3. Nutze die Tab-Taste zum schnellen Wechsel zwischen Feldern

## ❓ Häufige Fragen zu neuen Features

**Q: Wie viele Rankings kann ich speichern?**
A: Unbegrenzt, solange der Browser-Speicher ausreicht (praktisch: 20-50 Rankings problemlos möglich).

**Q: Kann ich Rankings zwischen Computern übertragen?**
A: Nicht direkt. Du müsstest die localStorage-Daten manuell exportieren/importieren (siehe Backup-Abschnitt).

**Q: Was passiert, wenn ich vergesse ein Ranking zu speichern?**
A: Die Daten sind verloren. Gewöhne dir an, regelmäßig zu speichern!

**Q: Werden die Rankings auch im Inkognito-Modus gespeichert?**
A: Nein, im Inkognito-Modus gehen alle Daten beim Schließen verloren.

**Q: Kann ich ein gespeichertes Ranking umbenennen?**
A: Nicht direkt. Du müsstest es laden, unter neuem Namen speichern und das alte löschen.

**Q: Was passiert wenn ich "Daten löschen" drücke, kann ich das rückgängig machen?**
A: Nein, gelöschte Daten sind unwiderruflich weg. Nur wenn du das Ranking vorher gespeichert hast, kannst du es wieder laden.

## 🎓 Best Practices

### Namenskonvention für Rankings

Gute Namen sind:
- ✅ "2024-12-01 Variante A"
- ✅ "Szenario: Pünktlichkeit gewichtet"
- ✅ "Vorschlag Team Nord"

Schlechte Namen sind:
- ❌ "Test"
- ❌ "asdf"
- ❌ "Ranking 1"

### Workflow-Empfehlung

1. **Basis-Ranking erstellen** mit Stammdaten → Speichern als "Basis [Datum]"
2. **Verschiedene Gewichtungen testen** → Jeweils mit sprechendem Namen speichern
3. **In Gremiensitzung**: Passende Rankings laden und diskutieren
4. **Nach Beschluss**: Finales Ranking speichern als "FINAL [Datum]"
5. **Aufräumen**: Alte Test-Rankings regelmäßig löschen

### Datenschutz

- ⚠️ Nutze keine echten Namen, wenn du Screenshots teilst
- ⚠️ Lösche sensible Rankings nach Verwendung
- ✅ Nutze anonymisierte Codes statt Namen bei sensiblen Daten

## 🆘 Problemlösung

### Problem: Gespeicherte Rankings werden nicht angezeigt

**Lösung:**
1. Prüfe ob du im gleichen Browser bist (Chrome ≠ Firefox)
2. Prüfe ob du nicht im Inkognito-Modus bist
3. Prüfe ob der Browser-Cache gelöscht wurde

### Problem: Ranking lässt sich nicht laden

**Lösung:**
1. Lade die Seite neu (F5)
2. Prüfe die Browser-Konsole auf Fehler (F12)
3. Eventuell ist das gespeicherte Ranking beschädigt → Löschen

### Problem: "Daten löschen" funktioniert nicht

**Lösung:**
1. Stelle sicher, dass JavaScript aktiviert ist
2. Lade die Seite neu
3. Prüfe ob der Button richtig angeklickt wurde

## 🎉 Viel Erfolg!

Mit diesen neuen Features wird die Arbeit mit der Listenwahl-Ranking App noch effizienter und flexibler!

---

**Letzte Aktualisierung:** Version 1.1 - Dezember 2024
