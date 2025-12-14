# Projekt-Dokumentation – Workflows & Betrieb

Diese Datei dokumentiert die grundlegenden Arbeitsabläufe dieses Projekts.  
Sie dient als langfristige Referenz und als Nachschlagewerk für die Pflege der Lore-Website.

Behandelte Themen:
- Markdown (Inhalte)
- Quartz (Website-Generierung)
- Git & GitHub (Versionierung und Deployment)
- Betrieb und Verfügbarkeit der Website

---

## Markdown – Inhalte pflegen

Alle Inhalte werden in Markdown (`.md`) geschrieben.  
Jede Datei entspricht einer eigenständigen Lore-Seite.

Die Strukturierung erfolgt über Ordner und interne Verlinkung.

Interne Verlinkung im Wiki-Stil erfolgt mit doppelten eckigen Klammern:

[[zielseite]]  
[[ordner/zielseite]]  
[[zielseite|Anzeigetext]]

Links dürfen auch auf noch nicht existierende Seiten zeigen.  
Quartz erkennt diese automatisch und integriert sie in das Seiten-Netz (Graph).

Textformatierung erfolgt mit Standard-Markdown:
- Überschriften strukturieren Inhalte
- Absätze für Fließtext
- Listen für Aufzählungen

Bilder und Karten werden lokal im Projekt gespeichert und per Markdown eingebunden:

![Beschreibung](pfad/zum/bild.png)

---

## Quartz – Website-Generierung

Quartz erzeugt aus allen Markdown-Dateien eine statische Website.

Quartz übernimmt automatisch:
- Navigation
- Volltextsuche
- Graph-/Netz-Ansicht
- Backlinks zwischen Seiten

Quartz ist kein Editor und keine Datenbank.  
Alle Inhalte bleiben einfache Textdateien.

### Lokal testen

Die Website kann lokal gestartet werden mit:

npx quartz build --serve

Die Seite ist anschließend unter http://localhost:8080 erreichbar.  
Beenden mit Strg + C.

### Online-Version

Die Online-Website wird nicht manuell gebaut.  
Build und Veröffentlichung erfolgen automatisch über GitHub Actions.

---

## Git & GitHub – Versionskontrolle

Das Projekt wird vollständig über Git versioniert.

Standard-Workflow für Änderungen:

git add .  
git commit -m "Kurzbeschreibung der Änderung"  
git push  

Jeder Push speichert Änderungen dauerhaft und nachvollziehbar im Repository.

Aktiver Hauptbranch des Projekts ist `v4`.

GitHub Pages wird ausschließlich über GitHub Actions betrieben.

---

## Wichtige Regeln

Der Ordner `public/` darf nicht manuell bearbeitet werden.  
Er wird ausschließlich automatisch durch Quartz erzeugt.

Inhalte werden nur im `content/`-Bereich geändert.

---

## GitHub Actions – Deployment

Jeder Push auf den Hauptbranch löst automatisch einen Deployment-Workflow aus.

Ablauf:
1. Einrichtung der Node-Umgebung
2. Installation der Abhängigkeiten
3. Quartz-Build
4. Veröffentlichung auf GitHub Pages

Der Status kann jederzeit überprüft werden unter:

GitHub → Repository → Actions

Ein grüner Workflow bedeutet:
- Website ist aktuell
- Website ist online

---

## Fehlerbehebung (Kurzreferenz)

Wenn die Website alte Inhalte zeigt:
- Prüfen, ob der letzte Workflow erfolgreich war
- Browser-Cache ggf. leeren

Wenn die Website nicht erreichbar ist:
- Settings → Pages prüfen
- GitHub Actions auf Fehler kontrollieren

Wenn der Build fehlschlägt:
- Actions-Log öffnen
- Häufige Ursachen:
  - falsche Node-Version
  - ungültige Markdown-Datei
  - fehlerhafte Quartz-Konfiguration

---

## Betrieb & Verfügbarkeit der Website

Die Website bleibt dauerhaft online, solange:
- das GitHub-Repository existiert
- GitHub Pages aktiviert bleibt
- der GitHub-Account nicht gelöscht wird

Es gibt:
- kein Ablaufdatum
- kein Inaktivitäts-Limit
- keine laufenden Kosten

Die Website bleibt auch dann online, wenn über längere Zeit keine Änderungen vorgenommen werden.

Alle Inhalte sind unabhängig vom lokalen Rechner gespeichert und können jederzeit:
- heruntergeladen
- gesichert
- auf ein anderes Hosting migriert werden

---

## Merksatz

Inhalte ändern → commit & push  
Website bauen und veröffentlichen → automatisch
