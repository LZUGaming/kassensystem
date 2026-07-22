# MARKT/24 Kassensystem

Ein browserbasiertes Kassenterminal (POS) zum Üben/Spielen — läuft komplett client-seitig, kein Server nötig.

**Features:**
- 87 Artikel aus 6 Warengruppen (Getränke, Obst/Gemüse, Backwaren, Wurst/Fleisch, Süßwaren, Molkereiprodukte)
- Warenkorb mit Netto/MwSt/Brutto-Berechnung, Bar/Karte, Rabatt
- Verkauf nur in ganzen Gebinden (Verpackungsgröße), Abrechnung pro Stück
- Alterssperre (18+) für alkoholische Getränke
- Lagerverwaltung mit Ein-/Ausbuchen (Wareneingang, Schwund, Beschädigt, Inventurkorrektur …)
- Kassenbestand (250,00 € Startbestand, real gestückelt) mit animierter Kassenlade
- Gegeben-Betrag per Schein-/Münz-Stückelung eintippen, live Rückgeld-Stückelung
- Storno auf allen Ebenen (letzter Artikel, Posten, Warenkorb, abgeschlossener Bon)
- Bons-Historie, Tagesabschluss/Z-Bericht, Ein-/Ausgänge-Protokoll
- Kassengeräusche (Scan, Storno, Fehler, Kassenlade)

## Als GitHub Pages veröffentlichen

1. Dieses Repo (mit `index.html` im Root) zu GitHub hochladen.
2. Im Repo: **Settings → Pages**.
3. Unter **Build and deployment** → Source: **Deploy from a branch**.
4. Branch: `main`, Ordner: `/ (root)` → **Save**.
5. Nach ca. 1 Minute ist die Seite live unter:
   `https://<dein-github-name>.github.io/<repo-name>/`

## Wichtiger Hinweis: reines Übungssystem

Das ist bewusst ein **Spiel-/Trainingssystem, kein Kassenbuch für echten Geschäftsbetrieb**. Die Datenbank
(IndexedDB im Browser) wird bei **jedem Laden der Seite komplett geleert und neu auf Standardwerte gesetzt**:

- Jeder Artikel wieder auf 30 Stk. Lagerbestand
- Kassenbestand wieder auf 250,00 € (in Standard-Stückelung)
- Bons, Ein-/Ausgänge-Protokoll und Tagesabschluss leer

Innerhalb einer Sitzung (ohne Neuladen) wird alles ganz normal live mitprotokolliert — nur beim nächsten
Seitenaufruf beginnt wieder alles bei null.
