# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-11-14 12:31 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-Ensamble×5 | profe (reto 5) | 36 | 238.3 | 16.1% | +25.9% |
| 🥈 | SolarNet-Cuantiles (q50) | profe (reto 6) | 36 | 238.5 | 16.1% | +26.3% |
| 🥉 | SolarNet-Ponderada | profe (reto 3) | 36 | 243.4 | 16.4% | +27.0% |
| 4 | SolarNet-CNN | profe (reto 4) | 36 | 245.9 | 16.6% | +22.3% |
| 5 | SolarNet-GRU | profe | 36 | 247.2 | 16.7% | +23.0% |
| 6 | SolarNet-Nubes | profe (reto 2) | 36 | 248.5 | 16.8% | +24.0% |
| 7 | SolarNet-Transformer | profe (reto 4) | 36 | 252.4 | 17.0% | +22.2% |
| 8 | Persistencia × radiación | profe | 36 | 284.9 | 19.2% | +18.2% |
| 9 | Persistencia 3 días | profe (reto 1) | 36 | 329.5 | 22.2% | +6.1% |
| 10 | Persistencia | profe | 36 | 404.3 | 27.3% | — |

![último día](resultados/ultimo_dia.png)

## 🧪 Backtest (días pasados, para arrancar en frío)

_Ojo: en el backtest el 'pronóstico' de clima es casi el clima observado → resultados optimistas._

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-GRU | profe | 30 | 149.7 | 9.8% | +43.5% |
| 🥈 | SolarNet-Cuantiles (q50) | profe (reto 6) | 30 | 154.1 | 10.1% | +42.1% |
| 🥉 | SolarNet-Ensamble×5 | profe (reto 5) | 30 | 157.2 | 10.3% | +41.5% |
| 4 | SolarNet-Nubes | profe (reto 2) | 30 | 158.2 | 10.4% | +41.3% |
| 5 | SolarNet-Transformer | profe (reto 4) | 30 | 160.0 | 10.5% | +39.9% |
| 6 | SolarNet-Ponderada | profe (reto 3) | 30 | 171.0 | 11.2% | +37.7% |
| 7 | SolarNet-CNN | profe (reto 4) | 30 | 178.3 | 11.7% | +33.4% |
| 8 | Persistencia × radiación | profe | 30 | 217.0 | 14.2% | +22.4% |
| 9 | Persistencia 3 días | profe (reto 1) | 30 | 268.5 | 17.6% | +14.1% |
| 10 | Persistencia | profe | 30 | 319.4 | 20.9% | — |

![backtest](resultados/backtest.png)
