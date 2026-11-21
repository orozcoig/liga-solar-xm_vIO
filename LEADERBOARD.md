# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-11-21 13:30 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-Cuantiles (q50) | profe (reto 6) | 43 | 227.0 | 15.2% | +27.1% |
| 🥈 | SolarNet-Ensamble×5 | profe (reto 5) | 43 | 227.3 | 15.2% | +26.9% |
| 🥉 | SolarNet-Ponderada | profe (reto 3) | 43 | 231.7 | 15.5% | +26.2% |
| 4 | SolarNet-CNN | profe (reto 4) | 43 | 231.9 | 15.5% | +23.6% |
| 5 | SolarNet-Nubes | profe (reto 2) | 43 | 235.1 | 15.7% | +25.4% |
| 6 | SolarNet-GRU | profe | 43 | 237.9 | 15.9% | +22.0% |
| 7 | SolarNet-Transformer | profe (reto 4) | 43 | 238.9 | 16.0% | +23.5% |
| 8 | Persistencia × radiación | profe | 43 | 273.4 | 18.3% | +19.2% |
| 9 | Persistencia 3 días | profe (reto 1) | 43 | 321.9 | 21.5% | +7.2% |
| 10 | Persistencia | profe | 43 | 392.7 | 26.3% | — |

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
