# CobbleCompanion: CobbleDollars/Create

Teil der **CobbleCompanion**-Familie — ein modulares Baukasten-System für Cobblemon-Server.
Siehe [Verwandte Module](#verwandte-module--related-modules) unten für alle Varianten.

**Kurzbeschreibung:**
Verbindet Create mit CobbleDollars: Lagerticker-Preise, Schlauer Beobachter und automatisierter
Verkauf.

## Beschreibung

Baut eine Brücke zwischen dem **Create**-Mod und der CobbleDollars-Wirtschaft:

- Live-Preisanzeige an Create-Lagertickern, synchronisiert mit deinem CobbleDollars-Kontostand.
- "Schlauer Beobachter" (Content Observer): automatische Verkaufszählung für Items, die per
  Create-Schacht in ein verlinktes Verkaufssystem wandern.
- Kaufladen-Integration (Buyshop) für per Lagerticker-Netzwerk verbundene Handelsposten.
- Kompatibel mit mobilen Create-Paketen (create_mobile_packages), sofern installiert.

**Abhängigkeiten:** CobbleCompanion: Basis + CobbleCompanion: CobbleDollars (beide erforderlich),
Create und CobbleDollars (beide erforderlich – ohne diese ist das Modul funktionslos).

---

## English

**Summary:**
Bridges Create and CobbleDollars: stock ticker prices, the smart content observer, and automated
selling.

## Description

Bridges the **Create** mod with the CobbleDollars economy:

- Live price display on Create stock tickers, synced with your CobbleDollars balance.
- "Content Observer": automatic sale counting for items funneled into a linked selling system via
  a Create chute.
- Buy-shop integration for trading posts linked through a stock ticker network.
- Compatible with mobile Create packages (create_mobile_packages), if installed.

**Dependencies:** CobbleCompanion: Basis + CobbleCompanion: CobbleDollars (both required), Create
and CobbleDollars (both required — the module does nothing without them).

---

## Bauen / Building

Aus Lizenzgründen liegen keine fremden Mod-Jars in `libs/` im Repo – du musst sie vor dem Bauen
selbst dort ablegen.
*No foreign mod jars ship in `libs/` for licensing reasons — place them there yourself before
building.*

**Eigene Abhängigkeiten (musst du selbst bauen) / Own dependencies (build them yourself):**
- `CobbleCompanion-Basis-*.jar` — aus [CobbleCompanion](https://github.com/siralusian/CobbleCompanion) bauen.
- `CobbleCompanion-CobbleDollars-*.jar` — aus [CobbleCompanion-CobbleDollars](https://github.com/siralusian/CobbleCompanion-CobbleDollars) bauen.

Beide jeweils mit `./gradlew jar`, das Ergebnis aus `build/libs/` hierher nach `libs/` kopieren.

**Erforderlich / Required:**
- `Cobblemon-neoforge-*.jar`, `CobbleDollars-neoforge-*.jar`
- `create-*.jar`, `architectury-*.jar`, `ponder-neoforge-*.jar` (Create-Kernabhängigkeiten)

**Optional:**
- `create_mobile_packages-*.jar`, `create_factory_abstractions-*.jar`

## Verwandte Module / Related modules

- [CobbleCompanion](https://github.com/siralusian/CobbleCompanion) — Basis
- [CobbleCompanion: CobbleDollars](https://github.com/siralusian/CobbleCompanion-CobbleDollars)
- [CobbleCompanion: CobbleDollars/CustomNPCs](https://github.com/siralusian/CobbleCompanion-CobbleDollars-CustomNPCs)
- [CobbleCompanion: CobblemonWorker](https://github.com/siralusian/CobbleCompanion-CobblemonWorker)
- [CobbleCompanion: Create/Let's Do](https://github.com/siralusian/CreateLetsDo)
- [CobbleCompanion: AllInOne](https://github.com/siralusian/CobbleCompanion-AllInOne)
- [CobbleCompanion: CobbleDollars-Bundle](https://github.com/siralusian/CobbleCompanion-CobbleDollarsBundle)
