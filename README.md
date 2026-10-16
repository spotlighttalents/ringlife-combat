# RINGLIFE Combat Series – Website

Fan-Website der RINGLIFE Combat Series (RCS). Eine statische Seite ohne Build-Schritt: `index.html` plus Bilder.

## Deploy auf Netlify

1. Netlify → **Add new site → Import an existing project → GitHub** → `spotlighttalents/ringlife-combat`
2. Branch: `main` · Build command: leer lassen · Publish directory: `.`
3. Deploy. Jeder Push auf `main` geht danach automatisch live.

Die Einstellungen stehen auch in `netlify.toml`.

## Formulare

Die Fighter-Bewerbung (`fighter-bewerbung`) und der Newsletter (`newsletter`) laufen über **Netlify Forms**.
Nach dem ersten Deploy unter **Site configuration → Forms** die Formularerkennung aktivieren (falls nicht automatisch an) und den Deploy neu anstoßen.
Benachrichtigungen per E-Mail: **Forms → Form notifications → Add notification → Email**.

Hinweis: Für einen echten Newsletter braucht es ein Double-Opt-in (z. B. Brevo, Mailchimp). Netlify sammelt die Adressen nur.

## Seiten

Die Unterseiten laufen über Anker in derselben Datei:

| Seite | Anker |
|---|---|
| Startseite | `/` |
| RCS 9 | `/#rcs-9` |
| Alle Events | `/#alle-events` |
| Fighter | `/#fighter` |
| Fighter-Profil (Beispiel) | `/#fighter-jan-yusufi` |
| Regeln | `/#regeln` |
| Tickets & FAQ | `/#tickets` |
| Fighter werden | `/#fighter-werden` |
| Impressum | `/#impressum` |
| Datenschutz | `/#datenschutz` |

## Vor dem Livegang offen

Gelb markierte Platzhalter (`class="ph"`) im Text:

- RCS 9: Einlasszeit, Ticketarten und Preise
- Impressum: Geschäftsführung, Registergericht und HRB, USt-IdNr., Kontakt-E-Mail, Verantwortlicher nach § 18 MStV
- Datenschutzerklärung (Pflicht, inkl. Netlify-Hosting, Netlify Forms, Google Fonts)
- Fighter-Profile und Fotos, Boxregeln, erlaubte Techniken und Fouls
- Allianz-Logo (aktuell Text), Link zum Fightwear-Shop
