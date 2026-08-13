# Krankengymnastik Wim Menzo — Website

Onepager für die Physiotherapie-Praxis **Krankengymnastik Wim Menzo**, Hauptstraße 18, 49835 Wietmarschen-Lohne.

## Aufbau

Die komplette Seite steckt in **einer einzigen Datei**: `index.html`. CSS und JavaScript sind inline, das Logo als data-URI eingebettet.

* keine Frameworks, keine Build-Schritte, keine Abhängigkeiten
* **null externe Requests** — keine Font-CDNs, kein Analytics, keine Tracker
* ~96 KB, Ladezeit unter einer Sekunde

Zum Ansehen genügt ein Doppelklick auf `index.html`. Zum Veröffentlichen genügt es, die Datei auf einen Webspace zu legen.

| Datei | Zweck |
|---|---|
| `index.html` | die vollständige Website |
| `KGLogo.png` | Original-Logo der Praxis (unverändert; in der Seite steckt eine freigestellte, verkleinerte Fassung) |

## Datenschutz

Die Seite setzt **keine** Cookies und lädt nichts von fremden Servern. Einwilligungspflichtig ist allein die optionale Google-Maps-Karte im Abschnitt „Kontakt & Anfahrt“:

* vor der Zustimmung wird nichts von Google geladen (Prior Blocking)
* gleichwertige Schaltflächen „Alle akzeptieren“ und „Nur notwendige“
* Widerruf jederzeit über „Cookie-Einstellungen“ im Fußbereich
* gespeichert wird ausschließlich die Entscheidung selbst, lokal im Browser, für 12 Monate

## Barrierefreiheit

Ausgelegt auf WCAG 2.1 AA: semantisches HTML, genau eine `h1`, Tastaturbedienung mit sichtbarem Fokus, Touch-Targets ab 44 px, Kontraste durchgehend über 4,5:1 (schlechtester Wert 5,88:1). `prefers-reduced-motion` schaltet sämtliche Animationen ab.

## Suchmaschinen

Die Seite ist auf lokale Suchen nach Physiotherapie in Wietmarschen-Lohne ausgerichtet: Titel und Beschreibung mit Ortsbezug, strukturierte Daten als verknüpfter Graph (`LocalBusiness`/`Physiotherapy` mit geprüften Koordinaten, Öffnungszeiten, Bewertung und allen 15 Leistungen), eine FAQ-Sektion sowie `robots.txt` und `sitemap.xml`.

**Vor der Live-Schaltung** sind vier Stellen mit der echten Domain zu füllen — die Suche nach `DOMAIN-EINTRAGEN` findet alle. Bis dahin bleiben `canonical` und `og:url` bewusst leer: eine Angabe, die auf eine nicht existierende Domain zeigt, schadet mehr, als sie nützt.

Die vollständige Anleitung samt Handlungsliste für das Google-Unternehmensprofil steht in **[GO-LIVE.md](GO-LIVE.md)**. Der Hinweis dort ist wichtig: Die Website ist nur einer von mehreren Faktoren — die Signale aus dem Unternehmensprofil wiegen bei lokalen Suchen deutlich schwerer.

## Offene Punkte

Diese Inhalte liefert der Praxisinhaber; im Quelltext sind sie als `TODO` markiert:

- [ ] Impressumstext (Angaben nach § 5 DDG, Berufsbezeichnung, zuständige Kammer)
- [ ] Datenschutzerklärung (muss die Google-Maps-Einbindung beschreiben)
- [ ] echtes Praxis-/Teamfoto statt des gekennzeichneten Platzhalters

Hinweis: Der Öffnungszeiten-Status („Jetzt geöffnet“) rechnet mit den regulären Zeiten und berücksichtigt keine Feiertage — darauf weist ein Text unter der Tabelle hin.
