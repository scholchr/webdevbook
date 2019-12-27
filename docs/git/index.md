# Git

## Key Concepts

### Three (and a half) States of Git

* Working Directory
* Staging area: a pre-commit holding are
* Commit: Git repository (history)
* (Remote repository)

## Häufige Probleme

### Eine bestehende Datei oder ein Verzeichnis wurde per `.gitignore` ignoriert, taucht aber noch im Index als `untracked file` auf. TODO: mit bereits erfassten Dateien testen!

https://stackoverflow.com/questions/1274057/how-to-make-git-forget-about-a-file-that-was-tracked-but-is-now-in-gitignore

`.gitignore` sorgt nur dafür, dass keine neu hinzugefügten Dateien von Git erfasst werden. Bereits erfasst Dateien können mit dem Befehl `git rm --cached <file>` aus dem Index entfernt werden. Für Verzeichnisse lautet der Befehl `git rm -r --cached <folder>`

Achtung: Sollte die Datei bereits comittete sein entfernt der `git rm` Befehl zwar keine Dateien aus dem lokalen Working Directory, wohl aber aus dem Repository