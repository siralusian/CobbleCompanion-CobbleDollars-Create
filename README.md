# CobbleCompanion: CobbleDollars/Create

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/C3W0229LCP)

[🇩🇪 Deutsche Version weiter unten](#deutsch)

## English

Bridges Create and CobbleDollars: stock ticker prices, the smart content observer, and automated
selling. Part of the modular **CobbleCompanion** family for Cobblemon — usable in both singleplayer
and multiplayer, though this particular module (an automated shop system) is aimed squarely at
multiplayer servers with an economy.

### What it does

- Live price display on Create stock tickers, synced with your CobbleDollars balance.
- "Content Observer": automatic sale counting for items funneled into a linked selling system via
  a Create chute.
- Buy-shop integration for trading posts (CobbleMerchant) linked through a stock ticker network.
- Compatible with mobile Create packages (create_mobile_packages), if installed.

### How to use it

Most of the interactions below need **AdminOp** ([granted via
`/companion adminop <name>`](https://github.com/siralusian/CobbleCompanion#admin-access--professor-tab))
or, for the two block-editor shortcuts, real Minecraft operator status — this module is built for
whoever sets up the server's shop system, not something a regular player configures.

- **Edit a stock ticker's prices**: **Ctrl+right-click the stock ticker block** (requires real OP)
  to open the price editor instead of Create's normal order menu.
- **Configure a Content Observer ("Schlauer Beobachter")**: **Ctrl+right-click the block**
  (requires real OP) to open its settings. A normal right-click is blocked for non-OPs once it's
  configured; before that, Create's own filter-slot interaction works normally.
- **Link a CobbleMerchant to a stock ticker or payout chest** (AdminOp):
  1. Ctrl+right-click the merchant to start link mode.
  2. Ctrl+right-click a stock ticker (price source) or a chest (payout target) to link it.
  3. Ctrl+right-click the same merchant again to cancel.

  (Ctrl, not Shift, deliberately — Shift+right-click on Create blocks often opens a different menu.)

**Dependencies:** CobbleCompanion: Basis + CobbleCompanion: CobbleDollars (both required), Create
and CobbleDollars (both required — the module does nothing without them).

### Building

No foreign mod jars ship in `libs/` for licensing reasons — place them there yourself before
building.

**Own dependencies (build them yourself):**
- `CobbleCompanion-Basis-*.jar` — build from [CobbleCompanion](https://github.com/siralusian/CobbleCompanion).
- `CobbleCompanion-CobbleDollars-*.jar` — build from [CobbleCompanion-CobbleDollars](https://github.com/siralusian/CobbleCompanion-CobbleDollars).

Both via `./gradlew jar`, copy the result from `build/libs/` into `libs/` here.

**Required:**
- `Cobblemon-neoforge-*.jar`, `CobbleDollars-neoforge-*.jar`
- `create-*.jar`, `architectury-*.jar`, `ponder-neoforge-*.jar` (Create core dependencies)

**Optional:**
- `create_mobile_packages-*.jar`, `create_factory_abstractions-*.jar`

### Other CobbleCompanion projects

- [CobbleCompanion](https://github.com/siralusian/CobbleCompanion) — the base mod.
- [CobbleCompanion: CobbleDollars](https://github.com/siralusian/CobbleCompanion-CobbleDollars) —
  the CobbleDollars base this module builds on.
- [CobbleCompanion: CobbleDollars/CustomNPCs](https://github.com/siralusian/CobbleCompanion-CobbleDollars-CustomNPCs)
- [CobbleCompanion: CobblemonWorker](https://github.com/siralusian/CobbleCompanion-CobblemonWorker)
- [CobbleCompanion: Create/Let's Do](https://github.com/siralusian/CreateLetsDo)
- [CobbleCompanion: AllInOne](https://github.com/siralusian/CobbleCompanion-AllInOne) — this
  module plus everything else, in one file.
- [CobbleCompanion: CobbleDollars-Bundle](https://github.com/siralusian/CobbleCompanion-CobbleDollarsBundle) —
  this module plus the CustomNPCs integration, in one file.

---

## Deutsch

Verbindet Create mit CobbleDollars: Lagerticker-Preise, Schlauer Beobachter und automatisierter
Verkauf. Teil der modularen **CobbleCompanion**-Familie für Cobblemon – nutzbar im Singleplayer
und auf Servern, wobei dieses Modul (ein automatisiertes Shop-System) klar auf Multiplayer-Server
mit Wirtschaft ausgerichtet ist.

### Was es macht

- Live-Preisanzeige an Create-Lagertickern, synchronisiert mit deinem CobbleDollars-Kontostand.
- "Schlauer Beobachter" (Content Observer): automatische Verkaufszählung für Items, die per
  Create-Schacht in ein verlinktes Verkaufssystem wandern.
- Kaufladen-Integration (Buyshop) für per Lagerticker-Netzwerk verbundene Handelsposten
  (CobbleMerchant).
- Kompatibel mit mobilen Create-Paketen (create_mobile_packages), sofern installiert.

### Benutzung

Die meisten der folgenden Interaktionen brauchen **AdminOp** ([vergeben über
`/companion adminop <Name>`](https://github.com/siralusian/CobbleCompanion#admin-zugang--professor-tab))
oder, bei den beiden Block-Editor-Abkürzungen, echten Minecraft-Operator-Status – dieses Modul ist
für die Person gebaut, die das Server-Shop-System einrichtet, nicht für die normale Spieler-Nutzung.

- **Preise eines Lagertickers bearbeiten**: **Strg+Rechtsklick auf den Lagerticker-Block**
  (erfordert echten OP) öffnet den Preis-Editor statt Creates normalem Bestell-Menü.
- **Schlauen Beobachter konfigurieren**: **Strg+Rechtsklick auf den Block** (erfordert echten OP)
  öffnet die Einstellungen. Ein normaler Rechtsklick ist für Nicht-OPs blockiert, sobald er
  konfiguriert ist; davor funktioniert Creates eigene Filter-Slot-Interaktion normal.
- **CobbleMerchant mit Lagerticker/Auszahlungs-Kiste verknüpfen** (AdminOp):
  1. Strg+Rechtsklick auf den Merchant startet den Verknüpfungs-Modus.
  2. Strg+Rechtsklick auf einen Lagerticker (Preisquelle) oder eine Kiste (Auszahlungsziel)
     verknüpft ihn.
  3. Erneutes Strg+Rechtsklick auf denselben Merchant bricht ab.

  (Bewusst Strg statt Umschalt – Umschalt+Rechtsklick öffnet bei Create-Blöcken oft ein anderes
  Menü.)

**Abhängigkeiten:** CobbleCompanion: Basis + CobbleCompanion: CobbleDollars (beide erforderlich),
Create und CobbleDollars (beide erforderlich – ohne diese ist das Modul funktionslos).

### Bauen

Aus Lizenzgründen liegen keine fremden Mod-Jars in `libs/` im Repo – du musst sie vor dem Bauen
selbst dort ablegen.

**Eigene Abhängigkeiten (musst du selbst bauen):**
- `CobbleCompanion-Basis-*.jar` — aus [CobbleCompanion](https://github.com/siralusian/CobbleCompanion) bauen.
- `CobbleCompanion-CobbleDollars-*.jar` — aus [CobbleCompanion-CobbleDollars](https://github.com/siralusian/CobbleCompanion-CobbleDollars) bauen.

Beide jeweils mit `./gradlew jar`, das Ergebnis aus `build/libs/` hierher nach `libs/` kopieren.

**Erforderlich:**
- `Cobblemon-neoforge-*.jar`, `CobbleDollars-neoforge-*.jar`
- `create-*.jar`, `architectury-*.jar`, `ponder-neoforge-*.jar` (Create-Kernabhängigkeiten)

**Optional:**
- `create_mobile_packages-*.jar`, `create_factory_abstractions-*.jar`

### Weitere CobbleCompanion-Projekte

- [CobbleCompanion](https://github.com/siralusian/CobbleCompanion) — die Basis-Mod.
- [CobbleCompanion: CobbleDollars](https://github.com/siralusian/CobbleCompanion-CobbleDollars) —
  die CobbleDollars-Basis, auf der dieses Modul aufbaut.
- [CobbleCompanion: CobbleDollars/CustomNPCs](https://github.com/siralusian/CobbleCompanion-CobbleDollars-CustomNPCs)
- [CobbleCompanion: CobblemonWorker](https://github.com/siralusian/CobbleCompanion-CobblemonWorker)
- [CobbleCompanion: Create/Let's Do](https://github.com/siralusian/CreateLetsDo)
- [CobbleCompanion: AllInOne](https://github.com/siralusian/CobbleCompanion-AllInOne) — dieses
  Modul plus alles andere, in einer Datei.
- [CobbleCompanion: CobbleDollars-Bundle](https://github.com/siralusian/CobbleCompanion-CobbleDollarsBundle) —
  dieses Modul plus die CustomNPCs-Anbindung, in einer Datei.
