# Git & GitHub Tutorial

## Inhaltsverzeichnis - test 2

- [Git \& GitHub Tutorial](#git--github-tutorial)
  - [Inhaltsverzeichnis - test 2](#inhaltsverzeichnis---test-2)
    - [**Chaos im Projekt? Git \& GitHub sind die Lösung!**](#chaos-im-projekt-git--github-sind-die-lösung)
    - [**Was ist Git?**](#was-ist-git)
    - [**Was ist GitHub?**](#was-ist-github)
    - [**Warum sollte man Git \& GitHub nutzen?**](#warum-sollte-man-git--github-nutzen)
    - [**Vorteile von GitHub:**](#vorteile-von-github)
    - [**Warum ist Git heute so wichtig?**](#warum-ist-git-heute-so-wichtig)
    - [**Wie funktioniert Git?**](#wie-funktioniert-git)
    - [**Erster Commit mit Git**](#erster-commit-mit-git)
    - [**Änderungen verwalten mit Git**](#änderungen-verwalten-mit-git)
    - [**GitHub-Konto erstellen \& Repository veröffentlichen**](#github-konto-erstellen--repository-veröffentlichen)
    - [**Zusammenarbeit im Team mit Git \& GitHub**](#zusammenarbeit-im-team-mit-git--github)
    - [**Warum Branches verwenden?**](#warum-branches-verwenden)
    - [**Branches in der Praxis verwenden**](#branches-in-der-praxis-verwenden)
    - [**Merge \& Zusammenarbeit**](#merge--zusammenarbeit)
    - [**Commits bearbeiten, zurücknehmen \& wiederherstellen**](#commits-bearbeiten-zurücknehmen--wiederherstellen)
    - [**Commits löschen oder rückgängig machen**](#commits-löschen-oder-rückgängig-machen)
    - [**Sicherer Weg: `git revert` verwenden**](#sicherer-weg-git-revert-verwenden)
    - [**Gelöschte Commits wiederherstellen**](#gelöschte-commits-wiederherstellen)
    - [**Was ist ein Fork?**](#was-ist-ein-fork)
    - [**Feature entwickeln \& Commiten**](#feature-entwickeln--commiten)
    - [**Was ist ein Pull Request (PR)?**](#was-ist-ein-pull-request-pr)
    - [**Review \& Merge-Prozess**](#review--merge-prozess)
    - [**Warum ist das wichtig?**](#warum-ist-das-wichtig)
    - [**Was ist ein GitHub Issue?**](#was-ist-ein-github-issue)
    - [**Gutes Issue erstellen**](#gutes-issue-erstellen)
    - [**Issue lösen – Schritt für Schritt**](#issue-lösen--schritt-für-schritt)
    - [**Pull Request (PR) erstellen**](#pull-request-pr-erstellen)
    - [**Merge-Strategien im Überblick**](#merge-strategien-im-überblick)
    - [**Vollständiger Workflow mit CLI oder Web**](#vollständiger-workflow-mit-cli-oder-web)
    - [**Was ist ein Merge?**](#was-ist-ein-merge)
    - [**Merge mit --no-ff Option**](#merge-mit---no-ff-option)
    - [**Was ist Rebase?**](#was-ist-rebase)
    - [**Unterschied: Merge vs. Rebase**](#unterschied-merge-vs-rebase)
    - [**Wann Rebase, wann Merge?**](#wann-rebase-wann-merge)
    - [**Best Practices im Team**](#best-practices-im-team)
    - [**Was ist `git stash`?**](#was-ist-git-stash)
    - [**Typisches Szenario**](#typisches-szenario)
    - [**Wichtige `stash`-Befehle**](#wichtige-stash-befehle)
    - [**Was passiert bei einem Merge-Konflikt nach `stash`?**](#was-passiert-bei-einem-merge-konflikt-nach-stash)
    - [**Grenzen von `stash`**](#grenzen-von-stash)
    - [**Was ist `git worktree`?**](#was-ist-git-worktree)
    - [**Warum `worktree` statt `stash`?**](#warum-worktree-statt-stash)
    - [**Beispiel: Zwei neue Features**](#beispiel-zwei-neue-features)
    - [**Entwicklung \& Zusammenführen**](#entwicklung--zusammenführen)
- [(dein Code)](#dein-code)
  - [**Merge oder Rebase?**](#merge-oder-rebase)
    - [**Problem: Große Dateien in GitHub**](#problem-große-dateien-in-github)
    - [**Lösung: Git LFS (Large File Storage)**](#lösung-git-lfs-large-file-storage)
    - [**Git LFS einrichten \& verwenden**](#git-lfs-einrichten--verwenden)
    - [**Projekt klonen mit LFS-Dateien**](#projekt-klonen-mit-lfs-dateien)
    - [**Vorteile von Git LFS**](#vorteile-von-git-lfs)
    - [**Was kommt als Nächstes?**](#was-kommt-als-nächstes)
    - [**Problem: Sensible Daten \& große Dateien in der Git-Historie**](#problem-sensible-daten--große-dateien-in-der-git-historie)
    - [**Lösung: `git filter-repo`**](#lösung-git-filter-repo)
    - [**Große Dateien aus Git entfernen**](#große-dateien-aus-git-entfernen)
    - [**API-Schlüssel ersetzen**](#api-schlüssel-ersetzen)
    - [**Wichtige Hinweise**](#wichtige-hinweise)
    - [**Fazit**](#fazit)
    - [**Was ist ein Git Submodul?**](#was-ist-ein-git-submodul)
    - [**Warum Submodule verwenden?**](#warum-submodule-verwenden)
    - [**Beispiel: Mathematischer Parser als Submodul**](#beispiel-mathematischer-parser-als-submodul)
    - [**Submodul updaten \& verwalten**](#submodul-updaten--verwalten)
    - [**Submodul wieder entfernen**](#submodul-wieder-entfernen)
    - [**Was ist ein Git Subtree?**](#was-ist-ein-git-subtree)
    - [**Submodule vs. Subtree**](#submodule-vs-subtree)
    - [**Subtree hinzufügen – Beispiel**](#subtree-hinzufügen--beispiel)
    - [**Subtree verwenden \& verwalten**](#subtree-verwenden--verwalten)
    - [**Vorteile von Git Subtree**](#vorteile-von-git-subtree)
    - [**Was ist `git bundle`?**](#was-ist-git-bundle)
    - [**Warum `git bundle` nutzen?**](#warum-git-bundle-nutzen)
    - [**Repo als Bundle speichern**](#repo-als-bundle-speichern)
    - [**Einsatzmöglichkeiten von `git bundle`**](#einsatzmöglichkeiten-von-git-bundle)
    - [**Was ist ein Git Patch?**](#was-ist-ein-git-patch)
    - [**Patch-Datei erstellen**](#patch-datei-erstellen)
    - [**Patch anwenden**](#patch-anwenden)
    - [**Wann Git Patch verwenden?**](#wann-git-patch-verwenden)
    - [**Was ist GitHub Actions?**](#was-ist-github-actions)
    - [**Warum GitHub Actions verwenden?**](#warum-github-actions-verwenden)
    - [**Beispiel: Super-Linter einrichten**](#beispiel-super-linter-einrichten)
    - [**Was macht der Linter?**](#was-macht-der-linter)
    - [**Fehler erkennen \& beheben**](#fehler-erkennen--beheben)
    - [**Was sind Git Hooks?**](#was-sind-git-hooks)
    - [**Warum Git Hooks verwenden?**](#warum-git-hooks-verwenden)
    - [**Beispiele für wichtige Hooks**](#beispiele-für-wichtige-hooks)
    - [**Commit-Message-Format prüfen**](#commit-message-format-prüfen)
    - [**Automatisierung im Team**](#automatisierung-im-team)
    - [**Was ist die GitHub API?**](#was-ist-die-github-api)
    - [**Voraussetzung: Token erstellen**](#voraussetzung-token-erstellen)
    - [**API-Befehle ausführen (z. B. mit `curl`)**](#api-befehle-ausführen-zb-mit-curl)
    - [**Was ist mit der API möglich?**](#was-ist-mit-der-api-möglich)
    - [**Was ist Git eigentlich?**](#was-ist-git-eigentlich)
    - [**GitHub**](#github)
    - [**GitLab**](#gitlab)
    - [**Bitbucket**](#bitbucket)
    - [**Azure DevOps**](#azure-devops)
    - [**AWS CodeCommit**](#aws-codecommit)
    - [**Vergleich – Wann was nutzen?**](#vergleich--wann-was-nutzen)
    - [**Git Workflows – Übersicht**](#git-workflows--übersicht)
    - [**1. GitHub Flow**](#1-github-flow)
    - [**2. Git Flow**](#2-git-flow)
    - [**3. Fork Workflow**](#3-fork-workflow)
    - [**4. Trunk Based Development**](#4-trunk-based-development)
    - [**5. GitLab Flow**](#5-gitlab-flow)
    - [**6. Release Flow (Microsoft Style)**](#6-release-flow-microsoft-style)
    - [**Vergleich \& Empfehlung**](#vergleich--empfehlung)
    - [**GitHub Projects – Planung \& Nachverfolgung**](#github-projects--planung--nachverfolgung)
    - [**1. Projekt anlegen**](#1-projekt-anlegen)
    - [**2. Aufgaben verwalten**](#2-aufgaben-verwalten)
    - [**3. Tabellenansicht**](#3-tabellenansicht)
    - [**4 Kanban Board**](#4-kanban-board)
    - [**5. Vorteile**](#5-vorteile)
    - [**Gelernte Inhalte festigen – Git \& GitHub effektiv anwenden**](#gelernte-inhalte-festigen--git--github-effektiv-anwenden)
    - [**Wie bleibt das alles im Kopf?**](#wie-bleibt-das-alles-im-kopf)
    - [**Simuliere echte Beiträge**](#simuliere-echte-beiträge)
    - [**Wiederholung macht Meister**](#wiederholung-macht-meister)
    - [**Zusammenführung**](#zusammenführung)

### **Chaos im Projekt? Git & GitHub sind die Lösung!**

🔧 In einem Teamprojekt kann es schnell unübersichtlich werden:  
– Wer hat was geändert?  
– Eine Datei wurde versehentlich gelöscht – und jetzt?  
– Zwei Personen arbeiten an derselben Datei – wessen Code zählt?

💡 Genau hier setzt diese Schulung an:  
Du lernst Git & GitHub **von Grund auf bis zum Expertenniveau** – praxisnah und verständlich.

📚 **Was du lernen wirst:**  
– Änderungen verfolgen & rückgängig machen  
– Code-Konflikte vermeiden und lösen  
– Im Team organisiert und stressfrei arbeiten  
– Projekte versionieren, sichern und veröffentlichen  
– Automatisierung und Zusammenarbeit effizient gestalten

✅ Am Ende kannst du ein komplettes Projekt professionell mit Git verwalten – sicher, strukturiert und teamfähig.

### **Was ist Git?**

Git ist ein Versionskontrollsystem, mit dem du verschiedene Versionen deiner Dateien lokal speichern und verwalten kannst. Du kannst jederzeit zu einer älteren Version zurückkehren.

### **Was ist GitHub?**

GitHub ist eine Online-Plattform, auf der du deine mit Git verwalteten Projekte speichern, teilen und gemeinsam mit anderen bearbeiten kannst.

### **Warum sollte man Git & GitHub nutzen?**  

Ohne Git ist die Arbeit fehleranfällig:  
– Änderungen gehen verloren  
– Fehler lassen sich schwer rückgängig machen  
– Teamarbeit wird chaotisch

Mit Git & GitHub kannst du:  
– Fehler leicht korrigieren  
– Änderungen nachvollziehen  
– Konfliktfrei im Team arbeiten

### **Vorteile von GitHub:**  

– Weltweit größte Open-Source-Plattform  
– Projekte veröffentlichen & Beiträge zu anderen leisten  
– Eigene Arbeit sichtbar machen (auch für Arbeitgeber)

### **Warum ist Git heute so wichtig?**  

Git-Kenntnisse sind in der Softwarebranche Standard. Viele Unternehmen nutzen es – also ist es ein großer Pluspunkt in deiner Entwicklerlaufbahn!

### **Wie funktioniert Git?**

🔹 Git speichert **Dateiversionen** nicht direkt, sondern in mehreren Schritten:

1. **Working Directory (Arbeitsverzeichnis):**  
   Hier erstellst, änderst oder löschst du Dateien. Git verfolgt sie noch nicht automatisch.

2. **Staging Area (Zwischenspeicher):**  
   Nur **fertige und speicherbereite Änderungen** werden hier hinzugefügt.  
   → So behältst du die Kontrolle und vermeidest Chaos.

3. **Repository (Lokales Git-Depot):**  
   Von der Staging Area werden die Änderungen ins Repository übernommen (= Commit).  
   Git erstellt dabei mit einem **SHA-1-Hash** einen eindeutigen Fingerabdruck für jede Version.

🔁 **Zurückspringen im Verlauf:**  
Alle Versionen sind wie eine Kette miteinander verbunden. Du kannst jederzeit zu einem früheren Stand zurückkehren.

🌍 **Zusammenarbeit mit GitHub:**  
Durch das Hochladen ins **Remote-Repository (z. B. GitHub)** können Teammitglieder die neuesten Änderungen abrufen, weiterentwickeln und gemeinsam am Projekt arbeiten.

### **Erster Commit mit Git**

🔧 **Git installieren & starten:**  
– Git von der offiziellen Website herunterladen  
– Git Bash (Terminal) öffnen – ideal für Git-Kommandos unter Windows

📁 **Projektordner initialisieren:**  
– Mit `cd` ins Arbeitsverzeichnis wechseln  
– `git init` ausführen → Git erstellt einen `.git`-Ordner zur Versionskontrolle

📄 **Dateien verfolgen:**  
– `git status` zeigt: nicht verfolgte Dateien = **rot**  
– `git add dateiname` → Datei wird zur Staging Area hinzugefügt = **grün**  
– `git add .` → alle Änderungen auf einmal hinzufügen

👤 **Nutzerinformationen konfigurieren:**  
– `git config --global user.name "Dein Name"`  
– `git config --global user.email "deine@email.com"`  
→ Git weiß, wer Änderungen gemacht hat (wichtig für Commits und Zusammenarbeit)

💾 **Commit durchführen:**  
– `git commit -m "Nachricht"` → Änderungen dauerhaft speichern  
– Jeder Commit bekommt eine eindeutige ID (SHA-1)

🕘 **Verlauf anzeigen:**  
– `git log` zeigt Commit-Historie mit ID, Nachricht und Zeit

### **Änderungen verwalten mit Git**

🔍 **Was hat sich geändert?**  
– `git diff` zeigt geänderte Zeilen:  
 🟩 grün = hinzugefügt 🟥 rot = gelöscht  
– `git diff datei.txt` → nur bestimmte Datei prüfen

📥 **Änderungen zur Staging Area hinzufügen:**  
– `git add .` → alle Änderungen  
– Danach zeigt `git diff` keine Änderungen mehr, da sie jetzt im Zwischenspeicher sind  
– Mit `git diff --staged` sieht man die Inhalte in der Staging Area

↩️ **Änderungen zurücknehmen:**  
– Arbeitsverzeichnis zurücksetzen (eine Datei):  
 `git restore datei.txt`  
– Alle Änderungen im Arbeitsverzeichnis zurücknehmen:  
 `git restore .`

📤 **Staging Area zurücksetzen:**  
– Einzelne Datei entfernen:  
 `git reset datei.txt`  
– Alle Dateien entfernen:  
 `git reset`  
📝 Achtung: Änderungen im Arbeitsverzeichnis bleiben erhalten!

📌 Wenn Änderungen **ganz gelöscht** werden sollen:  
→ Danach erneut `git restore` verwenden

### **GitHub-Konto erstellen & Repository veröffentlichen**

👤 **GitHub-Konto anlegen:**  
– Verwende dieselbe E-Mail wie bei `git config`  
– Benutzername & Passwort wählen  
– Verifizierung abschließen → Konto ist bereit

⚙️ **Nutzerinformationen verwalten:**  
– Ändern: `git config --global user.name "Neuer Name"`  
– Löschen: `git config --unset --global user.email`

📁 **Lokales Repository vorbereiten:**  
– In Projektordner wechseln  
– `git init` → Git-Repository starten  
– `git add .` → alle Dateien zur Staging Area hinzufügen  
– `git commit -m "Erster Commit"` → Änderungen speichern

☁️ **GitHub-Repository erstellen & verknüpfen:**  
– Auf GitHub neues Repository anlegen  
– Link kopieren und verknüpfen:  
  `git remote add origin [Repo-Link]`  
– Verbindung aufbauen & pushen:  
  `git push -u origin master`  
→ `-u` merkt sich die Verbindung für zukünftige Pushes

🔐 **Authentifizierung:**  
– Einloggen per Browser, Token oder Code  
→ Danach ist das lokale Projekt auf GitHub verfügbar!

### **Zusammenarbeit im Team mit Git & GitHub**

👥 **Teammitglied zum Projekt hinzufügen:**  
– Auf GitHub unter *Settings > Collaborators*  
– Benutzername eingeben → Einladung senden  
– Nach Annahme kann die Person am Projekt mitarbeiten

💻 **Projekt auf den eigenen Rechner klonen:**  
– Terminal öffnen → `git clone [Repo-Link]`  
– Projekt lokal verfügbar → bereit zur Entwicklung

📤 **Eigene Änderungen hochladen:**  
– Datei erstellen oder bearbeiten  
– `git add`, `git commit -m "Nachricht"`, `git push`  
→ Änderungen gehen ins Remote-Repo (GitHub)

📥 **Änderungen vom Team abrufen:**  
– `git fetch` → lädt Updates, aber noch nicht sichtbar  
– `git merge` → integriert Änderungen in das Arbeitsverzeichnis  
– Alternativ: `git pull` → beides in einem Schritt

⚠️ **Push-Fehler?**  
– Wenn Remote-Repo neuer ist als lokales:  
→ `git pull` vorher nötig  
→ Konfliktlösung ggf. mit Merge-Commit (Editor mit `:q` schließen)

📚 **Verlauf & Kontrolle:**  
– `git log` zeigt alle Commits  
→ Änderungen sind nachvollziehbar & sauber dokumentiert

### **Warum Branches verwenden?**

🌱 **Stabile Hauptversion schützen:**  
– Haupt-Branch (z. B. `main` oder `master`) sollte **immer stabil** und funktionsfähig sein.  
– Neue Features & Bugfixes werden in **eigenen Branches** entwickelt.

⚙️ **Vorteile von Branches:**  
– Änderungen riskieren nicht den Hauptcode  
– Parallele Entwicklung mehrerer Funktionen möglich  
– Fehlerhafte Branches können **einfach gelöscht** werden

---

### **Branches in der Praxis verwenden**

🔍 **Branch anzeigen & wechseln:**  
– `git branch` → aktuelle Branch anzeigen  
– `git switch branchname` → zu bestehendem Branch wechseln  
– `git switch -c neuerBranch` → neuen Branch erstellen und wechseln

🧪 **Beispiel:**  
– Branch: `feature/login-system`  
– Änderungen vornehmen, committen und pushen:  
  `git push -u origin feature/login-system`

---

### **Merge & Zusammenarbeit**

🔄 **Branch in Hauptcode integrieren:**  
– Zu `main` wechseln: `git switch main`  
– Updates abrufen: `git pull origin main`  
– Zusammenführen: `git merge feature/login-system`  
– Änderungen hochladen: `git push`

⚠️ **Merge-Konflikte vermeiden:**  
– Vor dem Merge: immer **aktuelle Hauptversion** holen  
– Sonst: Git erlaubt keinen Merge → Konfliktgefahr

### **Commits bearbeiten, zurücknehmen & wiederherstellen**

📝 **Commit-Nachricht ändern:**  
– `git commit --amend` → letzte Nachricht im Editor bearbeiten

⏪ **Zu früherem Commit wechseln:**  
– `git checkout [Commit-ID]`  
– Zurück zum Hauptbranch: `git checkout main`

### **Commits löschen oder rückgängig machen**

🧩 **Soft Reset:**  
– `git reset --soft HEAD~1`  
→ Letzter Commit wird entfernt, Änderungen bleiben in der Staging Area

🧩 **Mixed Reset:**  
– `git reset --mixed HEAD~1`  
→ Commit wird gelöscht, Änderungen im Arbeitsverzeichnis bleiben

🧨 **Hard Reset:**  
– `git reset --hard HEAD~1`  
→ Commit + Änderungen **komplett gelöscht**  
– GitHub aktualisieren: `git push --force`  
⚠️ Gefahr: Datenverlust!

### **Sicherer Weg: `git revert` verwenden**

– `git revert [Commit-ID]`  
→ Erstellt neuen Commit, der den alten rückgängig macht  
✅ Ideal für Teamarbeit, keine Daten gehen verloren

### **Gelöschte Commits wiederherstellen**

🔁 **`git reflog` – die geheime Zeitmaschine:**  
– Zeigt alle früheren Referenzen, inkl. gelöschter Commits  
– Wiederherstellen mit: `git reset --hard [Commit-ID]`  
⚠️ Achtung: Reflog wird **nach 90 Tagen** automatisch gelöscht

### **Was ist ein Fork?**

🔄 **Fork = Projektkopie in dein eigenes GitHub-Konto**  
– Ermöglicht dir, fremde Repos zu bearbeiten  
– CLI-Befehl: `gh repo fork`  
– Danach: `cd projektname` → Projekt lokal bearbeiten

### **Feature entwickeln & Commiten**

💡 Beispiel: Bug im Taschenrechner-Projekt  
– Neues Feature/Fehlerbehebung → **neuen Branch** erstellen  
– Änderungen vornehmen  
– Commit mit `git commit -m "Fehlerbehebung"`  
– Push mit `git push` (auf deinen Fork)

### **Was ist ein Pull Request (PR)?**

📬 **PR = Anfrage zur Übernahme deiner Änderungen ins Original-Repo**  
– CLI-Befehl: `gh pr create`  
→ Titel & Beschreibung angeben

👀 Projektbesitzer sieht den PR mit `gh pr list`  
→ Details prüfen mit `gh pr view`  
→ Änderungen vergleichen: `gh pr diff`

### **Review & Merge-Prozess**

✅ **PR-Ablauf im Original-Repo:**  
– Kommentar hinzufügen: `gh pr review --comment`  
– Genehmigen: `gh pr review --approve`  
– Änderungen anfordern: `gh pr review --request-changes`  
– Merge durchführen: `gh pr merge`  
→ PR wird automatisch geschlossen

### **Warum ist das wichtig?**

🌍 **Open-Source-Leben = Zusammenarbeit**  
– Mit Fork & PR kannst du zur Entwicklung beitragen  
– Auch ohne Code: durch Issues, Feature-Vorschläge, Doku-Verbesserungen  
– CLI macht den Prozess **schnell & effizient**

### **Was ist ein GitHub Issue?**

🛠️ Issues dienen zur Fehlererfassung, Feature-Vorschlägen oder Organisation.  
– Fehler = Bug melden  
– Neue Idee = Feature vorschlagen  
– Nutzung über Web oder CLI:  
 `gh issue create`

### **Gutes Issue erstellen**

✍️ Im Issue-Titel und Beschreibung:  
– Was ist das Problem?  
– Wie wurde es entdeckt?  
– Wie könnte man es lösen?

✅ Nachverfolgbarkeit durch:  
– Labels wie `bug`, `enhancement`  
– Selbst zuweisen: `gh issue edit --assign @me`

### **Issue lösen – Schritt für Schritt**

1. Neuen Branch erstellen: `gh repo clone`, `gh pr checkout -c fix/issue-123`  
2. Fehler beheben oder Feature umsetzen  
3. Commit mit Referenz:  
 `git commit -m "Fix: #123 Eingabevalidierung hinzugefügt"`  
→ GitHub schließt Issue automatisch beim Merge

### **Pull Request (PR) erstellen**

📬 Nach dem Commit:  
– `gh pr create` → Titel + Beschreibung  
– Änderung prüfen: `gh pr diff`  
– PR verlinkt automatisch das Issue  
→ Nach Merge wird Issue geschlossen

### **Merge-Strategien im Überblick**

🔀 Drei Wege zum Merge:  
– **Merge Commit**: mehrere Commits, Verlauf bleibt erhalten  
– **Rebase**: Änderungen oben auf aktuellen Stand setzen  
– **Squash**: alle Commits zu einem einzigen zusammenfassen

🧹 Nicht mehr genutzte Branches mit:  
`gh pr delete` oder `git branch -d`

### **Vollständiger Workflow mit CLI oder Web**

✅ Projekt verbessern durch:  
– Fehler melden  
– Änderungen vorschlagen & umsetzen  
– Pull Request öffnen  
– Merge & automatische Issue-Schließung

💡 Sowohl mit CLI als auch GitHub-Weboberfläche möglich

### **Was ist ein Merge?**

🔀 Merge = Änderungen aus einem Branch in den Hauptbranch übernehmen  
– Standardkommando: `git merge branchname`  
– Wenn Hauptbranch **aktuell** ist → **Fast-Forward Merge** (kein extra Commit)  
– Wenn Änderungen im Hauptbranch vorhanden → **Merge-Commit** wird erstellt

### **Merge mit --no-ff Option**

📌 `git merge --no-ff`  
– Erzwingt immer einen Merge-Commit  
– Vorteil: Historie bleibt **sichtbar & nachvollziehbar**

### **Was ist Rebase?**

📚 Rebase = Änderungen „oben draufsetzen“, als ob sie zuletzt gemacht wurden  
– Kommando: `git rebase main`  
– Die Commits deines Branches werden **neu geschrieben**  
→ Saubere, lineare Commit-Historie

### **Unterschied: Merge vs. Rebase**

| Merge                              | Rebase                               |
|------------------------------------|---------------------------------------|
| Beibehaltung der Verzweigungen     | Lineare Historie                     |
| Echte Merge-Commits                | Commit-Historie wird neu geschrieben |
| Gut für Teams                      | Gut für Einzelentwicklung            |
| Keine Gefahr für fremde Historie   | Vorsicht: **Force Push nötig!**      |

### **Wann Rebase, wann Merge?**

✅ **Rebase sinnvoll bei:**  
– Lokaler Entwicklung  
– Eigenen Branch aktuell halten  
– Vor dem finalen Merge zur Vereinfachung der Historie  

🚫 **Rebase vermeiden bei:**  
– Gemeinsamen Branches im Team  
– Wenn andere schon basierend auf dem Branch arbeiten  

### **Best Practices im Team**

⚠️ Vorsicht bei `git push --force` nach einem Rebase  
– Nur einsetzen, wenn du **allein auf dem Branch** arbeitest  
– In Teamprojekten → lieber `merge` oder `merge --no-ff` verwenden

### **Was ist `git stash`?**

📦 `git stash` ermöglicht es dir, **zwischenzuspeichern**, woran du arbeitest – ohne zu committen.  
→ Ideal, wenn du spontan zu einem anderen Branch wechseln musst.

### **Typisches Szenario**

1. Neue Funktion (z. B. Logarithmus) begonnen  
2. Muss pausiert werden → `git stash`  
3. Andere Funktion (z. B. Modulo) entwickeln  
4. Danach ursprüngliche Änderungen mit `git stash pop` zurückholen

### **Wichtige `stash`-Befehle**

🛠️  
– Änderungen speichern: `git stash`  
– Zurückholen & entfernen: `git stash pop`  
– Zurückholen & **behalten**: `git stash apply`  
– Alle Stashes zeigen: `git stash list`  
– Einzelnen entfernen: `git stash drop`  
– Alle löschen: `git stash clear`  
– Mit Beschreibung: `git stash save "Nachricht"` (älterer Syntax)

### **Was passiert bei einem Merge-Konflikt nach `stash`?**

⚠️ Wenn zwei Branches dieselbe Datei verändern:  
– `git` zeigt dir die Konflikte im Code  
– Du entscheidest, was übernommen werden soll  
– Danach: Konflikte auflösen und committen

### **Grenzen von `stash`**

📉 Wenn du **häufig stashst**, kann es schnell unübersichtlich werden  
→ Nicht ideal für **langfristige, parallele Entwicklungen**

✅ Alternative: **`git worktree`**  
→ Damit kannst du mehrere Branches gleichzeitig bearbeiten  
→ Thema im nächsten Video!

### **Was ist `git worktree`?**

🌲 Mit `git worktree` kannst du **mehrere Arbeitsverzeichnisse gleichzeitig** für dasselbe Repository erstellen.  
→ Ideal für parallele Feature-Entwicklung – **ohne Stash oder ständiges Branch-Wechseln**.

### **Warum `worktree` statt `stash`?**

❌ Bei `git stash`:  
– Änderungen müssen immer gespeichert & zurückgeholt werden  
– Auf Dauer unübersichtlich

✅ Bei `git worktree`:  
– Jeder Branch hat **einen eigenen Ordner**  
– Saubere Trennung & paralleles Arbeiten

### **Beispiel: Zwei neue Features**

🧮 Projekt: Taschenrechner  

1. Feature 1: Faktorielle Berechnung
2. Feature 2: BMI-Rechner

→ Für jedes Feature ein eigener Worktree:

```bash
git worktree add ../bmi-feature -b bmi-feature
git worktree add ../faktor-feature -b faktor-feature


### **Entwicklung & Zusammenführen**

🚧 In jedem Worktree:  
– Neue Dateien & Funktionen entwickeln  
– `git commit` wie gewohnt  
– Nach Fertigstellung:  
  → `git merge` ins Haupt-Repository  
  → `git worktree remove` + Branch löschen

---

### **Vorteile von `git worktree`**

✅ Unabhängige Entwicklungsumgebungen  
✅ Kein versehentliches Überschreiben  
✅ Klar strukturierte Arbeitsweise  
✅ Ideal für mehrere Aufgaben gleichzeitig


### **Fazit – Git Worktree**

Mit `git worktree` kannst du mehrere Features gleichzeitig entwickeln, ohne die Übersicht zu verlieren.  
→ Besser als `stash` für mittlere und große Projekte  
→ Einfaches Zusammenführen am Ende mit `merge`


### **Was ist ein Merge-Konflikt?**

⚠️ Merge-Konflikte entstehen, wenn **zwei Branches dieselbe Datei und dieselbe Zeile** verändert haben.  
→ Git kann nicht automatisch entscheiden, welche Änderung bleiben soll.


### **1. Konflikte manuell lösen**

🛠️ Git markiert die Konfliktstellen so:

```

### **Entwicklung & Zusammenführen**

<<<<<<< HEAD
(dein Code)
=======
(Code vom anderen Branch)
>>>>>>> branch-name
```
✅ Lösung:  
– Behalte, was du brauchst  
– Entferne die Konflikt-Markierungen  
– Speichern und `git add` ausführen

---

### **2. Mit `git mergetool` & `vimdiff` lösen**

📚 Nutze `git mergetool`, um visuell zu vergleichen:

– Links: **lokale Änderungen**  
– Rechts: **Remote-Branch**  
– Mitte: **gemeinsame Basis**

➡️ Kombination mit Tasten (`yy`, `p`) möglich  
➡️ Abschließen mit: `:wqa`

---

### **3. Konflikte mit VS Code lösen**

🖥️ Alternativ:  
```bash
code .
```

– VS Code erkennt Konflikte automatisch  
– Wähle:  
 ✅ „Current Change“  
 ✅ „Incoming Change“  
 ✅ oder „Beide übernehmen“  
– Speichern, fertig!

## **Merge oder Rebase?**

| Merge                             | Rebase                             |
|----------------------------------|------------------------------------|
| Beibehaltung der Historie        | Aufgeräumte, lineare Historie      |
| Besser rückverfolgbar            | Weniger Commits sichtbar           |
| Konfliktlösung klar dokumentiert | Vorsicht bei Teamarbeit (Force Push nötig) |

💡 **Tipp:**  
→ Bei Teams: Merge bevorzugt  
→ Bei Solo-Projekten: Rebase möglich

### **Problem: Große Dateien in GitHub**

📦 GitHub erlaubt **max. 100 MB pro Datei**  
– Größere Dateien verursachen **Fehler beim Push**  
– Auch kleinere Dateien können das Repo **unnötig aufblähen**  
→ Lange Ladezeiten & Speicherprobleme

### **Lösung: Git LFS (Large File Storage)**

🧠 Git LFS speichert große Dateien **außerhalb des normalen Repos**  
– Im Git-Repo liegt nur ein **Verweis (Pointer)**  
– Die Datei selbst liegt auf einem separaten **LFS-Server**

### **Git LFS einrichten & verwenden**

🔧 Schritte:  

1. Git LFS installieren & initialisieren:  
 `git lfs install`  
2. Datei zum Tracking hinzufügen:  
 `git lfs track "*.zip"`  
3. Commit & Push wie gewohnt  
→ Datei wird an LFS-Server übertragen, nicht direkt in GitHub

📁 Nachverfolgt in `.gitattributes`-Datei

### **Projekt klonen mit LFS-Dateien**

📥 Nach dem Klonen eines LFS-Repos:  
– Nur Verweise werden heruntergeladen  
– Um Dateien wirklich zu bekommen:  
 `git lfs pull`

### **Vorteile von Git LFS**

✅ Besseres Speicher-Management  
✅ Schnellere Klon-Vorgänge  
✅ Saubere Repos trotz großer Dateien (z. B. Videos, Binärdateien)

---

### **Was kommt als Nächstes?**

🔐 Wenn große Dateien **versehentlich** direkt gepusht wurden oder sensible Infos (z. B. API-Schlüssel) im Verlauf sind, hilft:  
→ `git filter-repo` (im nächsten Video)

### **Problem: Sensible Daten & große Dateien in der Git-Historie**

🚫 Git speichert **jede Version** einer Datei – auch gelöschte!  
→ API-Schlüssel oder große Dateien bleiben im **Commit-Verlauf** erhalten  
→ Sicherheitsrisiko & Speicherproblem

### **Lösung: `git filter-repo`**

🧹 `git filter-repo` schreibt die gesamte Git-Historie neu:  
– Entfernt gezielte Dateien rückwirkend aus allen Commits  
– Ersetzt sensible Inhalte (z. B. API-Keys)  
– Leichtgewichtig & schneller als `git filter-branch`

### **Große Dateien aus Git entfernen**

📁 Beispiel: 500 MB-Datei wurde irrtümlich gepusht  
👉 Schritte:  

1. Datei sichern  
2. `git filter-repo --invert-paths --path dateiname`  
3. Remote-Verbindung neu setzen  
4. `git push --force`  
→ Datei ist aus allen Commits **gelöscht**

### **API-Schlüssel ersetzen**

🔐 Beispiel: Variable `API_KEY="12345"`  
👉 Ziel: `"12345"` in allen Commits durch `"REDACTED"` ersetzen

📄 Vorgehen:  

1. Ersetzdatei (`replace.txt`) anlegen  
2. `git filter-repo --replace-text replace.txt`  
3. Force Push ausführen  
→ Schlüssel ist überall ersetzt

### **Wichtige Hinweise**

⚠️ Nach `filter-repo`:  
– Remote (`origin`) muss **neu hinzugefügt** werden  
– Immer `git push --force` notwendig  
– Alte Klone sind **nicht mehr kompatibel**

### **Fazit**

✅ Mit `git filter-repo` kannst du:  
– Große Dateien aus der Historie löschen  
– Sensible Daten wie API-Schlüssel sicher entfernen  
– Repositories langfristig sauber und sicher halten

### **Was ist ein Git Submodul?**

🔗 Ein **Submodul** ist ein externes Git-Repository, das in dein Hauptprojekt eingebunden wird.  
→ Ideal für **wiederverwendbare Komponenten** (z. B. Bezahlsysteme, Parser, Bibliotheken)

### **Warum Submodule verwenden?**

✅ Vorteile:  
– Unabhängige Entwicklung & Versionsverwaltung  
– Einfaches Wiederverwenden in mehreren Projekten  
– Sicherheitskritische Komponenten separat verwaltbar  
– Eigenes Team kann Submodul unabhängig betreuen

### **Beispiel: Mathematischer Parser als Submodul**

📦 Statt Code direkt zu integrieren:  

```bash
git submodule add https://github.com/beispiel/math-parser libs/math-parser
```

→ Wird **nicht kopiert**, sondern als **eigene Git-Quelle** verlinkt  
→ In VS Code oder im Terminal jederzeit sichtbar & kontrollierbar

### **Submodul updaten & verwalten**

📥 Nach dem Klonen eines Repos mit Submodul:

```bash
git submodule update --init --recursive
```

🔁 Änderungen im Submodul übernehmen:  
– Ins Hauptprojekt integrieren: `git commit`  
– Alte Version nutzen? → Einfach zu bestimmtem Commit zurückkehren

### **Submodul wieder entfernen**

🧹 Schritte:

1. Submodul-Verbindung lösen  
2. Dateien aus dem Projekt entfernen  
3. Einträge aus `.gitmodules` und `.git/config` bereinigen  
→ Submodul ist vollständig entfernt

✅ Submodule sind perfekt für:
– Wiederverwendbare, getrennt verwaltete Projektteile  
– Gemeinsame Nutzung über mehrere Projekte hinweg  
– Klare Trennung zwischen Hauptprojekt und Modul

⚠️ Wenn Module **stark miteinander gekoppelt** sind → besser `subtree` (nächstes Thema)

### **Was ist ein Git Subtree?**

🌳 **`git subtree`** integriert ein externes Repository **vollständig in dein Projekt** – der Code wird physisch hinzugefügt.  
→ Ideal, wenn der Code eng mit dem Projekt gekoppelt ist (z. B. UI-Komponenten für mobile Apps)

### **Submodule vs. Subtree**

| Submodule                              | Subtree                              |
|----------------------------------------|---------------------------------------|
| Verlinkt externes Repo (Referenz)      | Fügt Code direkt ein (Kopie)          |
| Extra `git clone` nötig                | Sofort nutzbar                        |
| Unabhängige Entwicklung                | Komplett integriert                   |
| Komplexer beim Entfernen / Updaten     | Einfache Verwaltung im Haupt-Repo     |

### **Subtree hinzufügen – Beispiel**

📦 Beispiel: Parser-Modul `math-parser` einbinden  

```bash
git subtree add --prefix=libs/math-parser \
  https://github.com/beispiel/math-parser.git master --squash
```

– `--prefix`: Zielordner im Projekt  
– `--squash`: Alle Commits als ein einziger zusammengefasst

### **Subtree verwenden & verwalten**

🔁 **Update eines Subtrees:**  

```bash
git subtree pull --prefix=libs/math-parser \
  https://github.com/beispiel/math-parser.git master --squash
```

🧹 **Entfernen:**  
– Einfach Ordner löschen  
– Änderungen committen & pushen → Subtree entfernt

### **Vorteile von Git Subtree**

✅ Komplett integrierter Code  
✅ Keine externen Abhängigkeiten beim Klonen  
✅ Einfach zu nutzen für tightly coupled Module  
✅ Perfekt für Komponenten, die mit dem Hauptprojekt wachsen sollen

### **Was ist `git bundle`?**

📦 Mit **Git Bundle** kannst du ein komplettes Git-Repository (inkl. Branches & Commits) in eine **einzige Datei** verpacken.  
→ Ideal für **Offline-Backups**, **sichere Archivierung** oder **Weitergabe ohne Internet**.

### **Warum `git bundle` nutzen?**

✅ Vorteile:
– Kein Remote-Server (z. B. GitHub) nötig  
– Funktioniert **ohne Internet**  
– Perfekt für große Repos oder sensible Projekte  
– Einfach zu transportieren (z. B. USB-Stick, Cloud, E-Mail)

### **Repo als Bundle speichern**

💾 Befehl zum Erstellen:

```bash
git bundle create projekt.bundle --all
```

→ Erstellt eine `.bundle`-Datei mit **allen Branches & Commits**

📁 Alternativ: Nur einen Branch speichern:

```bash
git bundle create projekt.bundle master


### **Bundle wiederherstellen**

📥 Neues Projekt aus Bundle klonen:
```bash
git clone projekt.bundle projekt-ordner
```

→ Funktioniert wie ein normales Repository  
→ Commit-Historie & Branch-Struktur bleiben erhalten

### **Einsatzmöglichkeiten von `git bundle`**

🌍 Typische Szenarien:
– Projekte **offline weitergeben**  
– Sicherung auf **externe Medien**  
– Migration zwischen **geschützten Netzwerken**  
– Archivierung von Repos für spätere Nutzung

✅ Mit `git bundle` kannst du dein Repository jederzeit **kompakt sichern oder weitergeben** – ganz ohne GitHub oder Internet.  
→ Im nächsten Schritt: **nur einen einzelnen Commit** weitergeben mit `git patch`.

### **Was ist ein Git Patch?**

🧩 Ein **Patch** speichert Änderungen aus einem oder mehreren Commits als **Textdatei** im Diff-Format.  
→ Ideal, um gezielte Änderungen in andere Projekte oder Branches zu übertragen – **ohne komplettes Repo**.

### **Patch-Datei erstellen**

📦 Einzelnen Commit als Patch speichern:  

```bash
git format-patch -1 <commit-hash>
```

📦 Mehrere Commits (z. B. die letzten 3):  

```bash
git format-patch -3
```

📦 Commit-Bereich als Patch:  

```bash
git format-patch <start-hash>..<end-hash>
```

→ Ergebnis: `.patch`-Dateien mit den jeweiligen Änderungen

### **Patch anwenden**

📥 Änderungen in ein anderes Projekt übernehmen:

1. Patch-Datei ins Zielprojekt kopieren  
2. Patch **anwenden (ohne Commit)**:  
 ```bash
git apply datei.patch```

3. Patch **mit Commit übernehmen**:  
 ```bash
git am datei.patch```

→ Änderung erscheint dann **im Commit-Verlauf**

---

### **Wann Git Patch verwenden?**

✅ Typische Anwendungsfälle:

– Einzelne Commits projektübergreifend teilen  
– Änderungen über E-Mail oder Datei weitergeben  
– Offline oder ohne Git-Remote arbeiten  
– Saubere Code-Reviews vorbereiten

📄 Mit `git patch` kannst du gezielte Änderungen leicht exportieren und importieren – unabhängig vom gesamten Repository.  
→ Im nächsten Video: **GitHub Pages – eigene Website direkt aus dem Repo hosten**

### **Was ist GitHub Actions?**

🤖 **GitHub Actions** ist ein CI/CD-System (Continuous Integration / Continuous Deployment),  
das automatisch Aufgaben nach jedem Push oder Pull Request ausführt.

### **Warum GitHub Actions verwenden?**

✅ Vorteile:
– Automatisches Testen & Linting  
– Benachrichtigungen bei Fehlern  
– Builds erstellen, Deployments durchführen  
– Aufgaben zu bestimmten Zeiten planen  
→ Spart Zeit und vermeidet manuelle Fehler

### **Beispiel: Super-Linter einrichten**

🧰 Ziel: Codequalität prüfen

📁 Struktur:

```git
.github/
└── workflows/
    └── linter.yml
```

📄 Inhalt (`linter.yml`):
– Trigger: `push`, `pull_request`  
– Schritte:  
 1. Repository auschecken  
 2. Super-Linter starten  
 3. GitHub Token übergeben

### **Was macht der Linter?**

🔍 Bei jedem Push prüft Super-Linter:
– Syntaxfehler  
– Formatierung  
– Dokumentation

❌ Bei Fehlern → Workflow schlägt fehl  
✅ Bei korrektem Code → Workflow erfolgreich

---

### **Fehler erkennen & beheben**

👨‍💻 GitHub zeigt:
– Welche Datei betroffen ist  
– In welcher Zeile der Fehler steckt  
– Warum der Fehler aufgetreten ist

🛠️ Fehler korrigieren → Push erneut → Workflow läuft erneut durch

🚀 Mit GitHub Actions kannst du:
– Testen, Linting, Build & Deployment automatisieren  
– Projekte stabiler & professioneller machen  
– Manuelle Arbeit reduzieren

📘 Tipp: Weitere fertige Actions findest du im [GitHub Marketplace](https://github.com/marketplace)

### **Was sind Git Hooks?**

🧠 **Git Hooks** sind Skripte, die bei bestimmten Git-Ereignissen automatisch ausgeführt werden – z. B. vor einem Commit, nach einem Push oder bei einem Merge.

### **Warum Git Hooks verwenden?**

✅ Vorteile:
– Commit-Nachrichten erzwingen  
– Codequalität vor Push sicherstellen  
– Tests vor Merge automatisch ausführen  
– E-Mail-/Slack-Benachrichtigungen senden

→ Automatisierte **Regelkontrolle im Team**

### **Beispiele für wichtige Hooks**

| Hook             | Zweck                               |
|------------------|--------------------------------------|
| `pre-commit`     | Tests ausführen, Linting prüfen       |
| `commit-msg`     | Commit-Message-Format erzwingen       |
| `pre-push`       | Codequalität prüfen vor Push          |
| `post-commit`    | Slack-Nachricht oder Log schreiben    |

📂 Speicherort: `.git/hooks/`  
📎 Standardmäßig `.sample` → muss umbenannt & aktiviert werden

### **Commit-Message-Format prüfen**

🛑 Nur Commits mit folgendem Format erlauben:

```commit
feat: Neue Funktion
fix: Fehlerbehebung
```

📜 Umsetzung:

1. `commit-msg` Hook aktivieren  
2. Format im Skript prüfen  
3. Ungültige Messages blockieren

---

### **Automatisierung im Team**

💡 Mit Git Hooks kannst du:

– Entwicklungsstandards durchsetzen  
– Fehlerquellen minimieren  
– Manuelle Reviews reduzieren  
– Einheitlichen Workflow sicherstellen

🔒 Git Hooks helfen dir, **Team-Regeln durchzusetzen**, **Fehler frühzeitig zu erkennen** und **deine Git-Prozesse zu automatisieren**.  
→ Im nächsten Video: GitHub API nutzen, um Aktionen direkt per Code auszuführen.

### **Was ist die GitHub API?**

🔧 Mit der **GitHub API** kannst du fast alle Funktionen von GitHub per **Code oder Terminal** automatisieren:  
– Repos verwalten  
– Issues & Pull Requests erstellen  
– Actions steuern  
– Sicherheit & Benutzer verwalten

---

### **Voraussetzung: Token erstellen**

🔐 Zuerst wird ein **Personal Access Token** benötigt:

1. GitHub → *Settings* → *Developer settings*  
2. „Fine-grained token“ generieren  
3. Rechte (z. B. nur Lesen/Schreiben für Repos) gezielt vergeben  
4. Token sicher speichern

---

### **API-Befehle ausführen (z. B. mit `curl`)**

📌 Beispiel: Eigenes Profil abfragen

```bash
curl -H "Authorization: token $TOKEN" https://api.github.com/user
```

📌 Beispiel: Neues Repository erstellen

```bash
curl -X POST -H "Authorization: token $TOKEN" \
  -d '{"name":"mein-repo"}' \
  https://api.github.com/user/repos
```

📌 Beispiel: Neues Issue mit Label

```bash
curl -X POST -H "Authorization: token $TOKEN" \
  -d '{"title":"Bug melden","labels":["bug"]}' \
  https://api.github.com/repos/<user>/<repo>/issues
```

---

### **Was ist mit der API möglich?**

✅ Mögliche Aktionen:
– Repos erstellen, löschen  
– Issues, PRs, Kommentare verwalten  
– Dateien hochladen  
– Actions starten oder überwachen  
– Profil & Organisationen bearbeiten

📚 Die offizielle GitHub API-Dokumentation hilft mit:
– Beispielen  
– Endpunkten  
– Antwortformaten

🧠 Die GitHub API ist ein mächtiges Tool für Automatisierung, Integration und Verwaltung – direkt über Code oder Terminal.  
→ Im nächsten Video: **GitHub Copilot** als smarter Assistent für API & Git-Kommandos!

### **Was ist Git eigentlich?**

Git = Ein verteiltes Versionskontrollsystem  
→ GitHub = Nur eine von vielen Plattformen, um Git zu nutzen!

---

### **GitHub**

- Größte Entwickler-Community der Welt  
- Ideal für Open-Source-Projekte  
- Features:
  - **Actions** (CI/CD)
  - **Copilot** (KI-Unterstützung)
  - 5 GB Speicher pro Repo (kostenlos)
- Wird u. a. für **Linux**, **React**, **VS Code** genutzt

---

### **GitLab**

- Self-Hosted möglich  
- Sehr stark bei **CI/CD & Automatisierung**  
- 10 GB Speicher pro Repo  
- Ideal für große Unternehmen  
- Fokus auf **Sicherheit & Kontrolle**

---

### **Bitbucket**

- Optimal für **kleine Teams & Start-ups**  
- Perfekte Integration mit **Jira & Trello**  
- 2 GB Speicher pro Repo (kostenlos)  
- Fokus auf Projektmanagement & Agilität

---

### **Azure DevOps**

- Entwickelt von **Microsoft**  
- Perfekt für .NET & Microsoft-Technologien  
- Starke Sicherheit & DevOps-Integration  
- 10 GB Speicher pro Repo  
- Ideal für **große Firmen**

---

### **AWS CodeCommit**

- Nahtloses Zusammenspiel mit AWS-Diensten  
- 1 GB Speicher pro Repo  
- Für Projekte im **AWS-Ökosystem** sehr geeignet  
- Skalierbar & cloudbasiert

---

### **Vergleich – Wann was nutzen?**

| Plattform       | Ideal für                                          |
|----------------|----------------------------------------------------|
| **GitHub**      | Open Source, große Community, Kollaboration       |
| **GitLab**      | Eigenes Hosting, volle Kontrolle, Sicherheit      |
| **Bitbucket**   | Kleine Teams, Atlassian-Tools                     |
| **Azure DevOps**| Microsoft-Umgebungen, große Projekte              |
| **AWS**         | Cloud-native Entwicklung im AWS-Ökosystem         |

---

Alle Plattformen basieren auf **Git**, unterscheiden sich aber in Integration, Speicher und Zielgruppen.  
🔍 Nächste Folge: **Git Workflows** – wie du dein Team effizient organisierst.

### **Git Workflows – Übersicht**

Es gibt **nicht nur einen** Weg, Git zu nutzen. Unterschiedliche Teams und Projekte erfordern unterschiedliche **Arbeitsabläufe**.

---

### **1. GitHub Flow**

- Für einfache & häufige Deployments
- Schritte:
  - Branch erstellen
  - Feature entwickeln
  - Pull Request (PR) erstellen
  - Testen
  - Merge in `main`
- ✅ Schnell & schlank  
- ⚠️ Kann bei vielen Branches unübersichtlich werden

---

### **2. Git Flow**

- Für **größere, strukturierte Projekte**
- Branch-Typen:
  - `main` → stabile Releases
  - `develop` → aktives Development
  - `feature/*` → neue Features
  - `release/*` → Vorbereitung auf Release
  - `hotfix/*` → schnelle Fehlerbehebung
- ✅ Sehr organisiert  
- ⚠️ Etwas komplex

---

### **3. Fork Workflow**

- Ideal für **Open Source**
- Schritte:
  - Projekt forken
  - Eigene Änderungen lokal umsetzen
  - PR stellen
- ✅ Beiträge von außen einfach verwalten

---

### **4. Trunk Based Development**

- Entwicklung direkt auf `main`
- Kleine, häufige Commits
- Ideal mit CI/CD
- ✅ Schnell, modern  
- ⚠️ Erfordert stabile Tests & Pipelines

---

### **5. GitLab Flow**

- Mischung aus GitHub & Git Flow
- Fokus: Umgebung (develop, staging, production)
- ✅ Klarer Deployment-Prozess  
- ⚠️ Weniger geeignet ohne CI/CD

---

### **6. Release Flow (Microsoft Style)**

- `main` bleibt stabil  
- Releases über `release/*`-Branches
- ✅ Für große Unternehmen & feste Versionierung

---

### **Vergleich & Empfehlung**

| Workflow           | Ideal für                                 |
|--------------------|--------------------------------------------|
| GitHub Flow        | Kleine Projekte, schnelle PRs              |
| Git Flow           | Strukturierte Teams, mittelgroße Projekte  |
| Fork Workflow      | Open Source & Community Contributions      |
| Trunk Based Dev    | Moderne Teams mit CI/CD                    |
| GitLab Flow        | Teams mit klaren Umgebungen                |
| Release Flow       | Große Firmen, stabile Releases             |

---

Wähle den Workflow, der zu deinem **Team**, deinem **Projektziel** und deinen **Tools** passt.  
🔜 Nächste Folge: **Projektplanung mit GitHub Projects**.

### **GitHub Projects – Planung & Nachverfolgung**

Eine gute Projektplanung ist entscheidend für den Erfolg.  
GitHub bietet mit **Projects** ein mächtiges Tool zur **organisierten Verwaltung von Aufgaben**.

---

### **1. Projekt anlegen**

- Unter dem Reiter **Projects** → neues Projekt erstellen
- Vorlagen: **Roadmap**, **Tabelle** oder **Board**  
- Aufgaben (Issues) können:
  - Manuell erstellt
  - Oder aus Repositories importiert werden

---

### **2. Aufgaben verwalten**

- Aufgaben (Issues) enthalten:
  - Verantwortliche Person
  - Typ (Feature, Bug, etc.)
  - Status (To Do, In Progress, Done)
  - Start- & Enddatum
  - Review-Datum

---

### **3. Tabellenansicht**

- Zeigt:  
  - Wer macht was  
  - Deadlines & Fortschritt  
- Hilfreich für Teams

---

### **4 Kanban Board**

- Aufgabenstatus im Überblick:
  - **To Do**, **In Progress**, **Done**
  - Eigene Spalten möglich (z. B. „Test“)
- Drag & Drop  
- Automatisches Verschieben nach Abschluss

---

### **5. Vorteile**

- Aufgabenplanung & Fortschrittskontrolle an einem Ort
- Automatische Synchronisierung mit Repositories
- Ideal für Teamarbeit & transparente Prozesse
- Bestehende Vorlagen aus Open-Source-Projekten wiederverwendbar

---

Mit **GitHub Projects** wird Projektarbeit:

- **strukturierter**
- **nachvollziehbarer**
- **professioneller**

### **Gelernte Inhalte festigen – Git & GitHub effektiv anwenden**

Nach 34 Kapiteln:  
✅ Commit  
✅ Branching  
✅ Merge  
✅ Pull Requests  
✅ Open Source Beiträge  
... hast du alles von Grund auf gelernt!

---

### **Wie bleibt das alles im Kopf?**

> **👉 Nur durch Praxis!**

- Starte ein Projekt mit **GitHub Projects**
- Erstelle **Branches**, mache **Commits**, löse bewusst **Merge-Konflikte**
- Teste **Undo-Funktionen** (z. B. `reset`, `restore`)
- Wiederhole Vorgänge regelmäßig!

---

### **Simuliere echte Beiträge**

- Erstelle ein **zweites GitHub-Konto**
- Eröffne **Pull Requests** aus diesem Konto
- Überprüfe und merge selbst → **Open-Source-Szenarien nachstellen**

---

### **Wiederholung macht Meister**

- Wiederhole typische Workflows in **verschiedenen Projekten**
- Lerne durch eigene Fehler
- Git wird mit der Zeit zur **zweiten Natur**

---

### **Zusammenführung**

- Git & GitHub sind keine Theorie – sie leben durch Übung
- Mit jeder Zeile Code wirst du sicherer
- Bald kannst du sagen:  
  **„Ich beherrsche Git & GitHub.“**
