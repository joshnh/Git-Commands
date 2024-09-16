
Git-Befehle
============

## Übersetzte Versionen
- [Versão em português](READMEpt.md)
- [Versión en español](READMEes.md)
- [Türkçe versiyon](READMEtr.md)
- [বাংলা সংস্করণ](READMEbn.md)
- [हिन्दी अनुवाद](READMEhi.md)
- [العربية](READMEar.md)

___

_Eine Liste meiner häufig verwendeten Git-Befehle_

*Wenn Sie an meinen Git-Aliasen interessiert sind, schauen Sie sich mein `.bash_profile` hier an: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

--

### Projekte Abrufen & Erstellen

| Befehl | Beschreibung |
| ------- | ----------- |
| `git init` | Ein lokales Git-Repository initialisieren |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Eine lokale Kopie eines Remote-Repository erstellen |

### Grundlegendes Snapshoten

| Befehl | Beschreibung |
| ------- | ----------- |
| `git status` | Status überprüfen |
| `git add [file-name.txt]` | Eine Datei zum Staging-Bereich hinzufügen |
| `git add -A` | Alle neuen und geänderten Dateien zum Staging-Bereich hinzufügen |
| `git commit -m "[commit message]"` | Änderungen committen |
| `git rm -r [file-name.txt]` | Eine Datei (oder einen Ordner) entfernen |

### Branching & Merging

| Befehl | Beschreibung |
| ------- | ----------- |
| `git branch` | Branches auflisten (der Stern zeigt den aktuellen Branch an) |
| `git branch -a` | Alle Branches auflisten (lokal und remote) |
| `git branch [branch name]` | Einen neuen Branch erstellen |
| `git branch -d [branch name]` | Einen Branch löschen |
| `git push origin --delete [branch name]` | Einen Remote-Branch löschen |
| `git checkout -b [branch name]` | Einen neuen Branch erstellen und zu ihm wechseln |
| `git checkout -b [branch name] origin/[branch name]` | Einen Remote-Branch klonen und zu ihm wechseln |
| `git branch -m [old branch name] [new branch name]` | Einen lokalen Branch umbenennen |
| `git checkout [branch name]` | Zu einem Branch wechseln |
| `git checkout -` | Zum zuletzt ausgecheckten Branch wechseln |
| `git checkout -- [file-name.txt]` | Änderungen an einer Datei verwerfen |
| `git merge [branch name]` | Einen Branch in den aktiven Branch mergen |
| `git merge [source branch] [target branch]` | Einen Branch in einen Ziel-Branch mergen |
| `git stash` | Änderungen in einem verschmutzten Arbeitsverzeichnis stashen |
| `git stash clear` | Alle gestashten Einträge entfernen |

### Projekte Teilen & Aktualisieren

| Befehl | Beschreibung |
| ------- | ----------- |
| `git push origin [branch name]` | Einen Branch in Ihr Remote-Repository pushen |
| `git push -u origin [branch name]` | Änderungen in das Remote-Repository pushen (und den Branch merken) |
| `git push` | Änderungen in das Remote-Repository pushen (gemerkter Branch) |
| `git push origin --delete [branch name]` | Einen Remote-Branch löschen |
| `git pull` | Lokales Repository auf den neuesten Commit aktualisieren |
| `git pull origin [branch name]` | Änderungen aus dem Remote-Repository pullen |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Ein Remote-Repository hinzufügen |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Den Ursprung eines Repositorys auf SSH setzen |

### Überprüfung & Vergleich

| Befehl | Beschreibung |
| ------- | ----------- |
| `git log` | Änderungen anzeigen |
| `git log --summary` | Änderungen anzeigen (detailliert) |
| `git log --oneline` | Änderungen anzeigen (kurz) |
| `git diff [source branch] [target branch]` | Änderungen vor dem Mergen vorschauen |
