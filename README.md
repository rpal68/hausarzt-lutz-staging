# hausarzt-lutz.de – Testumgebung

Statische Website der Hausarztpraxis René Lutz, Schweinfurt. Dieses Repository dient **ausschließlich zum Testen via GitHub Pages** vor dem Umzug auf das eigentliche Strato-Hosting.

## Live-Vorschau

Nach Aktivierung von GitHub Pages (Settings → Pages → Branch `main`, Root) erreichbar unter:

```
https://<benutzername>.github.io/<repo-name>/
```

## Struktur

```
index.html                        Startseite (startseite_hausarzt-lutz.html umbenannt)
service.html                      Termine, Rezepte, Überweisungen, Hausbesuche, FAQ
leistungen.html                   Leistungsübersicht
praxis-team.html                  Praxis & Team
news.html                         Aktuelles / Urlaubszeiten
impressum.html
datenschutz.html

urlaub.js                         Zentrale Urlaubs-/Feiertagslogik (Infobar)
aufnahmebogen.pdf                 Patienten-Aufnahmebogen zum Download

favicon.svg / favicon-32.png / favicon-16.png / apple-touch-icon.png
og-image.png                      Vorschaubild für Social Media / Messenger-Links
```

**Hinweis Dateinamen:** Alle internen Links (`href="index.html"`, `href="service.html"` usw.) erwarten die kurzen Dateinamen ohne `hausarzt-lutz`-Suffix. Beim Hochladen bitte entsprechend umbenennen:

| Datei im Ausgabeordner | Umbenennen zu |
|---|---|
| `startseite_hausarzt-lutz.html` | `index.html` |
| `service_hausarzt-lutz.html` | `service.html` |
| `leistungen_hausarzt-lutz.html` | `leistungen.html` |
| `praxis-team_hausarzt-lutz.html` | `praxis-team.html` |
| `news_hausarzt-lutz.html` | `news.html` |
| `impressum_hausarzt-lutz.html` | `impressum.html` |
| `datenschutz_hausarzt-lutz.html` | `datenschutz.html` |

Alle übrigen Dateien (Assets, `urlaub.js`, PDF) unverändert übernehmen.

## Bekannte Abweichungen im Testbetrieb (kein Fehler)

- **Canonical-Links und OpenGraph-Tags** zeigen fest auf `https://hausarzt-lutz.de/…`, nicht auf die GitHub-Pages-Adresse. Social-Media-Vorschauen (z. B. WhatsApp-Linkvorschau) zeigen daher testweise auf die falsche Domain – auf Strato ist das korrekt.
- **Rezept-Button, DOConline-Integration und `tel:`-Links** funktionieren unabhängig vom Hosting und lassen sich hier normal testen.
- **Kein Cookie-Banner, kein Tracking** – die Seite ist bewusst als cookie-freie statische Seite konzipiert; das gilt auch auf GitHub Pages.

## Nicht für den Live-Betrieb bestimmt

Dieses Repository ist eine Testumgebung. Der tatsächliche Go-live erfolgt über Strato-Hosting unter `hausarzt-lutz.de` mit AV-Vertrag nach Art. 28 DSGVO und lokal eingebetteten Schriftarten.

---

**Status:** Subseiten in Fertigstellung (Stand Juli 2026) · Go-live geplant für Anfang/Mitte August 2026
