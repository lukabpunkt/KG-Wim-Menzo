# Vor und nach der Live-Schaltung

Diese Liste ist nach Wirkung sortiert. Punkt 1 bringt mehr als alles andere zusammen.

**Vorweg, damit die Erwartung stimmt:** Eine Website allein bringt keine Spitzenposition bei Google. Bei lokalen Suchen stammen rund 32 % der Rankingsignale aus dem Google-Unternehmensprofil, 19 % aus der Website, 16 % aus Rezensionen. Die Website ist inzwischen technisch sauber und inhaltlich vollständig — der Rest liegt beim Praxisinhaber.

---

## 1. Google-Unternehmensprofil pflegen (größter Hebel)

Ein Profil existiert bereits — die 4,5 Sterne aus 12 Rezensionen stammen daher. Anmelden unter [business.google.com](https://business.google.com), Inhaberschaft bestätigen lassen, falls noch nicht geschehen.

- [ ] **Hauptkategorie „Physiotherapeut"** setzen. Die Kategorie entscheidet mit darüber, bei welchen Suchen die Praxis überhaupt auftaucht.
- [ ] **Name, Adresse, Telefon zeichengleich** mit der Website eintragen — also exakt `Krankengymnastik Wim Menzo`, `Hauptstraße 18, 49835 Wietmarschen`, `05908 217`. Schon Abweichungen wie „Str." statt „Straße" drücken die Sichtbarkeit.
- [ ] **Alle 15 Leistungen** als Leistungen im Profil anlegen (Liste unten).
- [ ] **Öffnungszeiten** eintragen: Mo–Do 08:15–19:00, Fr 08:15–17:00, Sa/So geschlossen. Feiertage gesondert pflegen.
- [ ] **Echte Fotos** hochladen — Außenansicht, Empfang, Behandlungsraum. Profile mit Fotos werden deutlich häufiger angeklickt.
- [ ] **Rezensionen beantworten**, auch die älteren. Antworten sind ein eigenes Qualitätssignal.
- [ ] Website-Feld auf https://lukabpunkt.github.io/KG-Wim-Menzo/ setzen (bzw. später auf die eigene Domain).

## 2. Search Console einrichten — die Seite ist live

Die Website läuft seit dem 13.08.2026 unter **https://lukabpunkt.github.io/KG-Wim-Menzo/** (GitHub Pages, HTTPS). Alle Adressangaben — `canonical`, `og:url`, strukturierte Daten, `sitemap.xml` — sind darauf eingestellt.

- [ ] [Google Search Console](https://search.google.com/search-console) öffnen, Property vom Typ **URL-Präfix** mit genau dieser Adresse anlegen.
- [ ] Bestätigung über die HTML-Datei-Methode: Google gibt eine Datei wie `google1a2b3c.html` aus; diese ins Repository legen, committen, dann in der Search Console auf „Bestätigen" klicken.
- [ ] Unter „Sitemaps" `sitemap.xml` einreichen.
- [ ] Über „URL-Prüfung" die Indexierung anstoßen — sonst dauert es Wochen.
- [ ] Nach ein bis zwei Wochen prüfen, ob die Seite unter „Leistung" Impressionen sammelt.

### Wenn später eine eigene Domain dazukommt

Der Unterpfad `github.io/KG-Wim-Menzo/` funktioniert, wirkt für eine Praxis aber provisorisch, und GitHub Pages kann von einem Projektpfad nicht sauber weiterleiten. Bei einem Umzug sind es fünf Stellen:

| Datei | Was |
|---|---|
| `index.html` | `canonical`, `og:url`, `og:image` |
| `index.html` | im JSON-LD `url`, `image`, `logo` in beiden Knoten |
| `sitemap.xml` | `<loc>` und `<lastmod>` |
| `robots.txt` | `Sitemap:`-Zeile |
| Search Console | neue Property anlegen, Adressänderung melden |

**Wichtig:** Solange die alte Adresse in `canonical` steht, verweist auch die neue Domain dauerhaft auf `github.io` — Google würde dann weiterhin die alte Adresse ranken.

## 3. Falsche Verzeichniseinträge bereinigen

In Online-Verzeichnissen kursiert der Eintrag **„Lingener Str. 25 / 05925 1819"**. Er gehört nicht zu dieser Praxis. Widersprüchliche Adress- und Telefonangaben im Netz schwächen die lokale Sichtbarkeit aktiv — Google traut dann keiner der Angaben.

- [ ] Einträge bei Das Örtliche, Gelbe Seiten, 11880, jameda und Bing Places prüfen und korrigieren oder löschen lassen.

## 4. Die offenen Fragen beantworten

Die FAQ auf der Website beantwortet sechs Fragen. Diese sechs fehlen noch, weil nur die Praxis sie beantworten kann. Jede zusätzliche Antwort ist echter Inhalt und hilft messbar:

- [ ] Gibt es Parkmöglichkeiten direkt an der Praxis?
- [ ] Werden Hausbesuche angeboten?
- [ ] Werden Privatpatienten und Selbstzahler behandelt?
- [ ] Wie lange dauert es üblicherweise bis zum ersten Termin?
- [ ] Ist die Praxis barrierefrei zugänglich?
- [ ] Können Rezepte per Post geschickt werden?

## 5. Rechtstexte und Fotos nachliefern

- [ ] **Impressum** nach § 5 DDG: Name, Anschrift, Kontakt, gesetzliche Berufsbezeichnung und verleihender Staat, zuständige Aufsichtsbehörde und Kammer, berufsrechtliche Regelungen, USt-IdNr. falls vorhanden.
- [ ] **Datenschutzerklärung** — muss die Verarbeitung von Gesundheitsdaten, die Kontaktaufnahme per Telefon und E-Mail sowie die optionale Google-Maps-Einbindung beschreiben.
- [ ] **Praxis- oder Teamfoto** als Ersatz für den gekennzeichneten Platzhalter.

---

## Die 15 Leistungen (für das Unternehmensprofil zum Kopieren)

Krankengymnastik · Manuelle Therapie (OMT) · Bobath — Kinder / Erwachsene · Massagen · Osteopathische Behandlung · Craniosacrale Therapie · Manuelle Lymphdrainage · Sportphysiotherapie · Medizinische Trainingstherapie · CMD-Therapie · Triggertherapie · Wärme-/Kältetherapie · Elektrotherapie · Kinesio-Taping · Fußreflexzonenmassage

## Was auf der Website bereits erledigt ist

Titel und Beschreibung auf lokale Suchen ausgerichtet · strukturierte Daten als verknüpfter Graph mit geprüften Koordinaten, Öffnungszeiten, Bewertung und allen 15 Leistungen · FAQ-Sektion · Standortangaben · `robots.txt` und `sitemap.xml` vorbereitet · Vorschaubild für geteilte Links · Ladezeit unter einer Sekunde ohne einen einzigen externen Request · mobil einwandfrei ab 320 px · WCAG 2.1 AA.

## Was bewusst nicht gemacht wurde

Keine Keyword-Häufung, keine versteckten Texte, keine erfundenen Zertifikate, Jahreszahlen oder Preisangaben. Google prüft medizinische Inhalte nach den strengsten Qualitätsmaßstäben; solche Tricks kosten dort mehr, als sie bringen.
