# Portfoliooptimierung

> Markowitz, Efficient Frontier und die Instabilität der Kovarianzschätzung.

![Status](https://img.shields.io/badge/status-in%20progress-blue) ![Python](https://img.shields.io/badge/python-3.12-informational) ![Tests](https://img.shields.io/badge/tests-pytest-success)

## 1. Hypothese

Was vermute ich über den Markt, **bevor** ich getestet habe? Ein Satz, ökonomisch begründet.

## 2. Daten und Aufbereitung

| | |
|---|---|
| Quelle | |
| Zeitraum | |
| Frequenz | |
| Survivorship Bias | wie behandelt? |
| Fehlende Werte | |
| Splits / Dividenden | |

## 3. Methode

Modell, Parameter, und warum genau dieses. Formeln knapp, Herleitung im `docs/`-Ordner oder Notebook.

## 4. Validierung

Train/Test **in der Zeit** getrennt, Walk-Forward, Purging. Anzahl der getesteten Varianten (ehrlich zählen).

## 5. Transaktionskosten

Spread, Slippage, Gebühren. Ohne Kosten ist jeder Backtest eine Lüge.

## 6. Risikokennzahlen

| Kennzahl | In-Sample | Out-of-Sample |
|---|---|---|
| Sharpe | | |
| Sortino | | |
| Max Drawdown | | |
| Turnover | | |
| Hit Rate | | |

## 7. Gescheiterte Ansätze

Was wurde probiert und hat nicht funktioniert, und warum. Der wichtigste Abschnitt.

## 8. Out-of-Sample-Ergebnis

Der ehrliche Test auf nie gesehenen Daten. Ein Plot mit beschrifteten Achsen und Einheiten.

## 9. Grenzen

Wann bricht das Modell? Welches Regime killt es?

## Reproduzieren

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m src.run          # Hauptlauf
pytest                     # Tests
```

## Struktur

```text
src/        ausführbare Module
notebooks/  Exploration (nicht die Wahrheit)
tests/      ein Test pro Kernfunktion
data/       nur Beispiel- oder Downloadskripte, keine Rohdaten
docs/       Herleitungen, Plots
```

## Lizenz

MIT
