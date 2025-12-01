# 🚀 Schnellstart: GitHub Pages Deployment

Diese Anleitung zeigt dir in 5 einfachen Schritten, wie du die Listenwahl-Ranking Webapp auf GitHub Pages veröffentlichst.

## ⚡ Voraussetzungen

- Ein GitHub-Account (kostenlos unter https://github.com)
- Die `index.html` Datei aus diesem Repository

## 📝 Schritt-für-Schritt Anleitung

### Schritt 1: Neues Repository erstellen

1. Gehe zu GitHub.com und melde dich an
2. Klicke auf das **"+"** Icon oben rechts
3. Wähle **"New repository"**
4. Gib einen Namen ein (z.B. `listenwahl-ranking`)
5. Wähle **"Public"** (für GitHub Pages erforderlich)
6. Klicke auf **"Create repository"**

### Schritt 2: Datei hochladen

1. In deinem neuen Repository klicke auf **"uploading an existing file"**
2. Ziehe die `index.html` Datei in das Upload-Feld
   - Oder klicke auf "choose your files" und wähle sie aus
3. Schreibe unten eine Commit-Nachricht (z.B. "Initial commit")
4. Klicke auf **"Commit changes"**

### Schritt 3: GitHub Pages aktivieren

1. Klicke in deinem Repository auf **"Settings"** (oben rechts)
2. Scrolle im linken Menü zu **"Pages"**
3. Unter "Source" wähle:
   - Branch: **main** (oder master)
   - Folder: **/ (root)**
4. Klicke auf **"Save"**

### Schritt 4: Warten und URL finden

1. Warte 1-2 Minuten (GitHub baut deine Seite)
2. Gehe zurück zu **Settings → Pages**
3. Du siehst eine grüne Box mit der URL:
   ```
   Your site is published at https://[dein-username].github.io/listenwahl-ranking/
   ```

### Schritt 5: Webapp nutzen! 🎉

1. Klicke auf die URL oder kopiere sie
2. Die Webapp ist jetzt online und nutzbar!
3. Du kannst die URL mit anderen teilen

## 🔄 Änderungen vornehmen

Wenn du später etwas ändern möchtest:

1. Gehe zu deinem Repository
2. Klicke auf `index.html`
3. Klicke auf das Stift-Symbol (✏️) oben rechts
4. Nimm deine Änderungen vor
5. Scrolle nach unten und klicke "Commit changes"
6. Nach 1-2 Minuten ist die Änderung online

## 💡 Tipps

- Die URL kannst du als Lesezeichen speichern
- Du kannst auch eine eigene Domain verbinden (siehe GitHub Docs)
- Die Webapp funktioniert auch offline nach dem ersten Laden
- Alle Daten bleiben lokal im Browser

## ❓ Probleme?

### Die Seite zeigt nur "404"
- Warte noch 2-3 Minuten, GitHub braucht Zeit zum Deployen
- Überprüfe in Settings → Pages ob die Seite aktiviert ist
- Stelle sicher, dass die Datei `index.html` heißt (nicht `index.htm`)

### Die Seite wird nicht aktualisiert
- Leere deinen Browser-Cache (Strg + Shift + R)
- Warte 1-2 Minuten nach dem Commit

### Die Seite ist leer
- Überprüfe ob die `index.html` Datei vollständig hochgeladen wurde
- Öffne die Entwickler-Konsole (F12) und suche nach Fehlern

## 🎯 Fertig!

Deine Listenwahl-Ranking Webapp ist jetzt online und kann von jedem mit der URL genutzt werden!

---

**Hinweis**: Diese Anleitung ist für absolute Anfänger. Wenn du mit Git vertraut bist, kannst du natürlich auch `git clone`, `git add`, `git commit` und `git push` verwenden.
