# 📤 Anleitung: Projekt auf GitHub hochladen

Diese Anleitung zeigt dir zwei Methoden, um dein Listenwahl-Ranking Projekt auf GitHub zu veröffentlichen.

## 🎯 Methode 1: Webinterface (Einfachste Methode)

### Schritt 1: Repository erstellen

1. Gehe zu https://github.com und melde dich an
2. Klicke oben rechts auf das **+** Symbol
3. Wähle **"New repository"**
4. Fülle das Formular aus:
   - **Repository name**: `listenwahl-ranking`
   - **Description**: "Webapp zur Ermittlung der optimalen Reihenfolge bei Listenwahlen"
   - **Public** auswählen (für GitHub Pages)
   - ✅ **Add a README file** NICHT anklicken (wir haben bereits eine)
5. Klicke **"Create repository"**

### Schritt 2: Alle Dateien hochladen

1. Du siehst nun eine leere Repository-Seite
2. Klicke auf **"uploading an existing file"** (blauer Link im Text)
3. Öffne den Ordner `listenwahl-ranking` auf deinem Computer
4. Wähle ALLE Dateien aus:
   - `index.html`
   - `README.md`
   - `QUICKSTART.md`
   - `LICENSE`
   - `.gitignore`
   - `package.json`
5. Ziehe alle Dateien auf einmal in den Upload-Bereich
6. Warte bis alle Dateien hochgeladen sind
7. Schreibe als Commit message: `Initial commit - Listenwahl-Ranking Webapp`
8. Klicke **"Commit changes"**

### Schritt 3: GitHub Pages aktivieren

1. Klicke in deinem Repository auf **"Settings"** (oben in der Menüleiste)
2. Scrolle im linken Seitenmenü zu **"Pages"**
3. Unter **"Build and deployment"**:
   - Source: **Deploy from a branch**
   - Branch: **main** → **/ (root)** → **Save**
4. Warte 1-2 Minuten

### Schritt 4: Deine URL finden

1. Gehe zurück zu **Settings → Pages**
2. Du siehst oben eine grüne Box:
   ```
   Your site is published at https://[username].github.io/listenwahl-ranking/
   ```
3. Klicke auf die URL - deine Webapp ist jetzt live! 🎉

## 🖥️ Methode 2: Git Command Line (Fortgeschritten)

Wenn du Git auf deinem Computer installiert hast:

```bash
# 1. Repository initialisieren
cd listenwahl-ranking
git init

# 2. Alle Dateien hinzufügen
git add .

# 3. Ersten Commit erstellen
git commit -m "Initial commit - Listenwahl-Ranking Webapp"

# 4. Mit GitHub verbinden (ersetze [username])
git remote add origin https://github.com/[username]/listenwahl-ranking.git

# 5. Hochladen
git branch -M main
git push -u origin main
```

Danach GitHub Pages aktivieren wie in Methode 1, Schritt 3.

## 📝 Was macht welche Datei?

| Datei | Beschreibung |
|-------|-------------|
| `index.html` | ⭐ **WICHTIGSTE DATEI** - Die komplette Webapp |
| `README.md` | Projektbeschreibung und Dokumentation |
| `QUICKSTART.md` | Schnellstart-Anleitung für Anfänger |
| `LICENSE` | MIT-Lizenz für das Projekt |
| `.gitignore` | Sagt Git, welche Dateien ignoriert werden sollen |
| `package.json` | Optional: Für npm/Node.js Entwicklung |

## ✅ Checkliste nach dem Upload

- [ ] Alle 6 Dateien sind im Repository sichtbar
- [ ] README.md wird auf der Repository-Hauptseite angezeigt
- [ ] GitHub Pages ist aktiviert (Settings → Pages)
- [ ] Die URL funktioniert (nach 1-2 Minuten)
- [ ] Die Webapp lädt und zeigt das Formular

## 🔄 Änderungen vornehmen

### Via Web-Interface:

1. Gehe zu deinem Repository
2. Klicke auf die Datei, die du ändern möchtest (z.B. `index.html`)
3. Klicke auf das Stift-Symbol ✏️ oben rechts ("Edit this file")
4. Nimm deine Änderungen vor
5. Scrolle nach unten zu "Commit changes"
6. Gib eine Beschreibung ein (z.B. "Update Gewichtungen")
7. Klicke "Commit changes"
8. Warte 1-2 Minuten → Änderung ist online

### Via Git:

```bash
# Änderungen vornehmen, dann:
git add .
git commit -m "Beschreibung der Änderung"
git push
```

## 🌐 URL anpassen (Optional)

Du kannst auch eine eigene Domain verwenden:

1. Kaufe eine Domain (z.B. bei Namecheap, GoDaddy, Strato)
2. Settings → Pages → Custom domain
3. Gib deine Domain ein
4. Folge den DNS-Anweisungen

## 💡 Profi-Tipps

### Repository-Link im README ergänzen

Nachdem du hochgeladen hast, ändere in `package.json` und `README.md`:
```
https://github.com/yourusername/listenwahl-ranking.git
```
zu deiner echten URL:
```
https://github.com/[dein-username]/listenwahl-ranking.git
```

### Repository beschreiben

1. Gehe zur Repository-Hauptseite
2. Klicke auf das Zahnrad ⚙️ neben "About" (oben rechts)
3. Füge eine Beschreibung hinzu
4. Füge Topics hinzu: `ranking`, `voting`, `webapp`, `react`, `personnel`
5. Setze einen Haken bei "Use your GitHub Pages website"
6. Speichern

### README-Badge hinzufügen

Ersetze in `README.md` die Platzhalter:
```markdown
![Listenwahl-Ranking System](https://img.shields.io/badge/Version-1.0.0-blue.svg)
```

## ❓ Häufige Probleme

### "Failed to publish your site"
- Stelle sicher, dass `index.html` im Root-Verzeichnis liegt (nicht in einem Unterordner)
- Überprüfe, ob das Repository "Public" ist

### Seite zeigt 404
- Warte 5 Minuten und lade dann neu
- Stelle sicher, dass die Datei genau `index.html` heißt (Kleinschreibung!)
- Cache leeren: Strg + Shift + R (Windows) oder Cmd + Shift + R (Mac)

### Änderungen erscheinen nicht
- Warte 1-2 Minuten nach dem Commit
- Hard Reload im Browser: Strg + F5
- Inkognito-Modus verwenden zum Testen

### Repository ist leer
- Stelle sicher, dass du auf "Commit changes" geklickt hast
- Überprüfe, ob du im richtigen Repository bist

## 📞 Weitere Hilfe

- GitHub Docs: https://docs.github.com/pages
- GitHub Pages Status: https://www.githubstatus.com/
- Git Tutorial: https://git-scm.com/book/de/v2

## 🎉 Geschafft!

Deine Listenwahl-Ranking Webapp ist jetzt:
- ✅ Auf GitHub gesichert
- ✅ Öffentlich zugänglich
- ✅ Professionell dokumentiert
- ✅ Bereit zur Nutzung

Teile die URL mit deinen Kolleginnen und Kollegen! 🚀
