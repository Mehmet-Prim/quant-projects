# Quant Projects

Fünf Grundlagenprojekte der quantitativen Finanzmathematik, gebaut während des ersten Studienjahres (B.Sc. Mathematik, Leibniz Universität Hannover, ab Oktober 2026). Jedes Projekt folgt derselben Regel: **Hypothese vor Code, Validierung in der Zeit, Kosten immer, gescheiterte Ansätze dokumentiert.**

| # | Projekt | Kern | Status |
|---|---|---|---|
| 1 | [Monte-Carlo-Simulation](01-monte-carlo/) | Zufallszahlen, Konvergenz, Varianzreduktion, Konfidenzintervalle | geplant · Winter 2026/27 |
| 2 | [Black-Scholes](02-black-scholes/) | Analytische Formel, numerische Lösung, Greeks, implizite Volatilität | geplant · Winter 2026/27 |
| 3 | [Binomialmodell](03-binomial-model/) | Konvergenz gegen Black-Scholes | geplant · Frühjahr 2027 |
| 4 | [Portfoliooptimierung](04-portfolio-optimization/) | Markowitz, Efficient Frontier, Kovarianz-Instabilität | geplant · Frühjahr 2027 |
| 5 | [Zufallsprozesse](05-stochastic-processes/) | Random Walk, Brownsche Bewegung, GBM | geplant · Sommer 2027 |

## Arbeitsregeln

- README zuerst, dann Code. Jede README hat dieselben neun Abschnitte (Hypothese, Daten, Methode, Validierung, Kosten, Risikokennzahlen, gescheiterte Ansätze, Out-of-Sample, Grenzen).
- Notebooks nur zum Explorieren; ausführbarer Code liegt in `src/`, ein Test pro Kernfunktion in `tests/`.
- Keine Rohdaten und keine Schlüssel im Repository. Daten werden per Skript geladen, Zugangsdaten kommen aus `.env`.
- Plots mit Achsenbeschriftung und Einheit.

## Einrichtung

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
for d in 0*/; do (cd "$d" && python -m pytest -q); done
```

## Lizenz

MIT
