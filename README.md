# Listenwahl-Ranking System

Eine professionelle Webanwendung zur Ermittlung der optimalen Reihenfolge bei Listenwahlen basierend auf gewichteten Kriterien.

![Listenwahl-Ranking System](https://img.shields.io/badge/Version-1.1.0-blue.svg)
![React](https://img.shields.io/badge/React-18-61dafb.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

## 🎯 Funktionen

- **11 Kandidaten verwalten**: Umfassende Dateneingabe für alle relevanten Kriterien
- **Flexible Gewichtung**: Alle 10 Bewertungskriterien sind individuell anpassbar
- **Intelligentes Ranking**: Automatische Berechnung mit Parität-Regeln bei Punktgleichheit
- **💾 Speichern & Laden**: Erstelle mehrere Rankings und speichere sie lokal im Browser
- **🗑️ Daten löschen**: Lösche Bewertungsdaten einzelner oder aller Personen
- **Responsive Design**: Funktioniert auf Desktop, Tablet und Mobile
- **Moderne UI**: Dunkles Theme mit Animationen und professionellen Visualisierungen

## ✨ Neu in Version 1.1

- **Speichern/Laden-Funktion**: Erstelle mehrere Rankings mit eigenem Namen und wechsle zwischen ihnen
- **Löschen-Buttons**: 
  - Einzelne Personen: Lösche alle Bewertungsdaten (Name, Geschlecht, Alter, Mitgliedschaft bleiben erhalten)
  - Alle Personen: Lösche alle Bewertungsdaten auf einmal
- **Verbesserte Pünktlichkeitsfelder**: Klare Überschriften für Sitzungsbeginn, kurze Pause und Mittagspause
- **Lokaler Speicher**: Alle gespeicherten Rankings bleiben auch nach Browser-Neustart erhalten

## 📋 Bewertungskriterien

Das System bewertet Kandidaten nach folgenden Kriterien:

1. **Stimmenzahl letzte Wahl** (Standard: 10%)
2. **Anzahl Arbeitsgruppen** (Standard: 10%)
3. **Sitzungsteilnahme** (Standard: 10%)
4. **Pünktlichkeit Sitzungsbeginn** (Standard: 10%)
5. **Pünktlichkeit kurze Pausen** (Standard: 5%)
6. **Pünktlichkeit Mittagspause** (Standard: 10%)
7. **Teilfreistellung gewünscht** (Standard: 10%)
8. **Vollfreistellung gewünscht** (Standard: 10%)
9. **Mitgliedschaftsdauer** (Standard: 15%)
10. **Alter** (Standard: 10%)

### Parität-Regeln bei Punktgleichheit

Bei identischer Punktzahl werden folgende Kriterien in dieser Reihenfolge angewendet:

1. **Weiblich vor männlich**
2. **Jünger als 40 Jahre vor älter als 40 Jahre**

## 🚀 Schnellstart

### Option 1: Direkter Start (einfachste Methode)

1. Lade die `index.html` Datei herunter
2. Öffne die Datei in einem modernen Webbrowser
3. Fertig! Die App läuft sofort ohne Installation

### Option 2: GitHub Pages Deployment

1. **Repository erstellen**:
   ```bash
   # Erstelle ein neues Repository auf GitHub
   # z.B. "listenwahl-ranking"
   ```

2. **Dateien hochladen**:
   - Gehe zu deinem GitHub Repository
   - Klicke auf "Add file" → "Upload files"
   - Ziehe die `index.html` Datei in das Upload-Feld
   - Commit die Änderungen

3. **GitHub Pages aktivieren**:
   - Gehe zu "Settings" → "Pages"
   - Unter "Source" wähle "main" Branch
   - Wähle "/ (root)" als Ordner
   - Klicke auf "Save"

4. **Zugriff auf deine App**:
   - Nach wenigen Minuten ist deine App unter folgender URL erreichbar:
   - `https://[dein-username].github.io/[repository-name]/`

### Option 3: Lokaler Webserver (für Entwicklung)

```bash
# Mit Python
python -m http.server 8000

# Mit Node.js
npx http-server

# Dann öffne im Browser: http://localhost:8000
```

## 📝 Verwendung

### 1. Gewichtungen anpassen

Klicke auf "Gewichtungen anpassen" um:
- Die Prozentanteile der einzelnen Kriterien zu ändern
- Die verbleibenden verfügbaren Prozentpunkte zu sehen
- Sicherzustellen, dass die Summe 100% beträgt

### 2. Kandidaten eingeben

Für jede der 11 Personen kannst du eingeben:
- **Persönliche Daten**: Vorname, Nachname, Geschlecht, Alter
- **Wahlhistorie**: Stimmenzahl bei der letzten Wahl
- **Engagement**: Anzahl Arbeitsgruppen, Sitzungsteilnahme
- **Pünktlichkeit**: 
  - 0 = pünktlich
  - Negative Werte = Minuten zu spät (z.B. -5, -10, -15)
  - Positive Werte = Minuten zu früh
- **Freistellungswünsche**: Teilfreistellung und/oder Vollfreistellung
- **Erfahrung**: Mitgliedschaftsdauer in Jahren und Monaten

### 3. Ranking ansehen

Das Ranking wird automatisch aktualisiert und zeigt:
- Position mit visueller Hervorhebung (Gold, Silber, Bronze für Top 3)
- Gesamtpunktzahl
- Fortschrittsbalken zur Visualisierung
- Relevante Kandidateninformationen

## 🎨 Pünktlichkeits-Bewertung

Die Pünktlichkeit wird wie folgt bewertet:

| Zeitabweichung | Punktzahl |
|---------------|-----------|
| Pünktlich oder früh (≥ 0 Min) | 100 Punkte |
| Bis 5 Min zu spät (-1 bis -5 Min) | 75 Punkte |
| 5-10 Min zu spät (-6 bis -10 Min) | 50 Punkte |
| Mehr als 10 Min zu spät (< -10 Min) | 25 Punkte |

## 🛠️ Technische Details

### Verwendete Technologien

- **React 18**: UI-Framework
- **Babel Standalone**: JSX-Transformation im Browser
- **CSS3**: Moderne Animationen und Gradients
- **Google Fonts**: Space Grotesk & JetBrains Mono

### Browser-Kompatibilität

- Chrome/Edge: ✅ Vollständig unterstützt
- Firefox: ✅ Vollständig unterstützt
- Safari: ✅ Vollständig unterstützt
- Opera: ✅ Vollständig unterstützt

### Datenspeicherung

Die Anwendung speichert **keine Daten** auf einem Server. Alle Eingaben bleiben lokal im Browser und werden beim Neuladen der Seite zurückgesetzt.

## 📦 Repository-Struktur

```
listenwahl-ranking/
│
├── index.html          # Hauptanwendung (alle Komponenten in einer Datei)
├── README.md           # Diese Dokumentation
└── .gitignore         # Git-Ausschlussliste
```

## 🔒 Datenschutz

- Keine Server-Kommunikation
- Keine Cookies
- Keine lokale Speicherung
- Alle Daten bleiben im Browser-RAM
- DSGVO-konform durch Design

## 🤝 Beitragen

Verbesserungsvorschläge und Bug-Reports sind willkommen!

1. Fork das Repository
2. Erstelle einen Feature-Branch (`git checkout -b feature/AmazingFeature`)
3. Committe deine Änderungen (`git commit -m 'Add some AmazingFeature'`)
4. Push zum Branch (`git push origin feature/AmazingFeature`)
5. Öffne einen Pull Request

## 📄 Lizenz

Dieses Projekt ist unter der MIT-Lizenz lizenziert - siehe LICENSE Datei für Details.

## 👤 Autor

Entwickelt für die Verwendung in Personalräten und ähnlichen Gremien.

## 🙏 Danksagungen

- React Team für das großartige Framework
- Google Fonts für die Schriftarten
- Alle Mitwirkenden und Tester

## 📞 Support

Bei Fragen oder Problemen:
- Öffne ein Issue auf GitHub
- Kontaktiere den Repository-Betreuer

---

**Hinweis**: Diese Anwendung dient als Hilfsmittel zur objektiven Bewertung. Die finale Entscheidung liegt immer bei den zuständigen Gremien und muss den jeweiligen rechtlichen Rahmenbedingungen entsprechen.
