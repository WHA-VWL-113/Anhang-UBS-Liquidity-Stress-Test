# UBS Kurzzeit-Stresstest (Kapitel 4)

Dieses Repository enthält die Daten und Berechnungsmodelle für die Analyse meiner Hausarbeit.

## Projektübersicht
Basierend auf den Daten der UBS Group AG (2023) wurde ein lineares Punktschätzungsmodell (Point Estimate) entwickelt, um die Überlebensfähigkeit der Bank in verschiedenen Stressszenarien zu prüfen.

### Datenbasis
* **Quelle:** UBS Group AG Geschäftsbericht 2023, S. 89–90.
* **HQLA Level 1:** 302.112 Mio. USD.
* **HQLA Level 2:** 29.456 Mio. USD.

### Szenarien im Modell
1. **Szenario A (Basel III Standard):** Reguläre LCR-Vorgaben ($k = 1.0$).
2. **Szenario B (CS-Benchmark):** Simulation basierend auf der CS-Krise im März 2023 ($k = 2.24$).
3. **Szenario C (Digital Flash Run):** Extremer Abfluss durch digitale Panik ($k = e^{1.54}$).

## Dateiinhalt
* `stresstest_ubs.ipynb`: Python-Notebook mit der Berechnung der Überlebensdauer.
* `ubs_lcr_data_2023.csv`: Exportierte LCR-Positionen inklusive Gewichtung.
