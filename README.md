# GOLDSHIELD AI — Analysis Archive

Echte, unveränderte Export-Reports von **GoldShield AI** (GENITUS INC, [globalfintech.net](https://globalfintech.net)) —
AI-gestützte technische Marktanalyse über Aktien, Krypto, Forex und Anleihen. Jeder Report ist ein
echter Snapshot zum angegebenen Datum: Live-Marktdaten, technischer Score (0-2), Sentiment, KI-Einschätzung
(RSI, Momentum, SMA20, Volatilität) und die **Signal-Rendite** (Performance seit letztem Signalwechsel --
nur in Reports ab ca. August 2026 enthalten, ältere Exports hatten dieses Feld noch nicht).

**19 Reports** über **12 Symbole**, Juni–Oktober 2026.

> AI-generierte, computationale Analyse — keine Anlageberatung. Marktdaten können verzögert sein.

## Live-Index (durchsuchbar, sortierbar, filterbar)

**[Index öffnen](https://babybounce500.github.io/goldshield-ai-analysis-archive/)**

## Alle Reports

| Symbol | Datum | Sentiment | Preis | Signal-Rendite | Report |
|---|---|---|---|---|---|
| CBK.XETRA | 2026-10-21 | 🔴 Bearish | €37.25 | +7.59% | [HTML](reports/GLOBALO-CBK.XETRA-Analysis-2026-10-21.html) |
| SAP.XETRA | 2026-10-21 | 🟢 Bullish | €204.50 | +6.81% | [HTML](reports/GLOBALO-SAP.XETRA-Analysis-2026-10-21.html) |
| AIG | 2026-10-17 | 🟢 Bullish | $80.70 | +6.65% | [HTML](reports/GLOBALO-AIG-Analysis-2026-10-17.html) |
| 2269.HK | 2026-10-16 | 🔴 Bearish | HK$48.20 | +8.45% | [HTML](reports/GLOBALO-2269.HK-Analysis-2026-10-16.html) |
| RHM.XETRA | 2026-10-15 | 🟢 Bullish | €1,026.00 | +4.34% | [HTML](reports/GLOBALO-RHM.XETRA-Analysis-2026-10-15.html) |
| AIG | 2026-10-14 | 🟢 Bullish | $77.65 | +2.63% | [TXT](reports/GLOBALO-AIG-Analysis-2026-10-14.txt) |
| C | 2026-10-08 | 🔴 Bearish | $127.32 | +3.89% | [HTML](reports/GLOBALO-C-Analysis-2026-10-08.html) |
| CBK.XETRA | 2026-10-08 | 🔴 Bearish | €37.82 | +6.18% | [HTML](reports/GLOBALO-CBK.XETRA-Analysis-2026-10-08.html) |
| RHM.XETRA | 2026-10-08 | 🔴 Bearish | €936.00 | +5.45% | [TXT](reports/GLOBALO-RHM.XETRA-Analysis-2026-10-08.txt) |
| USDCAD.FOREX | 2026-10-07 | 🟢 Bullish | — | +2.29% | [HTML](reports/GLOBALO-USDCAD.FOREX-Analysis-2026-10-07.html) |
| USDCHF.FOREX | 2026-10-07 | 🟢 Bullish | — | +3.12% | [HTML](reports/GLOBALO-USDCHF.FOREX-Analysis-2026-10-07.html) |
| NG10Y.GBOND | 2026-09-25 | 🟢 Bullish | $335.92 | +7.17% | [HTML](reports/GLOBALO-NG10Y.GBOND-Analysis-2026-09-25.html) |
| BTC-USD.CC | 2026-09-16 | 🔴 Bearish | $75,951.21 | +0.81% | [HTML](reports/GLOBALO-BTC-USD.CC-Analysis-2026-09-16.html) |
| RHM.XETRA | 2026-09-01 | 🔴 Bearish | €1,110.80 | +3.79% | [HTML](reports/GLOBALO-RHM.XETRA-Analysis-2026-09-01.html) |
| MS | 2026-08-05 | 🟢 Bullish | — | — | [HTML](reports/GLOBALO-MS-Analysis-2026-08-05.html) |
| AAPL | 2026-07-31 | 🟢 Bullish | $333.43 | — | [TXT](reports/GLOBALO-AAPL-Analysis-2026-07-31.txt) |
| AAPL | 2026-07-30 | 🟢 Bullish | — | — | [HTML](reports/GLOBALO-AAPL-Analysis-2026-07-30.html) |
| RHM.XETRA | 2026-07-30 | 🟢 Bullish | — | — | [HTML](reports/GLOBALO-RHM.XETRA-Analysis-2026-07-30.html) |
| AAPL | 2026-06-08 | 🟢 Bullish | — | — | [HTML](reports/GLOBALO-AAPL-Analysis-2026-06-08.html) |

## Pipeline für weitere Reports

Neue Downloads landen als `GLOBALO-{SYMBOL}-Analysis-{YYYY-MM-DD}.{html,txt}` in `reports/`.
Skalierbar für sehr viele Reports (getestet für "tausende" laut Anforderung):
1. Dateien nach `reports/` kopieren (Duplikate per MD5/Export-Timestamp-Diff erkennbar)
2. Extraktionsskript läuft über alle Reports, parst Sentiment/Score/Preis/RSI/Momentum/Volatilität/
   Signal-Rendite per Regex in `data.json`
3. `index.html` lädt `data.json` clientseitig -- Suche/Sortierung/Filter laufen rein im Browser,
   keine Server-Komponente nötig, skaliert auf tausende Einträge ohne Umbau.

**Hinweis zu Screenshots:** ursprünglich sollten Kachel-Screenshots der Report-Karten genutzt werden,
aber das Original-Export-Template hat einen CSS-Bug (`var(--green)`/`var(--red)` werden im Export
referenziert, aber nie definiert) -- die Sentiment-Bar ist dadurch bei eigenständigem Rendering
unsichtbar. Screenshots sahen deshalb kaputt/leer aus. Stattdessen werden die Kennzahlen direkt aus
den Reports extrahiert und in eigens gestalteten Karten dargestellt -- sieht besser aus und skaliert
ohne Bild-Generierung pro Report.

---
© 2026 GENITUS INC. — GoldShield AI
