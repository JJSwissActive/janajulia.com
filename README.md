# Jana Julia Kramer – Website

**Small Steps. Big Dreams.** · Offizielle Website von Jana Julia Kramer · **https://janajulia.com**
Betreut von ihren Eltern David & Fabienne Kramer.

Diese Anleitung erklärt in einfachen Schritten:

1. [Netlify einrichten (einmalig)](#1-netlify-einrichten-einmalig)
2. [Ein Resultat eintragen](#2-ein-resultat-eintragen)
3. [Ein Bild austauschen](#3-ein-bild-austauschen)
4. [Gut zu wissen](#4-gut-zu-wissen)

Es braucht **keine Programmierkenntnisse** und **keine Software** – alles geht im Browser.

---

## 1. Netlify einrichten (einmalig)

Netlify macht die Website öffentlich erreichbar. Jede Änderung hier auf GitHub ist danach **nach wenigen Sekunden automatisch online**.

1. Auf **https://app.netlify.com/signup** mit **«Sign up with GitHub»** (Konto JJSwissActive) anmelden – der kostenlose Plan genügt.
2. **«Add new project» → «Import an existing project» → «GitHub»** → Repository **`janajulia.com`** auswählen.
3. Einstellungen:
   - **Branch to deploy:** `main`
   - **Base directory:** leer lassen
   - **Build command:** leer lassen
   - **Publish directory:** `.` (nur ein Punkt)
4. **«Deploy»** klicken.
5. **Domains** (Project configuration → **Domain management**):
   - **«Add a domain»** → `janajulia.com` → als **Primary domain** festlegen
   - **«Add domain alias»** → `janajulia.ch`
   - Netlify zeigt die nötigen **DNS-Einträge** an → beim Domain-Anbieter eintragen. Das **https-Zertifikat** stellt Netlify danach automatisch und gratis aus.
   - `janajulia.ch` und `www.…` leiten automatisch auf **janajulia.com** weiter (Datei `_redirects`).

---

## 2. Ein Resultat eintragen

*Dauer: ca. 2 Minuten*

1. Hier auf GitHub den Ordner **`js`** öffnen → Datei **`results.js`** anklicken.
2. Oben rechts auf das **Stift-Symbol ✏️** (Edit) klicken.
3. Eine bestehende Zeile **kopieren** und darunter einfügen, dann anpassen. Aufbau:

   ```
   Datum | Anlass | Ort | Art | Distanz | Kategorie | Rang | Resultat-Link
   ```

   Beispiel:

   ```
   21.11.2026 | Basler Stadtlauf | Basel | Strasse | 1'000 m | U12 | 1 | https://datasport.com/...
   ```

   | Feld | So ausfüllen |
   |---|---|
   | **Datum** | `TT.MM.JJJJ`, z. B. `21.11.2026` |
   | **Art** | `Bahn`, `Strasse`, `Cross` oder `Triathlon` (für die Filter) |
   | **Rang** | nur die Zahl, z. B. `1`. **Leer lassen** = angemeldet → erscheint unter «Next Races» |
   | **Resultat-Link** | offizieller Link zur Rangliste (darf fehlen) |

4. Oben rechts **«Commit changes…»** → nochmals **«Commit changes»**.
5. Fertig. Nach wenigen Sekunden ist das Resultat online – **Siege, Podestplätze und Anzahl Rennen werden automatisch neu gezählt**, sortiert wird automatisch (neueste zuerst).

**Tipps**
- Ein angemeldetes Rennen ist schon drin? Einfach bei dieser Zeile **Rang und Link ergänzen** – es wandert dann automatisch von «Next Races» in die Resultate.
- Resultate eines **neuen Jahres** einfach dazuschreiben – die Jahresauswahl erscheint automatisch.
- Ist eine Zeile fehlerhaft (z. B. falsches Datum), wird **nur diese Zeile weggelassen** – der Rest der Tabelle bleibt sichtbar.
- Bitte keine **`** (Backtick-Zeichen) im Text verwenden.

---

## 3. Ein Bild austauschen

*Dauer: ca. 3 Minuten*

1. Neues Bild vorbereiten:
   - **Gleicher Dateiname** wie das alte Bild (siehe Tabelle unten)
   - **Format `.webp`** – ein JPG/PNG lässt sich gratis auf **https://squoosh.app** umwandeln (rechts «WebP» wählen, Qualität ca. 80)
   - **Ähnliches Seitenverhältnis** wie das alte Bild, Jana eher in der Bildmitte und mit etwas Luft über dem Kopf
2. Den passenden Ordner öffnen, z. B. `assets/images/highlights`.
3. **«Add file» → «Upload files»** → Bild hineinziehen → **«Commit changes»**. Das alte Bild mit gleichem Namen wird ersetzt.
4. Fertig – nach wenigen Sekunden ist das neue Bild online (evtl. Seite neu laden).

| Bereich | Datei | Format (Breite × Höhe) |
|---|---|---|
| Titelbild Computer | `assets/images/hero/hero-desktop.webp` | Querformat 16:9 (3200 × 1800) – Jana rechts, links Platz für Text |
| Titelbild Handy | `assets/images/hero/hero-mobile.webp` | Hochformat (1200 × 2982) |
| My Story | `assets/images/story/story-portrait.webp` | Hochformat 4:5 |
| My Sports | `assets/images/sports/running.webp`, `cross-country.webp`, `triathlon.webp` | Hochformat 4:5 |
| Highlights | `assets/images/highlights/swiss-final.webp`, `zofingen.webp`, `baeren-gp.webp` | Querformat 3:2 |
| What's Next | `assets/images/next/track-2027.webp`, `triathlon-2027.webp` | Querformat 4:3 |
| Sponsor | `assets/images/partner/sommertee-produkt.webp` | Querformat 16:9 |
| Gönner / Vereine | `assets/images/partner/logo-*.png`, `assets/images/team/logo-*.png` | Logo, transparenter Hintergrund |
| Team | `assets/images/team/team-01.webp`, `team-02.webp` | Quadratisch |
| Presse (Karte) | `assets/images/medien/medien-01.webp` … `-04.webp` | Querformat 3:2 |
| Presse (gross, Klick) | `assets/images/medien/gross/medien-01.webp` … `-04.webp` | ganzer Artikel, gut lesbar |
| Instagram | `assets/images/instagram/insta-01.webp` … `-06.webp` | Quadratisch (1080 × 1080) |
| Vorschau beim Teilen | `assets/images/og-image.jpg` | 1200 × 630 (JPG) |

**Neue Bilder an neuen Stellen** (z. B. ein weiterer Presseartikel, eine zusätzliche Karte) brauchen eine kleine Anpassung im Code → dafür Hilfe holen.

---

## 4. Gut zu wissen

- **Änderungen bündeln:** Jedes «Commit changes» veröffentlicht die Seite neu. Der kostenlose Netlify-Plan hat ein monatliches Kontingent – mehrere Resultate also lieber **auf einmal** eintragen.
- **Google:** Die Seite ist für Suchmaschinen freigegeben (Sitemap: `https://janajulia.com/sitemap.xml`). Für Statistiken zur Google-Suche die **Google Search Console** verwenden – sie braucht keinen Cookie-Banner.
- **Datenschutz:** Die Seite verwendet **keine Cookies und kein Tracking** und lädt nichts von Drittanbietern (auch die Schriften liegen auf dem eigenen Server). Darum braucht es **keinen Cookie-Banner** – auch die Google Search Console ändert daran nichts.
- **Impressum & Datenschutz** stehen in `impressum.html`.
- **Hilfe:** Mitarbeitende mit Zugriff (GitHub → Settings → Collaborators) können Änderungen direkt hier vornehmen.

---

*Die Website ist bewusst schlank gebaut (reines HTML, CSS und JavaScript, ohne Baukasten) – sie lädt schnell und braucht keine Updates oder Wartung.*
