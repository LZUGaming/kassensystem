# MARKT/24 Kassensystem

Ein browserbasiertes Kassenterminal (POS) für einen Supermarkt/Kiosk — läuft komplett client-seitig, kein Server nötig.

**Features:**
- 87 Artikel aus 6 Warengruppen (Getränke, Obst/Gemüse, Backwaren, Wurst/Fleisch, Süßwaren, Molkereiprodukte)
- Warenkorb mit Netto/MwSt/Brutto-Berechnung, Gegeben/Rückgeld
- Verkauf nur in ganzen Gebinden (Verpackungsgröße), Abrechnung pro Stück
- Alterssperre (18+) für alkoholische Getränke
- Lagerverwaltung mit Wareneingang (Bestand einbuchen)
- Kassenbon nach Zahlungsabschluss

## Als GitHub Pages veröffentlichen

1. Dieses Repo (mit `index.html` im Root) zu GitHub hochladen.
2. Im Repo: **Settings → Pages**.
3. Unter **Build and deployment** → Source: **Deploy from a branch**.
4. Branch: `main`, Ordner: `/ (root)` → **Save**.
5. Nach ca. 1 Minute ist die Seite live unter:
   `https://<dein-github-name>.github.io/<repo-name>/`

## Hinweis

Lagerbestände und Warenkorb leben nur im Arbeitsspeicher des Browsers — ein Neuladen der Seite setzt sie auf den Ausgangswert zurück.
