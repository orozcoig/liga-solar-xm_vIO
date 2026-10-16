# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-10-16 10:50 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | SolarNet-Cuantiles (q50) | profe (reto 6) | 7 | 229.1 | 17.0% | -5.0% |
| 🥈 | SolarNet-Ponderada | profe (reto 3) | 7 | 237.8 | 17.6% | -2.4% |
| 🥉 | SolarNet-Ensamble×5 | profe (reto 5) | 7 | 245.3 | 18.2% | -8.0% |
| 4 | SolarNet-GRU | profe | 7 | 251.4 | 18.6% | -10.0% |
| 5 | SolarNet-Transformer | profe (reto 4) | 7 | 253.5 | 18.8% | -13.6% |
| 6 | SolarNet-Nubes | profe (reto 2) | 7 | 254.6 | 18.9% | -13.6% |
| 7 | SolarNet-CNN | profe (reto 4) | 7 | 256.7 | 19.0% | -18.1% |
| 8 | Persistencia | profe | 7 | 263.8 | 19.5% | — |
| 9 | Persistencia 3 días | profe (reto 1) | 7 | 266.0 | 19.7% | -20.1% |
| 10 | Persistencia × radiación | profe | 7 | 349.9 | 25.9% | -44.6% |

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
