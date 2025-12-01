# 📋 Changelog - Listenwahl-Ranking System

## Version 1.1.0 (01.12.2024)

### ✨ Neue Features

#### Speichern & Laden von Rankings
- **Mehrere Rankings erstellen**: Erstelle beliebig viele Rankings mit eigenem Namen
- **Lokale Speicherung**: Alle Rankings werden im Browser gespeichert (localStorage)
- **Persistenz**: Rankings bleiben auch nach Browser-Neustart erhalten
- **Übersichtliche Liste**: Alle gespeicherten Rankings mit Datum/Uhrzeit anzeigen
- **Schnelles Wechseln**: Mit einem Klick zwischen verschiedenen Rankings wechseln
- **Einzeln löschen**: Nicht mehr benötigte Rankings können gelöscht werden

#### Daten löschen
- **Pro Person**: Lösche alle Bewertungsdaten einer einzelnen Person
  - Basis-Daten (Name, Geschlecht, Alter, Mitgliedschaft) bleiben erhalten
  - Bewertungsdaten (Stimmen, Arbeitsgruppen, Pünktlichkeit, etc.) werden gelöscht
- **Alle Personen**: Lösche Bewertungsdaten aller 11 Personen auf einmal
- **Sicherheitsabfragen**: Verhindert versehentliches Löschen

#### Verbesserte Benutzeroberfläche
- **Pünktlichkeitsfelder**: Jedes Feld hat jetzt eine eigene Überschrift
  - "Sitzungsbeginn"
  - "Kurze Pause"
  - "Mittagspause"
- **Bessere Beispiele**: Platzhalter zeigen typische Eingabewerte
- **Übersichtlichere Struktur**: Hauptüberschrift + individuelle Labels

### 🔧 Verbesserungen

- **Icons hinzugefügt**: Save, Trash, FolderOpen für bessere Visualisierung
- **Button-Styles**: Einheitliches Design für Primary, Secondary und Danger-Buttons
- **Hover-Effekte**: Gespeicherte Rankings heben sich beim Überfahren hervor
- **Responsive Layout**: Speichern/Laden-Bereich passt sich an Bildschirmgröße an

### 📚 Dokumentation

- **NEUE-FEATURES.md**: Ausführliche Anleitung zu allen neuen Features
- **README.md aktualisiert**: Version 1.1 Features hinzugefügt
- **Use Cases**: Praktische Anwendungsbeispiele dokumentiert
- **FAQ erweitert**: Häufige Fragen zu Speichern/Laden beantwortet

### 🐛 Bugfixes

- Keine Bugs in dieser Version (neue Features)

---

## Version 1.0.0 (01.12.2024)

### 🎉 Erste Veröffentlichung

#### Kernfunktionen
- **11 Kandidaten**: Eingabe für genau 11 Personen
- **10 Bewertungskriterien**: 
  - Stimmenzahl letzte Wahl
  - Arbeitsgruppen
  - Sitzungsteilnahme
  - Pünktlichkeit (3x)
  - Freistellungswünsche (2x)
  - Mitgliedschaftsdauer
  - Alter

#### Gewichtungssystem
- **Flexible Prozentverteilung**: Alle Kriterien individuell gewichtbar
- **Live-Anzeige**: Verbleibende Prozente werden angezeigt
- **Standard-Gewichtungen**: Sinnvolle Voreinstellungen

#### Ranking-Logik
- **Automatische Berechnung**: Sofortige Aktualisierung bei Änderungen
- **Normalisierung**: Faire Bewertung über alle Kriterien
- **Parität-Regeln**: 
  - Weiblich vor männlich bei Punktgleichheit
  - Unter 40 vor über 40 bei Punktgleichheit

#### Design
- **Modernes Dark Theme**: Professionelles dunkles Design
- **Animationen**: Smooth Hover-Effekte und Fade-In-Animationen
- **Responsive**: Funktioniert auf allen Geräten
- **Visuelle Highlights**: Top 3 mit Gold/Silber/Bronze-Badges

#### Dokumentation
- **README.md**: Vollständige Projektdokumentation
- **QUICKSTART.md**: 5-Schritte GitHub Pages Anleitung
- **GITHUB-UPLOAD.md**: Detaillierte Upload-Anleitung
- **START-HIER.md**: Einstiegshilfe für Nutzer

---

## Roadmap (mögliche zukünftige Features)

### Version 1.2 (geplant)
- [ ] Export/Import als JSON-Datei
- [ ] PDF-Export des Rankings
- [ ] Druckansicht optimieren
- [ ] Dunkler/Heller Modus Toggle

### Version 1.3 (Ideen)
- [ ] Vergleichsansicht mehrerer Rankings
- [ ] Detailansicht einzelner Kriterien
- [ ] Graphische Visualisierung der Scores
- [ ] Anpassbare Anzahl Personen (nicht fix 11)

### Version 2.0 (langfristig)
- [ ] Cloud-Synchronisation (optional)
- [ ] Mehrere Benutzer/Teams
- [ ] Versionsverwaltung für Rankings
- [ ] Mobile App (PWA)

---

## Mitwirkende

Entwickelt für effiziente Gremienarbeit in Personalräten und ähnlichen Organisationen.

## Lizenz

MIT License - Siehe LICENSE Datei für Details
