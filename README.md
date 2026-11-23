# Physiotherapie Braumann: Onepager-Entwurf

Entwurf für die Modernisierung von www.physiotherapie-braumann-sabine.de
(Physiotherapie Praxis "Dr. Gerhard Strube", Inh. Sabine Braumann, Oebisfelde).

Dies ist ein Showcase. Die offizielle Seite der Praxis ist weiterhin
www.physiotherapie-braumann-sabine.de. Der Entwurf ist per `noindex` von
Suchmaschinen ausgeschlossen.

## Aufbau

Reine statische Seite ohne Build-Schritt und ohne externe Abhängigkeiten.

| Datei | Inhalt |
|---|---|
| `index.html` | Onepager: Hero, Über uns, Leistungen, Therapien, Hausbesuche, Kontakt mit OpenStreetMap (lädt erst nach Klick) |
| `impressum.html` | Impressum-Vorlage |
| `datenschutz.html` | Datenschutz-Vorlage (Hosting bei IONOS angenommen) |
| `style.css` | Gesamtes Styling, Farben als Tokens in `:root` (Palette 60-30-10) |
| `fonts/` | Bricolage Grotesque, lokal eingebunden (keine Anfrage an Google), Lizenz in `fonts/OFL.txt` |
| `img/` | Logo (freigestellt), Favicon- und Touch-Icons |
| `favicon.ico` | Browser-Tab-Icon (Biene aus dem Logo) |

## Lokal ansehen

```
python -m http.server 8765
```

Danach http://localhost:8765 öffnen.

## Vor einer echten Veröffentlichung

- Gelb markierte Platzhalter in `impressum.html` und `datenschutz.html` ausfüllen und rechtlich prüfen lassen.
- `noindex` in `index.html` entfernen.
- Logo als SVG oder größere PNG (mindestens 600 px breit) von der Praxis besorgen.
- Den Hinweis "Gut zu wissen" zum Hausbesuch auf Kassenrezept von der Praxis bestätigen lassen.
