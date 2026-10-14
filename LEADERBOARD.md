# ☀️ Liga de Pronóstico Solar Colombia — Leaderboard

_Actualizado: 2026-10-14 11:14 (hora Colombia) · Métrica: MAE en horas de sol (06–18 h) · Skill = 1 − MAE/MAE_persistencia (positivo = le ganas a la persistencia)_

## 🏆 Liga oficial (predicciones hechas ANTES de conocer el dato real)

| # | Modelo | Autor | Días | MAE (MWh) | nMAE | Skill vs persistencia |
|---|---|---|---|---|---|---|
| 🥇 | Persistencia | profe | 5 | 188.6 | 12.8% | — |
| 🥈 | SolarNet-Ponderada | profe (reto 3) | 5 | 198.1 | 13.5% | -13.1% |
| 🥉 | SolarNet-Ensamble×5 | profe (reto 5) | 5 | 213.3 | 14.5% | -21.8% |
| 4 | SolarNet-Cuantiles (q50) | profe (reto 6) | 5 | 215.8 | 14.7% | -23.3% |
| 5 | SolarNet-GRU | profe | 5 | 217.1 | 14.8% | -23.5% |
| 6 | SolarNet-Transformer | profe (reto 4) | 5 | 228.5 | 15.5% | -30.4% |
| 7 | SolarNet-Nubes | profe (reto 2) | 5 | 230.5 | 15.7% | -30.9% |
| 8 | SolarNet-CNN | profe (reto 4) | 5 | 243.7 | 16.6% | -39.7% |
| 9 | Persistencia 3 días | profe (reto 1) | 5 | 246.8 | 16.8% | -40.5% |
| 10 | Persistencia × radiación | profe | 5 | 306.7 | 20.9% | -61.3% |

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
